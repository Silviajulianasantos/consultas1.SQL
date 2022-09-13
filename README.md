# consultas1.SQL

# EJERCICIOS CONSULTAS SQL

## Tabla de usuario

![Usuario](img/usuario.png "Usuario")

1. Para visualizar toda la informacion que contiene la tabla `usuario` se puede incluir con la instruccion SELECT el caracter'*' o cada uno de los campos 

SELECT * FROM `Usuario` 

![Consulta1](img/Consulta1.png "Consulta1")

2. Visualizar solamente la identificacion del usuario 

SELECT `identificacion` FROM `Usuario` 

![Consulta2](img/Consulta2.png "Consulta2")

3. Se desea obtener los registros cuya identificacion sean mayorres o iguales a 150, se debe utilizar la clausula WHere que especifica las condiciones que debe reunir los registros que se van a seleccionar 

SELECT * FROM `Usuario` WHERE identificacion>=`150`

![Consulta3](img/Consulta3.png "Consulta3")

4. Si se desea obtener los registros cuyo sus apellidos sean Vanegas o Cetina, se debe utilizar el operador IN que especifica los registros que se quieren visualizar de una tabla

SELECT `apellidos` FROM `Usuario` WHERE apellidos IN ('Vanegas','Cetina')

![Consulta4](img/Consulta4.png "Consulta4")

O se puede utilizar el operador OR 

SELECT `apellidos` FROM `Usuario` WHERE apellidos='Vanegas' OR apellidos='Cetina'

![Consulta4](img/Consulta4.2.png "Consulta4.2")

5. Si se desea obtener los registros cuya identificacion sea menor de '110' y la ciudad sea 'Cali', se debe utilizar el operador AND

SELECT * FROM `Usuario` WHERE identificacion<'110' AND ciudad_nac='Cali'

![Consulta5](img/Consulta5.png "Consulta5")

6. Si se desea obtener los regidtros cuyos nombres empiecen por la letra 'A', se debe utilizar el operador LIKE que utiliza los patrones '%' (todos) y ' ' (caracter)

SELECT * FROM `Usuario` WHERE nombre LIKE 'A%'

![Consulta6](img/CONSULTA6.png "Consulta6")

7. Si desea obtener los registros cuyos nombres contengan la letra 'a'

SELECT * FROM `Usuario` WHERE nombre LIKE '%a%'

![Consulta7](img/consulta7.png "Consulta7")

8. Si se desea obtener los registros donde la cuarta letra del nombre sea una 'a'

SELECT * FROM `Usuario` WHERE nombre LIKE'___a%'

![Consulta8](img/consulta8.png "Consulta8")