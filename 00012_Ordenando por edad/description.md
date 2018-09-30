Para este último ordenamiento vamos a pedirte:

> 1. Trae únicamente nombre, apellido, teléfono y fecha de nacimiento

> 2. De aquellos personas cuyo telefono NO SEA NULO

> 3. Ordenados por fecha de nacimiento DESCENDENTEMENTE

Te recordamos la estructura de la tabla por si no la tenes en mente: 

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
