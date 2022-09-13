# consultas1

#  EJERCICIOS CONSULTAS SQL

## Tabla usuario

![tabla usuario](img/tabla_usuario.png "Tabla usuario")

1. Para visualisar toda la informacion que contiene la tabla `usuario` se puede incluir con la instruccion SELECT el caracter '*' o cada uno de los campos de la tabla
`select * from usuario` 

![Consulta1](img/Consulta1.png "Consulta1")

2. Visualizar solamente la identificacion del usuario.

`select identificacion from usuario`

![Consulta2](img/Consulta2.png "Consulta2")

3. Si se desea optener los registros cuya identificacion mayor o igual a 150 se debe utilizar la clausula WHERE que especifica las condiciones que debe reunir los registros que se van a seleccionar 

`SELECT * FROM usuario WHERE identificacion>=` '150'

![Consulta3](img/Consulta3.png "Consulta3")

4. Si se desea obtener los regitros cuyo sus apellidos sean Vnegas o Cetina se debe utilizar el operador IN que especifica los registros que se quieren visualizar de una tabla

`SELECT apellidos FROM usuario WHERE apellidos IN ('Vanegas','Cetina')`

![Consulta4](img/Consulta4.png "Consulta4")

O se puede utilizar el operador OR

`SELECT apellidos FROM usuario WHERE apellidos='Vanegas' OR apellidos='Cetina'`

![Consulta4](img/Consulta4_2.png "Consulta4")

5. Si se desea obtener los registros cuya identificacion sea menor de '110' y la ciudad sea 'Cali' se debe utilizar el operador AND

![Consulta5](img/Consulta5.png "Consulta5")

6. Si se desea obtener los registros cuyos nombres empiecen por la letra 'A' se debe utilizar el operador LIKE que utiliza los patrones'%' (todos) y '_' (caracter)

`SELECT * FROM usuario WHERE nombre LIKE'A%'`

![Consulta6](img/Consulta6.png "Consulta6")

7. Si desea obtener los registros cuyos nombres contengan la letra 'a' 

`SELECT * FROM usuario WHERE nombre LIKE '%a%'`

![Consulta7](img/Consulta7.png "Consulta7")
