El operador **||** permite concatenar textos.

La consulta

``` sql
SELECT "Hola" || " " || "Mundo" as saludo from clientes;
```

va a traer el texto "Hola Mundo". Con esta misma ideas, podríamos utilizar columnas en vez de textos literales.

Tu objetivo es:

> Hacer una consulta que traiga UNA SOLA COLUMNA que tenga el nombre y el apellido de los clientes separados con espacio. La columna debe llamarse "nombre completo"
