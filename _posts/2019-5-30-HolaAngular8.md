---
layout: post
title: Hola Angular 8!
description: Todo lo que necesitas para crear tu primera app con Angular 8.
image: assets/images/blog/Angular8/Angular8.png
---

<div class="post-content">
    <iframe allow="encrypted-media" allowtransparency="true" class="image left" frameborder="0" height="300"
        src="https://open.spotify.com/embed/user/dangobah/playlist/70rsMUaAcQ6ZJ4hZJfbYY1" width="300"></iframe>

    <h2>Introducción</h2>

    <p>Angular es un framework JavaScript muy popular, usado para desarrollar aplicaciones web, de escritorio y móviles.
        El desarrollo de aplicaciones con angular, involucra HTML, CSS y TypeScript que posteriormente es compilado a
        JavaScript.</p>
    <p>Usar Angular proporciona ventajas como:</p>
    <h3>1. Soporte para Single Page Applications (SPA)</h3>
    <p>SPAs son un tipo de aplicación web que cargan una sola página HTML, esta página es actualizada dinámicamente
        deacuerdo a la interacción del usuario con la aplicación sin tener que recargar la página completa.</p>

    <h3>2. Two-way data binding</h3>
    <p>Esta característica nos permite actualizar datos de manera automática en dos vías. Es decir, si nuestra fuente de
        datos cambia, la interfaz actualiza los datos, y viceversa.</p>

    <h3>3. Modularidad</h3>
    <p>Por diseño, el código de nuestra aplicación está organizado en módulos. Un módulo está relacionado a grupos de
        componentes, directivas, pipes y servicios.</p>
    <p>La modularidad también provee otros beneficios en Angular, como la habilidad de cargar solamente los componentes
        que necesitamos, conocida como Lazy-Loading.</p>

    <h3>4. Requiere escribir menos código</h3>
    <p>A todos nos gusta escribir menos código, que al mismo tiempo sea más efectivo. Angular soporta la arquitectura
        MVC (Model-View-Controller). Adaptarnos a este diseño nos permite escribir menos código y hace más fácil
        implementar buenas prácticas.</p>

    <h3>5. Interfaz de usuario declarativa</h3>
    <p>Nos permite definir la interfaz de usuario utilizando HTML de manera intuitiva y menos compleja que hacerlo con
        JavaScript. No tenemos que preocuparnos por el orden en que se cargan los componentes o el flujo del programa.
    </p>

    <p>En los últimos días, se liberó la versión 8 de Angular. En esta versión se mejoraron los tiempos de arranque de
        las aplicaciones y se incluyen nuevos API para interactuar con la CLI.</p>

    <h2>Prerrequisitos</h2>
    <p>Para sacar el mayor provecho de Angular necesitas conocer un poco de:</p>
    <ul>
        <li>HTML</li>
        <li>TypeScript</li>
        <li>CSS</li>
    </ul>

    <h2>Paso 1: Obtener las herramientas</h2>
    <p>Antes que nada, debemos contar con algunas herramientas instaladas en nuestra computadora. Como yo ya tenía las
        herramientas instaladas, creé una máquina virtual con Elementary OS, una distribución de Linux basada en Debian.
    </p>

    <h3>Node.js</h3>
    <p>Angular, Angular CLI y las aplicaciones con angular dependen de librerías disponibles como paquetes de NPM.</p>

    <h4>En Linux (Debian)</h4>
    <p>Los siguientes comandos funcionan en distribuciones de Linux basadas en Debian. Si usas otra distribución, En la
        terminal del sistema, ejecuta las siguientes líneas:</p>
    <pre><code>sudo curl -sL https://deb.nodesource.com/setup_12.x | sudo bash -
        
        sudo apt-get install -y nodejs</code></pre>

    <h4>En Windows o MacOS</h4>
    <ol>
        <span class="image right"><a href="/assets/images/blog/Angular8/01-NodeInstall.png" target="_blank"><img
                    src="/assets/images/blog/Angular8/01-NodeInstall.png" alt="" /></a></span>
        <li>Utilizando cualquier navegador, ve a www.nodejs.org y descarga la versión más reciente.</li>
        <li>Ejecuta el archivo descargado e instala Node.js.</li>
        <li>Antes de continuar al siguiente paso, comprobamos la instalación ejecutando la siguiente línea en la
            terminal:</li>
        <pre><code>npm -v</code></pre>
    </ol>

    <h3>Angular CLI</h3>
    <span class="image left"><a href="/assets/images/blog/Angular8/02-AngularCLIInstall.png" target="_blank"><img
                src="/assets/images/blog/Angular8/02-AngularCLIInstall.png" alt="" /></a></span>
    <p>La interfaz de línea de comandos o CLI, es una herramienta que usaremos para inicializar, desarrollar y mantener
        nuestras aplicaciones. Para instalar Angular CLI ejecuta la siguiente línea en la terminal (es posible que
        necesites permisos de root o administrador):</p>
    <pre><code>npm install -f @angular/cli</code></pre>

    <h3>Visual Studio Code (o cualquier otro editor de código)</h3>
    <span class="image left"><a href="/assets/images/blog/Angular8/03-VSCodeDownload.png" target="_blank"><img
                src="/assets/images/blog/Angular8/03-VSCodeDownload.png" alt="" /></a></span>
    <p>Este paso es opcional. Puedes usar el editor de código que más te guste. Visual Studio Code es mi favorito por la
        cantidad de extensiones disponibles y la terminal integrada. Si prefieres no usar Visual Studio Code puedes
        omitir esta parte.</p>
    <ol>
        <li>Utilizando cualquier navegador, ve a <a href="http://code.visualstudio.com"
                target="_blank">code.visualstudio.com</a></li>
        <li>Descarga el instalador</li>
        <p>Las opciones de descarga varían dependiendo de tu Sistema operativo. Si estas usando Linux, tienes la opción
            de
            descargar un archive .deb o .rpm, como estoy usando Elementary OS, descargué el archivo .deb.</p>
        <li>Instala la aplicación</li>
        <p>En mi caso, ya tenía preinstalado “Eddy” como manejador de paquetes, puedes instalar “Eddy” o cualquier otro
            manejador de paquetes dependiendo de la distribución de Linux que estés utilizando.</p>
        <p>Por otro lado, si estas en Windows o MacOS, no tienes de que preocuparte. Simplemente haz clic en el botón de
            descarga e instala Visual Studio Code como cualquier otra aplicación.</p>
    </ol>

    <h4>Extensiones recomendadas</h4>
    <p>Esta parte también es opcional. Aunque puedes optar por utilizar Visual Studio Code sin instalar extensiones,
        recomiendo usar estas extensiones porque agregan características al editor y nos puede hacer el trabajo más
        fácil a corto y mediano plazo.</p>
    <p>En la ventana de Visual Studio Code, haz clic en el último botón de la barra de actividades en el lado izquierdo
        para abrir la vista de extensiones.</p>

    <h5>Angular Language Service</h5>
    <span class="image left"><a href="/assets/images/blog/Angular8/04-AngularLanguageService.png" target="_blank"><img
                src="/assets/images/blog/Angular8/04-AngularLanguageService.png" alt="" /></a></span>
    <p>Esta extensión provee una mejor experiencia al trabajar con plantillas de Angular con características como listas
        de autocompletado, mensajes de diagnóstico AOT, opciones para ver la definición de variables u objetos.</p>
    <ol>
        <li>En el campo de búsqueda, escribe “Angular” (sin comillas).</li>
        <li>En la lista de resultados, selecciona la extensión “Angular Language Service” y después haz clic en
            “Install”</li>
    </ol>

    <h5>TSLint</h5>
    <span class="image left"><a href="/assets/images/blog/Angular8/05-TSLint.png" target="_blank"><img
                src="/assets/images/blog/Angular8/05-TSLint.png" alt="" /></a></span>
    <p>TSLint es una herramienta de análisis de código TypeScript que revisa legibilidad, facilidad de mantenimiento y
        errores de funcionalidad. Puede personalizarse con tus propias reglas, configuraciones y formateadores.</p>
    <ol>
        <li>En el campo de búsqueda, escribe “TSLint” (sin comillas).</li>
        <li>En la lista de resultados, selecciona la extensión “TSLint” de Microsoft y después haz clic en “Install”.
        </li>
    </ol>

    <h5>Visual Studio IntelliCode</h5>
    <span class="image left"><a href="/assets/images/blog/Angular8/06-IntelliCode.png" target="_blank"><img
                src="/assets/images/blog/Angular8/06-IntelliCode.png" alt="" /></a></span>
    <p>Esta extensión provee características asistidas por inteligencia artificial para varios lenguajes de programación
        basadas en contexto y machine learning.</p>
    <ol>
        <li>En el campo de búsqueda, escribe “IntelliCode” (sin comillas).</li>
        <li>En la lista de resultados, selecciona la extensión “Visual Studio IntelliCode” y después haz clic en
            “Install”.</li>
    </ol>

    <h4>Tipo de letra Fira Code (opcional)</h4>
    <span class="image left"><a href="/assets/images/blog/Angular8/12-FiraCode.png" target="_blank"><img
                src="/assets/images/blog/Angular8/12-FiraCode.png" alt="" /></a></span>
    <p>Fira Code es una extensión del tipo de letra Fira Mono, que contiene ligaduras para combinaciones multicaracter
        más comunes en programación. Esta característica ayuda a leer y entender código más rápidamente.</p>
    <ol>
        <li>Utilizando cualquier navegador, ve a <a href="http://github.com/tonsky/FiraCode"
                target="_blank">github.com/tonsky/FiraCode</a> y descarga los archivos del repositorio</li>
        <li>Instala el tipo de letra en tu computadora. En mi caso, instalé los archivos OpenType.</li>
    </ol>

    <h5>Configurar Fira Code en Visual Studio Code</h5>
    <span class="image left"><a href="/assets/images/blog/Angular8/07-FiraCodeSettings.png" target="_blank"><img
                src="/assets/images/blog/Angular8/07-FiraCodeSettings.png" alt="" /></a></span>
    <ol>
        <li>En la ventana de Visual Studio Code, presiona CTRL+, en Windows o Linux, o CMD+, en MacOS para abrir la
            pantalla de configuración.</li>
        <li>Una vez en la pantalla de configuración, haz clic en “Text Editor” y después en la opción “Font”.</li>
        <li>En el campo “Font Family” escribe “Fira Code” (sin comillas).</li>
        <li>Activa la casilla “Font Ligatures”</li>
    </ol>

    <h2>Paso 2: Crear nuestra primera app con Angular 8</h2>
    <span class="image left"><a href="/assets/images/blog/Angular8/08-CreateApp.png" target="_blank"><img
                src="/assets/images/blog/Angular8/08-CreateApp.png" alt="" /></a></span>
    <ol>
        <li>Desde la terminal, navega al folder en donde quieres crear tu aplicación. Yo decidí crear un folder nuevo
            para guardar mis apps.</li>
        <li>Una vez dentro del folder donde vas a crear tu app, escribe el siguiente comando:</li>
        <pre><code>
        ng new [nombre de tu app]
    </code></pre>
        <p>Angular CLI comenzará a crear tu aplicación y te presentará algunas opciones. Primero debes indicar si
            quieres agregar Angular Routing a tu app, por lo general vas a necesitarlo, selecciona la opción para
            agregarlo.</p>
        <p>Después, debes especificar el formato de estilos que va a usar la aplicación, para este caso selecciona CSS.
        </p>
        <p>Por último, indica si deseas compartir datos de uso con Google.</p>
        <p>Ahora verifica que se creó un folder con el nombre de tu nueva aplicación.</p>
    </ol>

    <h3>Ejecuta la aplicación</h3>
    <span class="image left"><a href="/assets/images/blog/Angular8/09-VSCodeOpenFolder.png" target="_blank"><img
                src="/assets/images/blog/Angular8/09-VSCodeOpenFolder.png" alt="" /></a></span>
    <p>A partir de este paso, comienza a utilizar la terminal integrada de Visual Studio Code, si prefieres otro editor
        de código, puedes seguir usando la terminal de tu sistema operativo para ejecutar comandos.</p>
    <ol>
        <li>Abre Visual Studio Code y haz clic en el primer icono de la barra de actividad para mostrar el explorador de
            archivos.</li>
        <li>Haz clic en el botón “Open Folder” y selecciona el folder de tu nueva aplicación para que Visual Studio Code
            muestre los contenidos de tu aplicación en el explorador de archivos.</li>
        <li>En la barra de menú, has clic en “View” y después en la opción “Terminal” para abrir la terminal integrada.
        </li>
        <li>Desde esta terminal puedes ejecutar tu aplicación escribiendo:</li>
        <span class="image left"><a href="/assets/images/blog/Angular8/10-VSCodeConsole.png" target="_blank"><img
                    src="/assets/images/blog/Angular8/10-VSCodeConsole.png" alt="" /></a></span>
        <pre><code>ng serve --open</code></pre>
        <p>La diferencia entre estas dos opciones es que si usas “-- open” la aplicación se abre automáticamente en tu
            navegador predeterminado, de otra manera, tendrías que ejecutar cualquier navegador y abrir
            http://localhost:4200.</p>
    </ol>

    <p>Mientras la aplicación se está ejecutando, la ventana del navegador se actualiza automáticamente después de
        guardar cualquier cambio en tu código.</p>
    <p>Para dejar de ejecutar tu aplicación, presiona CTRL+C en la terminal.</p>

    <h2>Conclusión</h2>
    <span class="image left"><a href="/assets/images/blog/Angular8/11-AppRuns.png" target="_blank"><img
                src="/assets/images/blog/Angular8/11-AppRuns.png" alt="" /></a></span>
    <p>Ahora ya tienes lo necesario para comenzar a escribir aplicaciones web, móviles o de escritorio con Angular 8.
    </p>
    <p>El código fuente completo de la aplicación de ejemplo puedes encontrarlo en GitHub, en
        <a href="https://github.com/RCKSTR1/Angular8RCSTR-APP"
            target="_blank">https://github.com/RCKSTR1/Angular8RCSTR-APP</a> o si prefieres, puedes clonar el
        repositorio directo en
        https://github.com/RCKSTR1/Angular8RCSTR-APP.git</p>
    <p>Si tuviste algún problema o duda al seguir los pasos, o si tienes alguna pregunta acerca de este post, contáctame
        en Twitter, Facebook o LinkedIn.</p>
    <p>
        <strong>Es cuánto.</strong>
    </p>

    <h2>Fuentes</h2>
    <ul>
        <li>Documentación de Angular. <a href="https://angular.io/docs" target="_blank">https://angular.io/docs</a></li>
        <li>Guía de setup de Angular. <a href="https://angular.io/guide/setup-local"
                target="_blank">https://angular.io/guide/setup-local</a></li>
    </ul>
</div>