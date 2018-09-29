Resulta que también existe una tabla de clientes con la siguiente estructura:

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
      "apellido": {
        "type": "Text"
      },
      "email": {
        "type": "Text"
      },
      "telefono": {
        "type": "Text"
      },
      "celular": {
        "type": "Text"
      },
      "fecha_de_nacimiento": {
        "type": "Datetime"
      },
      "id_producto_preferido" : {
        "type": "Integer"
      }
    }
  }'>
</div>

Dada esta nueva tabla te pedimos lo siguiente:

> Realiza una consulta que traiga todos los clientes ordenados por nombre.