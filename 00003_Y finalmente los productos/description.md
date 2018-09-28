Cerrando nuestro esquema un poco más completo, se ve de la siguiente manera:

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
        "type": "Integer"
      }
    },
    "productos": {
      "id": {
        "type": "Integer",
        "pk": true
      },
      "nombre": {
        "type": "Text"
      },
      "modelo": {
        "type": "Text"
      },
      "descripcion": {
        "type": "Text"
      },
      "precio": {
        "type": "Real"
      },
      "puntuacion": {
        "type": "Real"
      },
      "id_categoria" : {
        "type": "Integer",
        "fk": {
          "to": { "entity": "categorias", "column": "id" },
          "type": "many_to_one"
        }
      },
      "id_marca" : {
        "type": "Integer",
        "fk": {
          "to": { "entity": "marcas", "column": "id" },
          "type": "many_to_one"
        }
      }
    },
    "marcas": {
      "id": {
        "type": "Integer",
        "pk": true
      },
      "nombre": {
        "type": "Text"
      }
    }
  }'>
</div>

Como verán, en el esquema, la columna `id_marca` hace referencia a una marca, mientras que `id_categoria` hace referencia a la categoría del producto.

Para este ejercicio:

> Hace una consulta que traiga todos los datos de todos los productos