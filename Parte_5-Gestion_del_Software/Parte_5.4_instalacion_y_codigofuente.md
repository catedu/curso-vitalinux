# Instalación de software y su código fuente

En éste apartado vamos a aprender a instalar software libre y hablaremos al final un poco sobre el código fuente (no te asustes).

## Instalación de Software

Una vez que sabemos qué aplicación queremos usar/probar, podremos instalarla si no lo estuviera usando algunos de los siguientes métodos

1. Vitalinux Play. Opción preferida para el entorno educativo
2. Synaptic. Completo pero algo complejo
3. Mediante migasfree
4. Centro de Software de Gnome.Menos recomendado
5. Manualmente mediante un paquete deb. Forma gráfica
6. Línea de comandos. Solo para expertos

> En la mayoría de los casos, deberemos hacer uso de una cuenta con permisos de administración para poder instalar/desinstalar software. En el caso de Vitalinux por ejemplo, la cuenta de docente y dga tienen por defecto permisos de administración.

### 1. Vitalinux Play

Con la finalidad de que los usuarios de Vitalinux (***docentes y estudiantes***) puedan localizar, proponer e instalar/desinstalar aplicaciones educativas, se ha creado la aplicación **Vitalinux Play**.  Ésta herramienta tiene catalogadas las apliaciones más afamadas dentro del mundo educativo.  En el caso de no encontrar en este almacén alguna aplicación de la cual se tiene constancia de que esta disponible para Linux, puede informarse de ello a los técnicos informáticos del proyecto Vitalinux a través del email **soportevitalinux@educa.aragon.es** con la finalidad de que la incluyan.

Entre sus características cabría destacar:

-  Permite al usuario instalar/desinstalar aplicaciones educativas sin necesidad de credenciales, con la finalidad de que sea un proceso lo más sencillo posible.
-  Las aplicaciones se encuentran categorizadas por niveles educativos: ***infantil, primaria, secundaria, bachillerato, etc**.  Esto permite filtrar las aplicaciones disponibles por el nivel educativo escriéndolo en el campo de búsqueda.
-  En la descripción de las aplicaciones se ha tratado de indicar la materia o área donde suelen ser utilizadas (***matemáticas, música, tecnología, etc.***), permitiendo de esta forma filtrarlas fácilmente escribiendo dicho patrón en el campo de búsqueda.

Para interactuar con **Vitalinux Play** simplemente debemos lanzarlo pulsando la combinación **CONTROL+ESPACIO** y escribir **Vitalinux Play**.

![Almacén de Software Educativo - Vitalinux Play](../img/parte5/vx-migasfree-play.png "Almacén de Software Educativo - Vitalinux Play")

### 2. Synaptic

Una de las aplicaciones más completa (gráfica) y usada en el mundo Linux para la gestión del software es **Synaptic**, aunque su aspecto visual no es tan amigable como el de otras aplicaciones equivalentes. Puede resultar algo "dura" para trabajar pero su eficiencia y robustez han hecho que sea una aplicación muy asentada y universalmente utilizada en muchas distribuciones Linux.

Entre sus características cabría destacar:

* Permite **actualizar la lista de software disponible en los repositorios** configurados en la máquina
* Permite **buscar** rápidamente, **instalar y desinstalar** aplicaciones
* Permite solventar problemas con **paquetes rotos** (paquetes que no se terminaron de instalar correctamente)

Para interactuar con **Synaptic** simplemente debemos lanzarlo pulsando la combinación **"CONTROL + ESPACIO"**' y tecleando **"Synaptic ..."** o también **"Instalar o Desinstalar Programas"**

![Synaptic](../img/parte5/synaptic.png "Gestor de Paquetes Synaptic")

La pantalla de Synaptic está dividida en 4 secciones. Las dos más importantes son la lista que incluye la sección de categorías (1) en el lado izquierdo y la de los paquetes (3) en el lado derecho. Al seleccionar un paquete de la lista se mostrará una descripción del mismo (4).

Para **instalar** un paquete seleccionaremos una categoría, pulsaremos con el botón derecho del ratón sobre el paquete deseado y seleccionaremos **Marcar para instalar o bien haremos doble clic** en el nombre del paquete. Marcaremos de esta forma todos los paquetes que deseesemos instalar en el sistema y pulsaremos sobre el botón **Aplicar** para que comience su instalación. Synaptic descargará él solo los paquetes necesarios desde los repositorios

También es posible emplear el botón **Buscar** para encontrar los paquetes que deseemos instalar. Al pulsar sobre este botón podremos realizar búsquedas de programas mediante su nombre o descripción. Una vez localizado el programa que deseamos instalar hacemos doble clic sobre él para instalarlo. Si queremos eliminar un programa bastará con que pulsemos con el botón derecho encima de éste y **seleccionemos Eliminar o Eliminar por completo**.

En todos los casos, los cambios surtirán efecto una vez que hagamos clic sobre el botón de **Aplicar**.

### 3. Mediante migasfree

Como ya se ha dicho en varias ocasiones, una caracterísitica que vamos a encontrar en **Vitalinux** y que le diferencia del resto de distribuciones Linux actuales, es que incorpora un **cliente Migasfree** que gestiona de forma centralizada y personlizada cada centro educativo.  En concreto, este cliente Migasfree garantiza que cada vez que arranca Vitalinux EDU DGA y tras iniciar sesión, se establece una comunicación con el servidor [Migasfree del programa de **Software Libre** de la DGA](http://migasfree.edcuca.aragon.es), y a través de dicha comunicación, Vitalinux deja en manos de **Migasfree** la configuración del equipo en cuanto a personalización y software: Migasfree provocará en el equipo Vitalinux todo aquello que se le haya encomendado previamente por el propio centro, y en concreto:

* Qué aplicaciones deben instalarse (y si no lo están, lo hará de forma automática)
* Qué aplicaciones se tienen que desinstalar (si las encuentra instaladas).
* Actualizar las aplicaciones instaladas y del sistema
* Instalación de periféricos: Impresoras, PDIs, Webcams....
* Además realiza otras acciones como:
  * Configurar el entorno del escritorio
  * Configurar las aplicaciones: navegadores, libreoffice, arduino...
  * Limpieza del equipo
  * Gestión de usuarios

En definitiva, **cualquier aspecto que se pueda configurar vía software, se puede programar y automatizar para todos (o parte) de los eqiupos del centro**

¿Y cómo sabe qué tiene  que hacer en cada equipo, si son muchos centros y cada uno usa un software diferente? A grandes rasgos, **Migasfree** tiene identificado al equipo Vitalinux en base a un identificador unívoco llamado **CID** y a un conjunto de **Etiquetas Migasfree** que se le pueden asignar. Cada centro puede personalizar así sus sistemas, y recibe la asesoría correspondiente entrando en el **programa de Asesoramiento del Proyecto Vitalinux**.

### 4. Centro de Software de Gnome

**Vitalinux** es una distribución basada en la versión ligera de Ubuntu, la cual dispone de su propio centro de software '''Software''' que permite al usuario instalar y desinstalar aplicaciones de una forma muy gráfica y convencional, al estilo que estamos acostumbrados de un Store actual del móvil, pudiendo filtrar la búsqueda de una manera categorizada: '''Educación, Ofimática, Internet''', etc.

> Atención: es posible que NO encontremos todo el software disponible (por problemas de indexación) o que incluso la aplicación presente "algunos bloqueos". Se aconseja usar alguno de los métodos anteriores.

Para interactuar con '''El Centro de Software''' simplemente debemos lanzarlo pulsando la combinación mágia **CONTROL + ESPACIO** y tecleando **Software**. Si no disponemos del lanzador, lo podremos encontrar en el menú o con el nombre de Centro de Software.

![Centro de Software 1](../img/parte5/softwareapp0.png "Centro de Software en VX-2.x")
![Centro de Software 1](../img/parte5/softwareapp0-vx-3.png "Centro de Software en VX-3.x")

### 5. Forma manual

De forma manual, dependerá de como nos faciliten el software:

* O bien es un paquete que debemos "instalar" antes de poder usar. Como lo que hemos visto hasta ahora, pero de forma manual. Serán archivos **.deb** que deberemos descargar y ejecutar para instalar.
* Es una aplicación que tiene todo los binarios y librerías ya compilados y empaquetados, de forma que se puede lanzar directamente. En éste caso, solo debemos marcarlos para ejectuar y lanzarlo. Es lo que se conoce comunmente como software portable. El más común actualmente es en formato **AppImage**

> Si optamos por la fórmula manual, debemos ser cuidadosos y saber de dónde estamos descagando el software para garantizar la seguridad e integridad de nuestro equipo y sobre todo, respetar las licencias de uso para respetar la legalidad del uso de la misma

Veamos un ejemplo de cada:

#### 5.1 Paquetes deb

![Descarga Software](../img/parte5/downloaddeb.png "Descargando Software")

1. Buscamos el software a instalar. Encontramos el fichero a descargar. El nombre del archivo (nootka_2.0.2_amd64.deb) nos está indicando la versión (2.0.2) y en éste caso la arquitectura (64 bits). Deberemos descargar éste si nuestra arquitectura del sistema operativo es 64 bits (lo mas común a día de hoy) o buscar el de 32 (en éste caso no hay posibilidad). También podemos encontrar el final con un all en lugar de amd64, lo que indica que sirve para cualquier arquitectura

> Observar que el software tiene versiones para múltiples arquitecturas...como debe ser :-)

![Instalando Software](../img/parte5/installdeb.png "Instalando Software en Vitalinux 2.x")
![Instalando Software](../img/parte5/installdeb-vx-3.png "Instalando Software en Vitalinux 3.x")

2. Una vez descargado, podemos instalarlo simplemente haciendo doble click sobre el paquete. Al instalarlo nos puede saltar una advertencia indicando que dicho paquete ya está en un "canal de distribución" (como es el caso), es decir, que se encuentra disponible en los repositorios...por si queremos instalarlo de ésta forma y asegurar que viene firmado y estable a la versión de distribución que tenemos (por ejemplo, las posibles librerías que necesite estarán en la versión esperada).

Es posible también encontrar url's en páginas web que directamente apuntan al paquete deb mediante un protocolo para instalar, siempre que sigamos el link desde un equipo Linux. Lo podremos probar en el [listado de aplicaciones](./Parte_5.3_listado_aplicaciones.md) mostrado.

#### 5.2 Ficheros AppImage

En el caso de ficheros AppImage, procederemos a descargarlo igualmente. En éste ejemplo, el nombre sería nootka-1.7.3-beta3-b3917-x86_64.AppImage, indicando que es para una arquitectura de 64 bits

Ésta forma de distribución, no requiere de ninunga instalación para ejecutarse, pero:

* Es muy **cómodo** ya que no requiere instalación, dependencias de librerías con versiones que no tenemos
* No requiere permisos **privilegiados** para poder usarlo (dependiendo de las acciones que quiera realizar). Los paquetes deb requieren permisos de superusuario para ser instalados.
* **No** se mantedrá **actualizado**
* Es posible que le cueste arrancar algo más, ya que contiene todas las librerías y programas adicionales que necesite
* Deberemos añadir el **lanzador** que queramos para poder tenerlo accesible de forma cómoda (menú, escritorio, lanzador de aplicaciones...)

![AppImage en vx](../img/parte5/appimage_vx.png "Lanzando AppImage en Vitalinux")

> En vitalinux se ha faclitado su ejecución de forma que no es necesario dar permisos de ejecución a los archivos AppImage, pero si queremos darlos solo tenemos que ir a las propiedes del archivo y marcarlo como ejecutable:

![Permisos de ejecución](../img/parte5/appimage_exe.png "Permisos de ejecución sobre appimage en Vitalinux 2.x")
![Permisos de ejecución](../img/parte5/appimage_exe-vx-3x.png "Permisos de ejecución sobre appimage en Vitalinux 3.x")


Hay otras tecnologías de distribución de softare como pueden ser Snap y Flatpak, que se están abriendo camino. Puedes [consultar más información aquí por ejemplo sobre snap aquí](https://itsfoss.com/use-snap-packages-ubuntu-16-04/)

### 6. Línea de comandos. Opción avanzada que excede a los contenidos de éste curso.

Mediante la línea de comandos, podemos instalar software, desinstalar, comprobar, buscar...usando los repositorios que tenemos configurados.
Antes ya hemos visto algo con obs-studio. Veamos un ejemplo mas completo de acciones que puedes hacer

Actualizar la lista de paquetes disponibles en el repositorio

```bash
sudo apt-get update
```

Actualizar todos los paquetes instalados en el equipo

```bash	
sudo apt-get upgrade
```

Instalar un paquetes:

```bash	
sudo apt-get install nombre_del_paquete
```

Desinstalar paquetes:

```bash	
sudo apt-get remove nombre-del-paquete
```

Desinstalar un paquete y sus archivos de configuración asociados:

```bash	
sudo apt-get remove --purge nombre-del-paquete
```

## Código fuente. Opción avanzada que excede a los contenidos de éste curso.

Para finalizar éste apartado, debemos destacar un aspecto importante del software libre: es **código abierto**, y por tanto podemos consultar su código fuente, modificarlo...

> Recordar que OpenSource no siempre es software libre. Podemos tener programas de código abierto (opensource) con licencias restrictivas de uso.

Podemos descargar el código fuente usando el siguiente comando, siempre que **tengamos en los repos** marcado que queremos tener disponible además del software (deb) el código fuente (**deb-src**)

```bash
apt source nombre_paquete
```

Pero una forma más interensante para poder consultar el código es ir a las plataformas que se usan para la gestión de proyectos de software. La mayoría usa un sistema de control de versiones llamado git. Como servidores, hay muchos, pero los más usadas son:

* [Launchpad](https://launchpad.net/). Por ejemplo del paquete [Cheese](https://code.launchpad.net/ubuntu/+source/cheese)
* [Github](https://github.com/). Aquí encontramos por ejemplo el código del software comentado antes [obs-studio](https://github.com/obsproject/obs-studio)
* [Gitlab](https://gitlab.com/inkscape/inkscape). Por ejemplo el código de [Inkspcape](https://gitlab.com/inkscape/inkscape)

Está fuera del alcance de éste curso manejar éstas herramientas de control de código. Conocer de algunos proyectos/aplicaciones el código fuente, o por lo menos seguir su desarrollo nos va a permitir involucrarnos mas en dicho programa, estar atento a las novedades, poder reportar incidencias o incluso colaborar en su mejora. Dependiendo de la edad de los estudiantes y su compromiso puede ser intereante incluso hacerles participes a los mismos. Por ejemplo...podríamos ayudar a traducir un software al castellano como han hecho algunos COFO's en sus centros...estaríamos fomentando las habilidades lingüisticas y tecnológicas.

El **código fuente de los programas que se escriben para Vitalinux**, lo podemos encontrar en su [propio servidor de gitlab](https://gitlab.vitalinux.educa.aragon.es).

Fuentes: 
* https://itsfoss.com/remove-install-software-ubuntu/
* https://ubunlog.com/