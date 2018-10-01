Queda una última tabla para explorar. La tabla de ventas.

Esta tabla va a ser la que una los productos con los clientes, siendo una relación de **muchos a muchos**. Esto es porque un cliente puede comprar muchos productos (Por ejemplo manzanas rojas y manzanas verdes) y a su vez las manzanas rojas pueden ser compradas por muchos clientes!

De este modo, nuestro diagrama se ve así:

<div
  class='mu-erd'
  data-entities='{
    "clientes": {
      "id": {
        "type": "Integer",
        "pk": true
      },
      "nombre": {
        "type": "Text"
      },
      "apellido" : {
        "type": "Text"
      }
    },
    "ventas": {
      "id": {
        "type": "Integer",
        "pk": true
      },
      "id_cliente" : {
        "type": "Integer",
        "fk": {
          "to": { "entity": "clientes", "column": "id" },
          "type": "many_to_one"
        }
      },
      "id_producto" : {
        "type": "Integer",
        "fk": {
          "to": { "entity": "productos", "column": "id" },
          "type": "many_to_one"
        }
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
          "to": { "entity": "producto", "column": "id" },
          "type": "many_to_one"
        }
      },
      "id_marca" : {
        "type": "Integer",
        "fk": {
          "to": { "entity": "producto", "column": "id" },
          "type": "many_to_one"
        }
      }
    }
  }'>
</div>

Para este último ejercicio te vamos a pedir una consulta que explore las 3 tablas!!!

Para esto, es importante aclarar en el **WHERE** donde estan las relaciones que unen a estas tablas para que traiga los datos realmente relevantes.

Dado esto, queremos una consulta que nos permita visualizar a los clientes y que productos compraron.

En el resultado deberían verse únicamente, nombre y apellido del cliente y el nombre del producto.

¡Éxitos!