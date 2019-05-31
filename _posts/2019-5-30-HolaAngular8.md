---
layout: post
title: Hola Angular 8!
description: Todo lo que necesitas para crear tu primera app con Angular 8.
image: assets/images/blog/HelloWorld/hello.png
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
    <pre><code>
        sudo curl -sL https://deb.nodesource.com/setup_12.x | sudo bash -
        
        sudo apt-get install -y nodejs
    </code></pre>

    <h4>En Windows o MacOS</h4>
    <ol>
        <li>Utilizando cualquier navegador, ve a www.nodejs.org y descarga la versión más reciente.</li>
        <li>Ejecuta el archivo descargado e instala Node.js.</li>
        <li>Antes de continuar al siguiente paso, comprobamos la instalación ejecutando la siguiente línea en la
            terminal:</li>
        <pre><code>
            npm -v
        </code></pre>
    </ol>

    <h3>Angular CLI</h3>
    <p>La interfaz de línea de comandos o CLI, es una herramienta que usaremos para inicializar, desarrollar y mantener
        nuestras aplicaciones. Para instalar Angular CLI ejecuta la siguiente línea en la terminal (es posible que
        necesites permisos de root o administrador):</p>
    <pre><code>
        npm install -f @angular/cli
    </code></pre>

    <h3>Visual Studio Code (o cualquier otro editor de código)</h3>
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
    <p>Esta extensión provee una mejor experiencia al trabajar con plantillas de Angular con características como listas
        de autocompletado, mensajes de diagnóstico AOT, opciones para ver la definición de variables u objetos.</p>
    <ol>
        <li>En el campo de búsqueda, escribe “Angular” (sin comillas).</li>
        <li>En la lista de resultados, selecciona la extensión “Angular Language Service” y después haz clic en
            “Install”</li>
    </ol>







    -contenido nuevo-
    <p>Mi nombre es Adrian, soy de Tijuana, Baja California, “la ciudad mas peligrosa del mundo” dicen algunos. Pero a
        mi no me ha traído mas que cosas buenas. Aquí nací y crecí. Es una ciudad llena de oportunidades, que tiene
        oídos para las buenas ideas, sin importar de donde vengan.</p>

    <p>Soy de los afortunados que tuvieron la oportunidad de convertirse en lo que querían ser desde niños. Yo no quería
        ser ni bombero ni astronauta, sino que esperaba los días de escuela en que nos llevaban al laboratorio de
        computación, a dibujar en Paint con Windows 95, o jugar algún juego en la computadora.</p>

    <p>Un día, cuando tenía 8 años, en lugar de abrir Word, o Paint, llegamos al laboratorio y en las pantallas había
        una ventana desconocida, era el IDE de LOGO. La profesora Vicky nos contó una historia acerca de una tortuga, y
        escribió en el pizarrón 4 “palabras mágicas” necesarias para mover a la tortuga. Ese fue el día que escribí mi
        primera línea de código, Ahora podía hacer dibujos escribiendo líneas de código y ver como se iban dibujando en
        la pantalla. Y ya. desde entonces lo que yo quería hacer era tener una computadora y escribir código para hacer
        dibujos y regalárselos a todo el mundo.</p>

    <p style="text-align:center !important;">
        <span class="image"><img src="/assets/images/blog/HelloWorld/logo_mit.png"></span>
        <br><i>LOGO. Existe una version moderna del ide online:
            <a href="https://turtleacademy.com/" target="_blank">https://turtleacademy.com/</a>
        </i>
    </p>

    <p>Pasaron algunos años, y ahora estaba en la universidad. Con las mismas ganas de escribir código en una
        computadora, pero ahora acompañado de personas que igual que yo, habían decidido en algún punto de sus vidas,
        escribir código, o hacer redes, o diseñar microprocesadores.</p>

    <p>Fast forward al 2019, tengo 31 años, soy desarrollador de software, desde 2007 especializado en tecnologías de
        Microsoft, aunque últimamente incursionando en la realidad aumentada. Hace un año, recibí la invitación de
        LinkedIn para el programa de Career Advisors, me pareció una manera interesante de contribuir a otros con mi
        grano de arena. Sin embargo, hace tiempo que me vengo dando cuenta de los efectos que la barrera del lenguaje
        tiene en el desarrollo de software, de la desventaja que puede representar para las personas que no pueden
        adquirir conocimiento porque no han tenido el tiempo o la oportunidad de aprender inglés.</p>

    <p>Este blog es mi manera de decir gracias a todos de los que he aprendido algo y que de alguna manera me ayudaron a
        convertirme en lo que siempre quise desde que era un niño.</p>

    <p>Sinceramente, espero alguno de estos días poder escribir algo que le ayude a alguien a escribir su primera línea
        de código.</p>

    <p>
        <strong>Es cuánto.</strong>
    </p>
</div>