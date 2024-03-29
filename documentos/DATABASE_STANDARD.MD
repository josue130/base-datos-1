<!--ts-->
# Índices
* [Introducción](#introducción)
* [Justificación](#justificación)
* [Estandar para entidades](#estandar-para-entidades)
* [Estandar para atributos](#estandar-para-atributos)
* [Estandar para llaves primarias](#estandar-para-llaves-primarias)
* [Estandar para llaves foráneas](#estandar-para-llaves-foráneas)
* [Estandar para índices](#estandar-para-índices)
<!--te-->


# *Introducción*

En esta tarea se tiene como objetivo la investigación de los diferentes estándares de nombres para generar código en SQL, En la tarea se deberá elegir un estándar de todos los investigados, el estándar elegido tiene que cumplir todos los **requisitos** que se piden en la tarea. El estandar a utilizar es el "PascalCase".


# *Justificación*

Después de la investigación llegue a evaluar un estándar que me parecía familiar, el estándar "PascalCase", es el estándar que he utilizado a lo largo de mi tiempo programando sin saberlo, es uno de los estándares que más facilitan el entendimiento del código para entidades, atributos, tipos de datos, llaves primarias, llaves foráneas e índices. 

# *Estandar para entidades*
Se utiliza la letra mayúscula para el comienzo de cada palabra en la entidad. Ejemplo:

**Create Table PascalCase**(

	NombreEjemplo varchar(30) not null
	
);

# *Estandar para atributos*
Se utiliza la primera letra en mayúscula para el comienzo de la palabra, si el nombre del atributo incluye dos palabras cada palabra empezara en mayúscula. Ejemplo:

Create Table PascalCase(

	Nombre varchar(30) not null,
	FechaPrestamo date
	
);

# *Estandar para llaves primarias*
Para las llaves primarias se utiliza de igual manera la letra en mayúscula para el comienzo de la palabra, si el nombre del atributo incluye dos palabras cada palabra empezara en mayúscula. Ejemplo:

Create Table PascalCase(

	Nombre varchar(30) primary key o NombreUsuario varchar(30) primary key
);


Una excepción en este estándar es el uso Pk que suele ser utilizado al inicio de llave primaria o final con un guion bajo. Ejemplo:

Create Table PascalCase(

	Nombre_Pk varchar(30) primary key o Pk_NombreUsuario varchar(30) primary key
);

# *Estandar para llaves foráneas*
Para las llaves foráneas se utiliza de igual manera la letra en mayúscula para el comienzo de la palabra, si el nombre del atributo incluye dos palabras cada palabra empezara en mayúscula, se utiliza el distintivo Fk para el nombre al inicio o al final con un guion bajo. Ejemplo:

create table PascalCase(

	Constraint Fk_Carnet Foreign Key (Carnet) References Estudiante(Carnet),
	Constraint CodigoLibro_Fk Foreign key (CodigoLibro) References Libro(Codigo)
	
	);
# *Estandar para índices*
Para el estandar de indices se utiliza de igual manera la letra en mayúscula en el comienzo de la palabra. Ejemplos:

Create Unique Clustered Index LibrosCodigo On Libros(Codigo);

Create NonClustered Index LibrosTitulo On Libros(Titulo);








                                                           
