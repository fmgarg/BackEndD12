# Desafío "Usando el objeto PROCESS". 

Este proyecto se encuentra realizado utilizando JS, NodeJS, express, express-handlebars, express-session, passport-local, sockets.io y bootstrap, entre otras.

Al ingresar a la ruta localhost:8080/info encontrarás información que se obtiene a través del objeto PROCESS.

AL ingresar a la ruta localhost:8080/randoms se activa un CHILD_PROCESS del archivo calc.js que se ejecuta en un hilo separado. Hay un parametro por default sino se puede cambiar el parámetro localhost:8080/randoms?cant=PARAMETRONUMERICO. 

Las credenciales se movieron al archivo .env y se cargan mediante la librería dotenv.

El puerto de escucha del servidor por default es 8080 pero se puede pasar otro por argumentos. Esto se realizó con la librería minimist.

## Consideraciones generales

El proyecto corresponde al desafío de la clase 28 del curso de Back End en Coderhouse.

El nombre del usuario en los saludos NO esta hardcodeado sino que se obtiene a traves de socket desde una variable pusheada con req.session.user.

Los usuarios son almacenados en la base de datos ecommerce en Mongo Atlas, lo mismo las sesiones.

Las contraseñas se encryptan con la biblioteca bcrypt.

#### `Acerca de mi`

Mi nombre es Francisco González, tengo 42 años y en la actualidad me encuentro estudiando en Coder para ser desarrollador Full Stack. 

Me pueden contactar a través de mi email: [fmgarg@gmail.com](mailto:fmgarg@gmail.com) y/o por whatsapp: +549 11 5412 2848.