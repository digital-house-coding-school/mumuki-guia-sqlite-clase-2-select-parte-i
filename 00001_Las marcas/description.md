Es hora de trabajar con una nueva base de datos. En este caso estaremos trabajando con un pequeño e-commerce que hará una venta de productos.

Para comenzar, nuestros productos tendrán categorías con lo cual, conozcamos la primer tabla:

<div
  class='mu-erd'
  data-entities='{
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

Para este primer ejercicio:

> Hace una consulta que traiga todos los datos de todas las marcas