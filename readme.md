## Daniel Alejandro Ordoñez Clavijo 67000567


# Explicacíon del codigo:

En la busqueda para solucionar el problema, no encontre una manera sencilla de hacerlo sando la libreria smtplib, en su reemplazo encontre otra, llamada  FLask Mail que esta hecha para hacer uso de SMTP desde flask.

# Gmail
Dado una actualización del año pasado en Gmail no deja cambiar la opción de aplicaciones menos seguras, por lo que tuve que buscar una alternativa.

## Autentificacion en dos pasos y clave de aplicación

En uno de los apartados de seguridad del correo, toca habilitar la opción de autentificación en dos pasos, la cual habilita la opción de claves de aplicación, se llenan dos apartados y da la contraseña que agregue en 'MAIL_PASSWORD'

# Linea 7 a 13 main.py

Todo este apartado hace referencia a la configuración que nos da Flask Mail.

## HTML y CSS
Por facilidad, decidi no usar CSS, si no solo llamar a bootstrap.
Pero para tener completo el trabajo, decidi configurar el boton que viene por default en bootstrap, asignandole un estilo llamado desde la carpeta "static/css/style.css". con el siguiente href dentro del elemento 

```
<link href="{{ url_for('static', filename='css/style.css') }}">
```

## main.py

El resto del codigo es el llamado a las clases hechas en el html, donde recoge lo escrito en el asunto, correo y comentario. 

El codigo utiliza los protocolos HTTP GET y POST
