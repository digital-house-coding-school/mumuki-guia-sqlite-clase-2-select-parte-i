Del mismo modo que los productos tienen marcas...también tienen categorías!

Conozcamos esta nueva tabla:

<div
  class='mu-erd'
  data-entities='{
    "categorias": {
      "id": {
        "type": "Integer",
        "pk": true
      },
      "nombre": {
        "type": "Text"
      },
      "id_categoria_padre" : {
        "type": "Integer",
        "fk": {
          "to": { "entity": "categorias", "column": "id" },
          "type": "many_to_one"
        }
      }
    }
  }'>
</div>

Para este ejercicio:

> Hace una consulta que traiga todos los datos de todas las categorías