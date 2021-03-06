![logo_aitex_min.png](./images/logo_aitex_min.png "Logotipo de Aitex")

#React

Tenemos la opción de trabajar con la versión de **"react.js"** a partir del código proporcioando en su página oficial, pero nosotros lo tendremos instalado como módulo en nuestro proyecto a través del gestor de paquetes **"npm"** y registrado como dependencia de desarrollo en nuestro "package.json".

##Modificaciones entre versiones

Para poder comprobar ***qué versión*** disponemos, desde el prompt de node.js ejecutaremos el comando  
`> npm show react version`

###[Historial de versiones](:https://github.com/facebook/react/blob/master/CHANGELOG.md)

| Fecha | Versión |Detalle modificaciones realizadas|
|:--------:|:--------:|------|
|07/10/2015|**[0.14][enlaceReact14]**|División del paquete **"react"** en dos: **"react"** y **"react-dom"** para facilitar el renderizado. Por lo que facilita compartir componentes entre la versión web de "react" y el "react nativo".|
|29/03/2016|**[0.14.8][enlaceReact148]**|Solucionado el problema de la pérdida de memoria relacionada con la renderización en el lado del servidor.|
|07/04/2016|**[15.0][enlaceReact150]**|Modificaciones en la interacción con el DOM:|
|||El identificador utilizado por react.js **"data_reactid"** no aparecerá como atributo para cada nodo DOM cómo se hacía anteriormente. Para conseguir que el renderizado del DOM sea más ligero pero con el inconveniente de que no se sabrá si el sitio web está usando React.js o no.|
|||**"no hay más `<span\>` extra"**, en el renderizado de textos de bloque.Podemos renderizar textos plano  intercalados con nodos de comentario que se utilizan para demarcación.Esto nos da la misma capacidad de actualizar las piezas individuales de texto, sin crear nodos anidados adicionales. |
|||**Soporte de etiquetas SVG** gácias a que JSX y el método `React.createElement` trabaja con nombres de etiquetas.
|08/04/2016|**[15.0.1][enlaceReact1501]**|Nuevas interacciones con el DOM:|
| | |1) Método "React.__spread ha quedado obsoleto. |
| | |2) Bug fijado sobre la pérdida de la posición del cursor en los inputs.|

>**SVG:** Gráficos Vectoriales Redimensionables (o Scalable Vector Graphics) son una especificación para describir "gráficos vectoriales" bidimensionales, tanto estáticos como animados) en formato XML.

##Referencias

+ [Página oficial de "npm".](https://www.npmjs.com/)
+ [Página oficial de react.js.](https://facebook.github.io/react/index.html)
+ [React.js - blog oficial - versiones.](https://facebook.github.io/react/blog/)
+ [Lista completa de cambios en la versión 15.0.](https://facebook.github.io/react/blog/2016/04/07/react-v15.html)
+ [¿What is debbuging?](https://en.wikipedia.org/wiki/Debugging)
+ [Página oficial de react.js en npm.](https://www.npmjs.com/package/react)
+ [Vídeo: Curso React.js por OutKast.](https://www.youtube.com/watch?v=utAoFpE0tJs&index=1&list=PLEtcGQaT56ci0QiNycpR8mXWeaXcZn5yA)
+ [Vídeo: React.js en #programadorIO.](https://www.youtube.com/watch?v=ejMEwNVoOT0)
+ [Vídeo: Curso de React.js framework de facebook (latino)](https://www.youtube.com/watch?v=EDhvRw93Ui8&list=PLSuKjujFoGJ2XwyfRvH2nvJ44gvxBEPOd).
+ [Ejemplo de aplicación con React.js y ECMAScript 6](https://carlosazaustre.es/blog/ejemplo-de-aplicacion-con-react-js-en-ecmascript-6/)
+ [Ejemplo uso de React.js 0.14 con ECMAScript 6-7](http://blog.ricardofilipe.com/post/babel-react-es7-sample)
+ [Completa introducción a React.js (marzo 2016)](https://btholt.github.io/complete-intro-to-react/)
+ [Tutorial de React.js en Tutorials-Point](http://www.tutorialspoint.com/reactjs/index.htm)
+ [Diferencias entre React.createClass y React.Component](https://toddmotto.com/react-create-class-versus-component/)

<!-- Referencias  ocultas -->

[enlace1]:https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi
[enlace2]:http://facebook.github.io/react/blog/2015/09/02/new-react-developer-tools.html
[enlaceComponentesreact]:https://facebook.github.io/react/docs/glossary.html
[enlaceReact1501]:https://platzi.com/blog/react-15/
[enlaceEtiquetasHTML]:https://facebook.github.io/react/docs/jsx-in-depth.html
[enlaceAtributosetiquetas]:https://facebook.github.io/react/docs/tags-and-attributes.html
[enlaceDiferenciasreact]:https://toddmotto.com/react-create-class-versus-component/
[enlaceReact150]:https://facebook.github.io/react/blog/2016/04/07/react-v15.html
[enlaceReact148]:https://facebook.github.io/react/blog/2016/03/29/react-v0.14.8.html
[enlaceReact14]:https://facebook.github.io/react/blog/2015/10/07/react-v0.14.html
[enlaceECMA2105]:https://babeljs.io/blog/2015/06/07/react-on-es6-plus

