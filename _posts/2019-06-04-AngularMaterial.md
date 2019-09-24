---
layout: post
title: Angular + Material
description: Crea aplicaciones modernas y atractivas con Angular y Material Design.
image: images/blog/AngularMaterial/materialdesign.png
author: rckstr
preview-content: "Material Design es un lenguaje visual que sintetiza los principios clásicos de buen diseño con la
innovación de tecnología y ciencia. Material Design tiene como objetivo desarrollar un sistema que unifique la
experiencia de usuario a través de diferentes plataformas, dispositivos y métodos de entrada y al mismo tiempo, proveer
una base personalizable y flexible para la innovación."
---

<div class="post-content">
    <iframe allow="encrypted-media" allowtransparency="true" class="image left" frameborder="0" height="300"
        src="https://open.spotify.com/embed/user/dangobah/playlist/3uqfYUo6nQCSIvg4UG9Ww5" width="300"></iframe>

    <h2>Introducción</h2>

    <p>Material Design es un lenguaje visual que sintetiza los principios clásicos de buen diseño con la innovación de
        tecnología y ciencia. Material Design tiene como objetivo desarrollar un sistema que unifique la experiencia de
        usuario a través de diferentes plataformas, dispositivos y métodos de entrada y al mismo tiempo, proveer una
        base personalizable y flexible para la innovación.</p>

    <p>Angular Material es una librería de componentes para aplicaciones con Angular. Estos componentes nos permiten
        crear aplicaciones atractivas, consistentes y funcionales apegándose a los principios de Material Design.</p>

    <h2>Paso 1: Instalar Angular Material, Angular CDK y Angular Animations</h2>

    <blockquote> Si necesitas ayuda creando una aplicación de Angular, puedes ver los detalles en el post <i><a
                href="{% link _posts/2019-05-30-HolaAngular8.md %}" target="_blank">"¡Hola Angular 8!"</a></i>.
    </blockquote>

    <p>Puedes usar NPM o YARN para instalar los paquetes. Desde el folder de tu aplicación, en la terminal del sistema
        ejecuta la siguiente línea:</p>
    <h3>NPM</h3>
    <pre><code>npm install --save @angular/material @angular/cdk @angular/animations</code></pre>
    <h3>YARN</h3>
    <pre><code>yarn add @angular/material @angular/cdk @angular/animations</code></pre>

    <h2>Paso 2: Configurar las animaciones</h2>
    <p>Después de instalar el paquete de animaciones, importa el módulo <strong>BrowserAnimationsModule</strong> en tu
        aplicación para habilitar el soporte de animaciones.</p>

    <p>En el archivo app.module.ts de tu aplicación, agrega BrowserAnimationsModule a la lista de imports.</p>
    <div class="row">
        <div class="8u 12u$(small)">
            <pre><code>import {BrowserAnimationsModule} from '@angular/platform-browser/animations';

@NgModule({
    ...
    imports: [BrowserAnimationsModule],
    ...
})
export class AppModule { }</code></pre>
        </div>
        <div class="4u 12u$(small)"><span class="image fit"><a
                    href="/images/blog/AngularMaterial/01-ImportAnimations.png" target="_blank"><img
                        src="/images/blog/AngularMaterial/01-ImportAnimations.png" alt="" /></a></span></div>
    </div>

    <h2>Paso 3: Importar los componentes de Material UI</h2>
    <p>Los componentes de Material pueden importarse directamente en app.module.ts, sin embargo, como buena práctica,
        vamos a crear un módulo separado para importar los componentes. De esta manera, podemos tener nuestros módulos
        mejor organizados.</p>

    <ol>
        <li>En la consola, ejecuta la siguiente línea:</li>
        <pre><code>ng generate module material</code></pre>
        <li>Importa el nuevo módulo en app.module.ts</li>
        <div style="text-align: center"><span class="image 4u 12u$(small)"><a
                    href="/images/blog/AngularMaterial/02-CustomModule.png" target="_blank"><img
                        src="/images/blog/AngularMaterial/02-CustomModule.png" alt="" /></a></span></div>
        <li>Importa y exporta los componentes de Material en el módulo material.module.ts</li>
        <p>Para este ejemplo importaremos los siguientes componentes:</p>
        <div class="row">
            <div class="10u 12u$(small)">
                <ul>
                    <li>MatButtonModule</li>
                    <li>MatMenuModule</li>
                    <li>MatToolbarModule</li>
                    <li>MatIconModule</li>
                    <li>MatCardModule</li>
                    <li>MatSidenavModule</li>
                    <li>MatListModule</li>
                </ul>
                <p>Ya importados los componentes que vamos a utilizar, podemos llamarlos desde nuestra aplicación.</p>
            </div>
            <div class="2u 12u$(small)"><span class="image fit"><a
                        href="/images/blog/AngularMaterial/03-ImportComponents.png" target="_blank"><img
                            src="/images/blog/AngularMaterial/03-ImportComponents.png" alt="" /></a></span></div>
        </div>



    </ol>

    <h3>Estilos, íconos y soporte de gestos (opcional)</h3>
    <h4>Temas prefabricados</h4>
    <p>Podemos incluir estilos prefabricados en nuestra aplicación, para este ejemplo, agrega lo siguiente a styles.css.
    </p>
    <pre><code>@import "~@angular/material/prebuilt-themes/deeppurple-amber.css";</code></pre>

    <h4>Soporte de gestos</h4>
    <p>Algunos componentes como slide toggle, sliders y tooltips requieren HammerJS para soportar gestos. En este
        ejemplo no los estamos importando, pero en caso de que quieras usarlos puedes instalar HammerJS desde la consola
        ejecutando:</p>
    <pre><code>npm install --save hammerjs</code></pre>
    <p>Después de instalar hammerjs, debes importarlo en el archivo main.ts.</p>
    <pre><code>import 'hammerjs';</code></pre>
    <div style="text-align: center">
        <span class="image 4u 12u$(small)"><a href="/images/blog/AngularMaterial/04-hammerjs.png" target="_blank"><img
                    src="/images/blog/AngularMaterial/04-hammerjs.png" alt="" /></a></span>
    </div>

    <h4>Iconos</h4>
    <p>Para poder utilizar los iconos de Material UI, tenemos que cargar la fuente de Material Icons en el bloque
        <strong>head</strong> del archivo index.html.</p>
    <pre><code>&lt;link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet"&gt;</code></pre>
    <div style="text-align: center">
        <span class="image 4u 12u$(small)"><a href="/images/blog/AngularMaterial/05-Icons.png" target="_blank"><img
                    src="/images/blog/AngularMaterial/05-Icons.png" alt="" /></a></span>
    </div>

    <h2>Paso 4: Construir nuestra interfaz de usuario</h2>
    <p>En este paso crearemos un ejemplo de interfaz de usuario responsiva utilizando los componentes de Material UI
        importados en nuestra aplicación.</p>
    <p><strong>Reemplaza los contenidos de app.component.ts con el siguiente código:</strong></p>
    <pre><code>import { Component, ChangeDetectorRef, OnDestroy } from '@angular/core';
import { MediaMatcher } from '@angular/cdk/layout';

@Component({
    selector: 'app-root',
    templateUrl: './app.component.html',
    styleUrls: ['./app.component.css']
})
export class AppComponent implements OnDestroy {
    title = 'Angular + Material';
    mobileQuery: MediaQueryList;
    fillerNav = ['Opción 1', 'Opción 2', 'Opción 3', 'Opción 4', 'Opción 5', 'Opción 6', 'Opción 7'];

    fillerContent = Array.from({ length: 50 }, () => 'Interfaz gráfica usando componentes de Material UI. RCKSTR1 en GitHub. rckstr1.github.io');

    private _mobileQueryListener: () => void;

    constructor(changeDetectorRef: ChangeDetectorRef, media: MediaMatcher) {
    this.mobileQuery = media.matchMedia('(max-width: 600px)');
    this._mobileQueryListener = () => changeDetectorRef.detectChanges();
    this.mobileQuery.addListener(this._mobileQueryListener);
    }

    ngOnDestroy(): void {
    this.mobileQuery.removeListener(this._mobileQueryListener);
    }
}
        </code></pre>

    <p><strong>Reemplaza los contenidos de app.component.html con el siguiente código:</strong></p>
    <pre><code>&lt;div class="app-container" [class.app-is-mobile]="mobileQuery.matches"&gt;
    &lt;mat-toolbar color="primary" class="app-toolbar"&gt;
        &lt;button mat-icon-button (click)="snav.toggle()"&gt;
        &lt;mat-icon&gt;menu&lt;/mat-icon&gt;
        &lt;/button&gt;
        &lt;h1 class="app-app-name"&gt;&#123;&#123;title}}&lt;/h1&gt;
    &lt;/mat-toolbar&gt;
    
    &lt;mat-sidenav-container class="app-sidenav-container" [style.marginTop.px]="mobileQuery.matches ? 56 : 0"&gt;
        &lt;mat-sidenav #snav [mode]="mobileQuery.matches ? 'over' : 'side'" [fixedInViewport]="mobileQuery.matches"
        fixedTopGap="56"&gt;
        &lt;mat-nav-list&gt;
            &lt;a mat-list-item routerLink="." *ngFor="let nav of fillerNav"&gt;&#123;&#123;nav}}&lt;/a&gt;
        &lt;/mat-nav-list&gt;
        &lt;/mat-sidenav&gt;
    
        &lt;mat-sidenav-content&gt;
        &lt;router-outlet&gt;&lt;/router-outlet&gt;
        &lt;p *ngFor="let content of fillerContent"&gt;&#123;&#123;content}}&lt;/p&gt;
        &lt;/mat-sidenav-content&gt;
    &lt;/mat-sidenav-container&gt;
&lt;/div&gt;
      </code></pre>

    <p><strong>Reemplaza los contenidos de app.component.css con el siguiente código:</strong></p>
    <pre><code>.app-container {
    display: flex;
    flex-direction: column;
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
}

.app-is-mobile .app-toolbar {
    position: fixed;
    z-index: 2;
}

h1.app-app-name {
    margin-left: 8px;
}

.app-sidenav-container {
    flex: 1;
}

.app-is-mobile .app-sidenav-container {
    flex: 1 0 auto;
}
</code></pre>

    <h2>Paso 5: Ejecutar nuestra aplicación</h2>
    <p>En la consola integrada de Visual Studio Code, ejecuta la aplicación.</p>
    <pre><code>ng serve --open</code></pre>
    <p>Listo. Tenemos nuestra primera aplicación con Angular 8 y Material UI.</p>
    <div style="text-align: center">
        <span class="image 4u 12u$(small)"><a href="/images/blog/AngularMaterial/06-ItWorks.png" target="_blank"><img
                    src="/images/blog/AngularMaterial/06-ItWorks.png" alt="" /></a></span>
    </div>

    <h2>Conclusión</h2>
    <p>En este post vimos los pasos necesarios para utilizar componentes de Material Design en nuestras aplicaciones con
        Angular.</p>
    <p>Ahora estas listo para experimentar con Angular 8 y los componentes de Material UI.</p>
    <p>El código fuente completo de la aplicación de ejemplo puedes encontrarlo en GitHub, en <a
            href="https://github.com/RCKSTR1/AngularMaterial"
            target="_blank">https://github.com/RCKSTR1/AngularMaterial</a> o si prefieres, puedes clonar el repositorio
        directo en https://github.com/RCKSTR1/AngularMaterial.git</p>
    <p>Si tuviste algún problema o duda al seguir los pasos, o si tienes alguna pregunta acerca de este post, contáctame
        en Twitter, Facebook o LinkedIn.</p>

    <p>
        <strong>Es cuánto.</strong>
    </p>

    <h2>Fuentes</h2>
    <ul>
        <li>Documentación de Angular Material. <a href="https://material.angular.io/guide/getting-started"
                target="_blank">https://material.angular.io/guide/getting-started</a></li>
    </ul>

</div>
