![logo_aitex.png](images/logo_aitex_min.png "Logotipo de Aitex")
#¿Qué es Node.js?

Inicialmente es una librería y un entorno de ejecución de entrada y salida, dirigida por eventos, asíncrona que se ejecuta con el intérprete de JavaScript "V8" creado por Google. Además fue la primera librería basasda en JavaScript y con un gran rendimiento.

En pocas palabras, **[Node.js][webNode]** es un runtime multiplataforma de JavaScript, que ha cogido mucha fuerza gracias a su [versatilidad] y al auge de JavaScript. El motivo de nuestro interés en él, se centra en el hecho de haber múltiples utilidades o scripts hechos (a partir de ahora los llamaremos módulos) que nos ayudarán a poder trabajar y automatizar tareas, pudiendo crear aplicaciones orientadas a las redes de comunicación, interactuar con componentes del sistema operativo a través de funciones que cumplen con el estándar **POSIX**.

> **POSIX**, norma escrita por la **IEEE** _(Institute of Electrical and Electronics Engineers)_, definiendo una interfaz estándar del sistema operativo y el entorno, incluyeno un intérprete de comandos (o "shell") así como programas de utilidades comunes para apoyar la portabilidad de las aplicaciones a nivel de código fuente *(fuente: Wikipedia)*.

Define las interfaces y el entorno, utilidades comunes que un sistema operativo puede soportar y hacerlos disponibles para que el código fuente de un programa sea compilable y ejecutable.

Además de ejecutar scripts, posee un gestor de paquetes denominado [npm] que lo usaremos reiteradamente a lo largo de nuestro proceso de desarrollo.

Durante la edición del presente documento, la versión con la que trabajaremos será la **4.4.4 [LTS][enLTS]** que es la que se recomienda en la página oficial.

>**LTS:** son las abreviaturas de *"Long Term Support"* (soporte a largo plazo) utilizadas para indicar que una versión o edición de un software tendrá soporte (actualizaciones, correción de errores) durante un período de tiempo *(fuente: Wikipedia).*

Podemos acceder a la amplia documentación de la [API 4.4.4 LTS][docApiNode].

##Características de Node.js
Para conocer las características que tiene Node.js por defecto (sin requerir indicadores de tiempo de ejecución) clicar [aquí][linkECMAScript].  


##ECMAScript en Node.js
Recordemos que Node.js está contruido sobre la versión del motor de renderización de Chrome V8. Para estar al día con las últimas actualizaciones de este motor, se debe asegurar que las nuevas características de la especificación de **"JavaScript ECMA-262"** es presentada a los desarrolladores de Node.js en tiempo y forma, así como las contínuas mejoras de rendimiento y estabilidad.

>**ECMAScript:** es una especificación de lenguaje de programación. Define un lenguaje de tipos dinámicos inspirado en Java y otros lenguajes del estilo de "C". Soporta algunas características de la programación orientada a objetos mediante objetos basados en prototipos y pseudoclases. Los navegadores web incluyen una implementación del ECMAScript.  

###Uso que le daremos a Node.js
En un primer momento lo utilizaremos como entorno de desarrollo de nuestra aplicación, es decir, lo utilizaremos como runtime para “lanzar” las diferentes tareas que necesitaremos ejecutar en nuestro proyecto desarrollado en “Visual Studio Community 2015”, siendo éstas:

+ **Servidor web**, aparte del IIS Expres (Internet Information Services v10) es posible lanzar nuestro servidor para que a medida que vamos realizando cambios tanto en los ficheros JavaScript como en el "html".  

+ **Minificador de código**, todos los ficheros “.jsx”, “.js”, “.json” podremos convertirlos a JavaScript nativo mediante un único fichero js, comprensible por el navegador, ofreciendo la posibilidad de que durante el proceso de desarrollo / producción sea posible la modificación de cualquier fichero mientras se encuentre dando servicio a los usuarios.  

+ **Notificador de cambios**,esto implica que cualquier cambio que se realice en el código de los ficheros indicados en el “gulpfile.js” (tareas que se ejecutarán) a su vez serán notificadas al “minificador” para que se actualice el fichero único “index.js”.

Por tanto será utilizado como servidor de aplicaciones.

Para producción dispondremos de un servidor con Internet Information Services (IIS) donde alojaremos la página, usaremos Reactjs como framework para el front-end y mediante los paquetes de Node que tendremos instalados previamente

##Arquitecturas utilizadas
###Arquitectura de desarrollo
![arquitectura_desarrollo.png](images/arquitectura_desarrollo_visual.png)

###Arquitectura de producción
![arquitectura_produccion.png](images/arquitectura_produccion_visual.png)

##Referencias
+ [Página oficial npm](https://docs.npmjs.com/getting-started/what-is-npm).
+ [Página oficial Node.js](https://nodejs.org/en/).
+ [Node.js en GitHub](https://github.com/nodejs/nodejs.org).
+ [ECMAScript2015 (ES6) in Node.js](https://nodejs.org/en/docs/es6/).
+ [Standar ECMA-262 - *ECMAScript 2015 Language Specification*](http://www.ecma-international.org/publications/standards/Ecma-262.htm).
+ [Soporte a largo plazo - LTS Node.js](https://github.com/nodejs/LTS#lts_schedule).
+ [Documentación Node.js 4.4.0 LTS](https://nodejs.org/dist/latest-v4.x/docs/api/).
+ [A Case-by-Case Tutorial Node.js](https://www.toptal.com/nodejs/why-the-hell-would-i-use-node-js).
+ [Tutorial Node.js](http://www.tutorialspoint.com/nodejs).

<!--  Referencias y enlaces a las fuentes -->
[webNode]:https://nodejs.org/en/
[versatilidad]:http://www.nodehispano.com/2011/11/que-es-node-js-nodejs/
[npm]:https://www.npmjs.com/
[enLTS]:https://github.com/nodejs/LTS#lts_schedule
[linkECMAScript]:https://nodejs.org/en/docs/es6/
[docApiNode]:https://nodejs.org/dist/latest-v4.x/docs/api/
[bowerVSnpm]:http://stackoverflow.com/questions/18641899/what-is-the-difference-between-bower-and-npm
[webBower]:https://www.npmjs.com/package/bower
