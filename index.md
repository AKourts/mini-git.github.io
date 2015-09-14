---
layout: default
---

Desarrollo colaborativo y despliegue de aplicaciones: `git`
----------------------------------------------------------

[git](https://git-scm.com) es un programa distribuido de gestión de
control de versiones. Se diseñó originalmente para la gestión de
fuentes del núcleo de Linux, pero hoy en día se usa también de forma
extensiva para despliegue de aplicaciones.

Un sistema de control de versiones permite saber a quién corresponde
cada cambio en un fuente y revertir tales cambios si hay algún
problema en los mismos. También permite trabajar simultáneamente con
diferentes versiones y, eventualmente, fusionarlas conservando los
cambios en las mismas. El hecho de que se puedan revertir los cambios
y también integrarse en un flujo de desarrollo (que incluya
integración continua, por ejemplo) es la clave de su popularidad en el
despliegue de aplicaciones en la nube.


>Esta
[presentación sobre Git y su uso en GitHub](https://www.slideshare.net/jjmerelo/introduccin-al-uso-git-y-github-para-trabajo-colaborativo)
>está más enfocada al uso general, pero las órdenes básicas que se usan
>para desplegar en la nube se tratan también. El [Zen de Git de Psicobyte](http://www.psicobyte.com/descargas/ZenDeGit.pdf) presenta de forma amena todos los conceptos del programa.

El ciclo básico de uso de `git` consiste, tras la clonación, en hacer
`pull` - modificar - `commit` - `push`. Este último sincroniza la
versión local con la versión remota. Se pueden hacer varios `commits`
antes de hacer `push`; todos los cambios se subirán al hacerlo. En
realidad el programa es mucho más complejo y admite múltiples cambios,
pero a este nivel es suficiente con conocer esto. Es decir:

    #Descarga el repo
	git clone git@github.com:mini-git/mini-git.github.io.git

	#O actualízalo
	git pull

	#O en caso de tener varios repositorios origen
	git pull origin master
	
	#Añade un fichero al repo o al commit
	git add _posts/un_post.md

	#Mensaje del commit y añade todos los ficheros modificados
	git commit -am "Añade un post"

	#Sincroniza con el repositorio remoto
	git push


>Este [vídeo de 14 minutos](https://www.youtube.com/watch?v=ygbWIJWe29Y)
>sirve como introducción al uso de `git`.

## Mini tutorial y chuleta

En [El Baúl del programador](http://elbauldelprogramador.com/mini-tutorial-y-chuleta-de-comandos-git/), con una lista extensa de comandos.

## Libro

[Aprende git... Y de camino, GitHub](https://www.amazon.es/dp/B00K515GL2?tag=atalaya-21&camp=3634&creative=24822&linkCode=as4&creativeASIN=B00K515GL2&adid=19NA41Y1VM1XXMDBM6N9&), por un euro, es una introducción bastante completa, hecha por [Psicobyte](http://psicobyte.github.com) y un servidor.

## Autor

JJ Merelo ([Twitter](http://twitter.com/jjmerelo)/[GitHub](http://github.com/JJ)/[G+](https://plus.google.com/+JJMerelo/posts?rel=author)).

![JJ Merelo](http://1.gravatar.com/avatar/dd366bcdcf85991fa8af1b6d11d3ad49)

### Licencia

[CC-BY-SA](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)

<div class="github-fork-ribbon-wrapper right fixed" style="width: 150px;height: 150px;position: fixed;overflow: hidden;top: 0;z-index: 9999;pointer-events: none;right: 0;"><div class="github-fork-ribbon" style="position: absolute;padding: 2px 0;background-color: #333;background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.15));-webkit-box-shadow: 0 2px 3px 0 rgba(0, 0, 0, 0.5);-moz-box-shadow: 0 2px 3px 0 rgba(0, 0, 0, 0.5);box-shadow: 0 2px 3px 0 rgba(0, 0, 0, 0.5);z-index: 9999;pointer-events: auto;top: 42px;right: -43px;-webkit-transform: rotate(45deg);-moz-transform: rotate(45deg);-ms-transform: rotate(45deg);-o-transform: rotate(45deg);transform: rotate(45deg);"><a href="https://github.com/mini-git/mini-git.github.io" style="font: 700 13px &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif;color: #fff;text-decoration: none;text-shadow: 0 -1px rgba(0, 0, 0, 0.5);text-align: center;width: 200px;line-height: 20px;display: inline-block;padding: 2px 0;border-width: 1px 0;border-style: dotted;border-color: rgba(255, 255, 255, 0.7);">Fork me on GitHub</a></div></div>
