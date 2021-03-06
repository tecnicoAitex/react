![logo_aitex.png](../../nodejs/images/logo_aitex_min.png "Logotipo de Aitex")

#Ejemplos en Visual Studio 2015

Adjuntamos varios ejemplos sobre la creación de una aplicación web SPA utilizando "React.js" junto con "Node.js", el gestor de paquetes "npm" y módulos de "Node.js".

> En la codificación hemos utilizado indistintamente **ECMAScript 5 y 6** tanto en ficheros JSX como con JavaScript. Al final mediante la tarea de transformación indicada en el fichero **["gulpfile.js"](../../npm/nodejs_packages/2_1_gulpfile.md)** quedará todo en JavaScript nativo.

+ **Tabla de rutas con** `react-router` **/ enrutamiento** web (`web.config`) para la navegación web. Consiguiendo una navegación como una SPA sin refrescar.  

> SPA (o single-page application): es una aplicación de página única o sitio web que cabe en una sola página con el propósito de dar una experiencia más fluida a los usuarios como una aplicación de escritorio. En una SPA todos los códigos de HTML, JavaScript y CSS se cargan de una vez.

+ **Comunicación entre componentes:** muestra de componentes, agrupados por grupo, ensayo y tareas. Uso de jQuery para los eventos que sucedan dentro del padre.  

+ **Uso de "Flux"**, pretendemos sustituir jQuery por flux y así no depender de una variable de entorno que recoge todos los eventos que suceden dentro del padre, para luego poder separar el código en distintos ficheros según los componentes que utilizamos.

##Instalación
Descargado el repositorio "react", nos situaremos dentro de la carpeta `visualStudio projects` y a su vez dentro de `[NombreProyecto]/src/[NombreProyecto]`.  

Utilizando el **cliente npm** y desde el "prompt de Node.js" instalaremos los módulos de Node.js con `> npm install`.  

Después desde el propio Visual Studio sólo tendremos que cargar el fichero con extensión `.sln` (Microsoft Visual Studio Solution) encontrado en el `[NombreProyecto]/` para ejecutarlo.

##Referencias
+ [Intergración de "npm" en Visual Studio Web](http://webtooling.visualstudio.com/package-managers/npm/).
+ [Soporte para "gulp" en Visual Studio Web](http://webtooling.visualstudio.com/task-runners/gulp/).