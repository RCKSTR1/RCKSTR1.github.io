---
layout: post
title: '¿Qué es SOLID?'
description: 'Una breve (muuy breve) introducción a los 5 primeros principios del diseño orientado a objetos. Escribe
código limpio, fácil de mantener y extender.'
image: images/blog/SOLIDIntro/Banner-SolidIntro.jpg
author: rckstr
preview-content: 'Los principales lenguajes modernos de programación están influenciados por el paradigma orientado a
objetos. Pero, ¿qué es el diseño orientado a objetos? ¿Cuáles son sus ventajas y desventajas?'
---

<div class="post-content">
    <iframe allow="encrypted-media" allowtransparency="true" class="image left" frameborder="0" height="300"
        src="https://open.spotify.com/embed/playlist/2XqR85eq5Ae0lSgMXoIj84" width="300"></iframe>

    <h2>Introducción</h2>

    <p>
        Los principales lenguajes modernos de programación están influenciados por el paradigma orientado a objetos.
        Pero, ¿qué es el diseño orientado a objetos? ¿Cuáles son sus ventajas y desventajas?
    </p>
    <p>
        Comúnmente los desarrolladores no podemos contestar estas preguntas ni tenemos presentes los principios que
        constituyen la base de las disciplinas de las que derivaron nuestros lenguajes de programación.
    </p>
    <p>
        Podríamos afirmar que virtualmente todos los desarrolladores de software utilizan algún tipo de lenguaje
        orientado a objetos. Sin embargo, la mayoría, usamos estos lenguajes sin saber por qué, y sin saber cómo obtener
        el mayor beneficio del diseño orientado a objetos.
    </p>

    <h2>¿Qué es SOLID?</h2>

    <p>
        SOLID es un acrónimo para los primeros 5 de 11 principios del diseño orientado a objetos que exponen el manejo
        de dependencias, presentados por Robert C. Martin, también conocido como “Uncle Bob”.
    </p>

    <p>
        Los primeros 5 principios del diseño orientado a objetos se refieren al diseño de clases.
    </p>

    <div class="table-wrapper">
        <table>
            <tbody>
                <tr>
                    <td><strong>SINGLE RESPONSIBILITY PRINCIPLE</strong></td>
                    <td>Principio de responsabilidad única</td>
                    <td style="text-align: center;"><i>"Una clase debe tener una, y solo una, razón para cambiar"</i>
                    </td>
                </tr>
                <tr>
                    <td><strong>OPEN CLOSED PRINCIPLE</strong></td>
                    <td>Principio de abierto/cerrado</td>
                    <td style="text-align: center;"><i>"Debes ser capaz de extender el comportamiento de una clase sin
                            modificarla"</i></td>
                </tr>
                <tr>
                    <td><strong>LISKOV SUBSTITUTION PRINCIPLE</strong></td>
                    <td>Principio de sustitución de Liskov</td>
                    <td style="text-align: center;"><i>"Las clases derivadas deben ser sustituibles por sus clases
                            base"</i></td>
                </tr>
                <tr>
                    <td><strong>INTERFACE SEGREGATION PRINCIPLE</strong></td>
                    <td>Principio de segregación de interfaces</td>
                    <td style="text-align: center;"><i>"Diseña interfaces pequeñas que sean especificas del cliente"</i>
                    </td>
                </tr>
                <tr>
                    <td><strong>DEPENDENCY INVERSION PRINCIPLE</strong></td>
                    <td>Principio de inversión de dependencias</td>
                    <td style="text-align: center;"><i>"Depende de abstracciones, no de concreciones"</i></td>
                </tr>
            </tbody>
        </table>
    </div>

    <p>
        Apegarse a los principios SOLID, nos facilita a los desarrolladores escribir software fácil de mantener y
        extender.
        También nos ayuda a prevenir malas prácticas, a facilitar refactorización de código y también fomenta el
        desarrollo ágil
        de software.
    </p>
    <p>
        En los siguientes posts exploraremos cada uno de los 5 principios SOLID para presentar los beneficios que
        brindan y
        ayudar a identificar las áreas de oportunidad para implementarlos, así como tomar en cuenta el posible costo de
        aumentar
        complejidad a nuestro código contra el beneficio de tener código más apegado a estos principios.
    </p>
    <p>
        En resumen, aplicar los principios solid de manera adecuada nos permite tener código limpio, que se traduce en
        sistemas
        más flexibles y estables.
    </p>
    <p>
        ¡Hasta la próxima amigos!
    </p>

    <h2>Fuentes</h2>
    <ul>
        <li>Pluralsight. “SOLID Principles of Object Oriented Design”.
            <a href="https://app.pluralsight.com/library/courses/principles-oo-design/table-of-contents"
                target="_blank">https://app.pluralsight.com/library/courses/principles-oo-design/table-of-contents</a>
        </li>
        <li>butUncleBob.com. “The principles of OOD”.
            <a href="http://butunclebob.com/ArticleS.UncleBob.PrinciplesOfOod "
                target="_blank">http://butunclebob.com/ArticleS.UncleBob.PrinciplesOfOod</a>
        </li>
    </ul>

    <h2>Créditos</h2>
    <ul>
        <li>
            Elementos de diseño en el banner.
            <a href="http://www.freepik.com" target="_blank">Designed by rawpixel.com /
                Freepik</a>
        </li>

    </ul>
</div>
