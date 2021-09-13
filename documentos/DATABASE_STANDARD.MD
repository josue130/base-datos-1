
# *Introducción*

En esta tarea se tiene como objetivo la investigación de los diferentes estándares de nombres para generar código en SQL, En la tarea se deberá elegir un estándar de todos los investigados, el estándar elegido tiene que cumplir todos los **requisitos** que se piden en la tarea.


# *Justificación*

Después de la investigación llegue a evaluar un estándar que me parecía familiar, el estándar "PascalCase", es el estándar que he utilizado a lo largo de mi tiempo programando sin saberlo, es uno de los estándares que más facilitan el entendimiento del código para entidades, atributos, tipos de datos, llaves primarias, llaves foráneas e índices. 

# *Estandar para entidades*
Se utiliza la letra mayuscula para el comienzo de cada palabra en la entidad.

Ejemplo:

**Create Table PascalCase**(

	NombreEjemplo varchar(30) not null
	
);

# *Estandar para atributos*
Se utiliza la primera letra en mayuscula para el comienzo de la pralabra, si el nombre del atributo incluye dos palabras cada palabra empezara en mayuscula.
Ejemplo:

**Create Table PascalCase**(

	Nombre varchar(30) not null,
	FechaPrestamo date
	
);






                                                           
