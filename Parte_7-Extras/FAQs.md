#  Preguntas Frecuentes - FAQs
## Contenido

<li class="toclevel-1">[1 ¿Sin acceso gráfico? Como resolver problemas cuando no tenemos acceso al entorno grafico](#.C2.BFSin_acceso_gr.C3.A1fico.3F_Como_resolver_problemas_cuando_no_tenemos_acceso_al_entorno_grafico)
<ul>
- [1.1 Introducción](#Introducci.C3.B3n)
- [1.2 Síntomas](#S.C3.ADntomas)
<li class="toclevel-2">[1.3 Propuesta de solución](#Propuesta_de_soluci.C3.B3n)
<ul>
- [1.3.1 Abrir una sesión por consola](#Abrir_una_sesi.C3.B3n_por_consola)
- [1.3.2 Comprobar si tenemos conectividad](#Comprobar_si_tenemos_conectividad)
- [1.3.3 Ejecución de comandos que intentan resolver configuraciones o instalaciones que se han quedado a mitad](#Ejecuci.C3.B3n_de_comandos_que_intentan_resolver_configuraciones_o_instalaciones_que_se_han_quedado_a_mitad)
- [1.3.4 Dejar el sistema actualizado](#Dejar_el_sistema_actualizado)

- [2.1 Burlington](#Burlington)
<li class="toclevel-2">[2.2 Oxford](#Oxford)
<ul>
- [2.2.1 Como instalar un libro de Oxford](#Como_instalar_un_libro_de_Oxford)

- [7.1 Servicio de Congelación en Vitalinux](#Servicio_de_Congelaci.C3.B3n_en_Vitalinux)
- [7.2 ¿Cómo puedo hacer prácticas de instalación de software sin que persistan en Vitalinux?](#.C2.BFC.C3.B3mo_puedo_hacer_pr.C3.A1cticas_de_instalaci.C3.B3n_de_software_sin_que_persistan_en_Vitalinux.3F)

- [13.1 Idiomas](#Idiomas)

- [16.1 Hardware](#Hardware)
- [16.2 Rendimiento](#Rendimiento)
- [16.3 Aplicaciones](#Aplicaciones)
- [16.4 Resumiendo](#Resumiendo)

- [17.1 ¿Lubuntu es ligero por el software preinstalado y su Entorno de Escritorio?](#.C2.BFLubuntu_es_ligero_por_el_software_preinstalado_y_su_Entorno_de_Escritorio.3F)
- [17.2 ¿Qué perderíamos y ganaríamos en el caso de que Vitalinux se basara en otra distribución de Ubuntu?](#.C2.BFQu.C3.A9_perder.C3.ADamos_y_ganar.C3.ADamos_en_el_caso_de_que_Vitalinux_se_basara_en_otra_distribuci.C3.B3n_de_Ubuntu.3F)
- [17.3 Si tenemos ordenadores potentes en casa ... ¿nos merece la pena modificar el Entorno de Escritorio de Vitalinux/Lubuntu?](#Si_tenemos_ordenadores_potentes_en_casa_..._.C2.BFnos_merece_la_pena_modificar_el_Entorno_de_Escritorio_de_Vitalinux.2FLubuntu.3F)
- [17.4 Ordenadores con Win XP con Pentium 3GHz y 1 GB de RAM ... ¿se podrían reutilizar con Vitalinux?](#Ordenadores_con_Win_XP_con_Pentium_3GHz_y_1_GB_de_RAM_..._.C2.BFse_podr.C3.ADan_reutilizar_con_Vitalinux.3F)
- [17.5 ¿En vitalinux siempre se instala el software a través de gestores? ¿No puedes llevar un ejecutable en un pendriver para instalar un programa como en windows?](#.C2.BFEn_vitalinux_siempre_se_instala_el_software_a_trav.C3.A9s_de_gestores.3F_.C2.BFNo_puedes_llevar_un_ejecutable_en_un_pendriver_para_instalar_un_programa_como_en_windows.3F)
- [17.6 ¿Desde migasfree se puede instalar software que no esté en repositorios (*p.e. un DVD para dar clases de ingles en el aula*)](#.C2.BFDesde_migasfree_se_puede_instalar_software_que_no_est.C3.A9_en_repositorios_.28p.e._un_DVD_para_dar_clases_de_ingles_en_el_aula.29)

## ¿Sin acceso gráfico? Como resolver problemas cuando no tenemos acceso al entorno grafico

### Introducción

A consecuencia de las peticiones de varios de vosotros con problemas en el arranque de los equipos ya que no se consiguen iniciar con ningún usuario, queremos facilitar un procedimiento para repararar un equipo dañado.


### Síntomas

Uno de los mayores problemas con el que nos encontrarmos es que NO se puede iniciar sesión gráfica. Es decir:
** Aparece la pantalla de login de usuario (extraña más si tenemos el equipo configurado para que arranque de forma automática) y cuando hago login con cualquiera de ellos el sistema me vuelve a la pantalla de login**. Por tanto el sistema no arranca el entorno gráfico.


Estos problemas suelen aparecer por ejemplo cuando no hemos realizado un apagado adecuado de la máquina, normalmente cuando estaba por ejemplo instalando una actualización y no hemos dado tiempo a que termine. Puede afectar a software del sistema gráfico que impide que se cargue el escritorio.


Vitalinux cuenta con un sistema de autorecuperación del sistema para éstos casos. Es decir, cuando arranca el sistema lo primero que intenta es solucionar actualizaciones no terminadas, pero **requiere que el sistema gráfico arranque, es decir que un usuario entre en el sistema.**


Nos encontrarmos en una encrucijada. El sistema no puede autoreparse ya que necesita entrar en modo gráfico, pero no puede hacerlo.


### Propuesta de solución

Lo primero que necesitaremos es que el equipo esté conectado a la red ya que es posible que necesite descargar algo para poder recuperarse.

-  Si está por cable no tendremos problemas (ya que posiblemente tu red tenga servidor para asignar direcciones de forma dinámica)
-  Si el equipo se suele conectar por wifi deberás llevarlo a un punto donde puedas conectarle un cable de red
Si no hay opción de tener red, podemos seguir con el procedimiento ya que aún así podemos tener esperanzas...


#### Abrir una sesión por consola

Después abriremos una sesión por terminal para poder iniciar una sesión (recordamos que el entorno gráfico impide la entrada al sistema). Para ello realizamos la combinación de teclado: CTRL+ALT+F3 (a la vez). Ésto nos llevará a una terminal:


Una vez allí nos loguearemos indicando el usuario docente (+Intro). Cuando nos pida la password introduciremos la contraseña que tenemos en ese equipo para ese usuario (no aparecerán los típicos *, y parecerá que no se escribe nada ). Luego pulsaremos de nuevo Intro y ya tendremos una sesión de docente abierta en consola:


#### Comprobar si tenemos conectividad

Ahora podemos comprobar si tenemos red simplemente haciendo un ping a google. Para ello escribe 
`ping 8.8.8.8` y luego pulsa Intro. *Nota: Para parar el ping en cualquier caso pulsa la combinación CTRL+C*

-  Si responde es que tienes conexión-  Si no responde es que no tienes conexión
Si hay conectividad tendrás más posibilidades de que todo el proceso que falta termine con éxito.


#### Ejecución de comandos que intentan resolver configuraciones o instalaciones que se han quedado a mitad

Ahora deberemos introducir los dos siguientes comandos. Para ello escribe lo que se indca y pulsa Intro. Si en algún caso te pregunta por una solución escribe la opción por defecto. Si te pregunta por una contraseña, introduce la del usuario docente:
En primer lugar intentaremos que el sistema termine de configurar aquello que se pudo quedar a mitad:


En segundo lugar, y una vez que haya terminado el proceso anterior intentaremos terminar de instalar lo que quedara a mita:


#### Dejar el sistema actualizado

Podemos al final dejar el sistema perfectamente actualizado ejecutando lo siguiente:


Esperamos que ésto pueda ayudar a resolver los problemas encontrados. Si aún así no se resuelve, siempre puedes abrir una [incidencia en soporte](http://soporte.vitalinux.educa.aragon.es) indicando donde has tenido problemas


**Nota final:** * No dedemos olvidar una solución fácil y rápida. Reinstalar el equipo. Si hemos configurado el sistema para que todas las acciones sobre el equipo estén automatizadas con migasfree (programas instalados, configuraciones de impresoras...), reinstalar el sistema puede ser una alternativa muy rápida ya que la misma no demora más allá de 10 minutos. Si antes tenemos que sacar datos que no teníamos guardados podemos consultar [Vitalinux/FAQs_recuperar_datos](http://wiki.vitalinux.educa.aragon.es/index.php/Vitalinux/FAQs_recuperar_datos)*


## Como hacer uso de los libros digitales en Vitalinux

Una de las ventajas que nos va a aportar desplegar Vitalinux es que nos permite automatizar y/o gestionar de forma centralizada los libros digitales o iPacks de diversas editoriales.


En algunas ocasiones ésta acción se puede realizar de forma automática para el coordinador solicitando los libros necesarios, pero en otras ocasiones el libro/ipack deberá ser desplegado en cada centro por parte del coordinador. Dependerá mucho de la Editorial y Libro solicitado.


Éste documento pretende aclarar ésta información para que sepamos como actuar cuando necesitemos hacer uso de dichos materiales en nuestro centro.


Veamos pues como está la situación por Editoriales:


### Burlington

Los libros de burlington se pueden desplegar de forma sencilla


### Oxford

Con Oxford tenemos más problemas ya que no disponemos de todos los ipack. Conseguir más no es viable para el equipo actualmente. Además hay que tener en cuenta que la Editorial solo da soporte para instalaciones locales (no en servidor) y recomiendan que los docentes accedan a los ipack vía web usando Oxford Premium. Aún así, vemos que los ipack se pueden usar siguiendo el esquema de burlington.


*Nota sobre flash: Los libros de Oxford usan flash en su mayoría. Si no queremos tener problemas en el uso de los mismos (cuando usamos la versión online) deberemos usar el navegador Firefox. Recordar que Google Chrome ha dejado de dar soporte y funcionlidad a flash y es posible que nos encontremos con problemas usando dicho navegador)*


#### Como instalar un libro de Oxford

La instalación del libro de Oxford en local es sencilla.

1.  Obtienes el libro o bien en formato DVD, pincho o descargándolo de la web. Para ello habla con tu comercial
<li> Si lo descargas de la web o te la pasan en un formato .zip lo primero que debes hacer es extrarlo en el escritorio por ejemplo o en tu carpeta personal...luego lo podrás borrar ya que solo sirva para instalarlo

![](img/contenido-zip-oxford.png)
<li> Ejecutas el instalador correspondiente. Si has instalado un Vitalinux de 32 bits tendrás que usar setup-linux. Si es de 64 bits setup-linux-x64. Para saber cual es tu arquitectura puede preguntar a la aplicación (CTRL+Espacio) "Conocer Dire..."

![](img/ejecutando-instalador-oxford.png)
<li> Después del asistente te habrá creado un directorio en la cuenta del usuario (/home/docente) llamado "Oxford University Press" y dentro del mismo un directorio por libro que hayas instalado. Por ejemplo, si tienes varios libros:

![](img/listado-libros-oxford.png)
<li> Desde ahora puedes acceder al libro directamente entrando en el directorio que ha creado en "Oxford University Press" -&gt; linux -&gt; oup
<ul>1.  Pero como hemos indicado, puedes usar nuestra aplicación para arrancarlo de forma cómoda
<li> También puedes copiar el resultado (la carpeta con el libro que se ha creado en "Oxford University Press") al directorio docente del servidor caché e indicarnos que lo has copiado (a través de la incidencia) para que lo hagamos visible a todos los equipos de tu centro
1.  **Importante:** Si en tu centro tienes ordenadores donde has instalado Vitalinux en 32bits y otros en 64 bits, tendrás que instalar el libro en un equipo de 32 y en otro de 64 y copiar ambos (en directorios separados) al caché para que lo tengas disponible para todos los ordenadores. Es decir, si solo instalas el libro en un equipo de 32 bits, lo copias al servidor y lo preparamos para que se vea de forma general, solo será accesible para equipos con 32 bits (los equipos de 64 no lo verán disponible)</li></ul></li>
### Libros accesibles por Blinklearning

Algunos libros/editoriales empiezan a integrarse dentro de la plataforma de Blinklearning. Desde Vitalinux se ha facilitado la instalación de su cliente offline para acceder de forma sencilla a la plataforma.


### Pearson

Los libros de Pearson que nos hemos encontrado hasta ahora se pueden arrancar usando su cliente para Microsoft (usando Wine). Se pueden dejar en el caché y arrancar desde allí o arracarlos en local.


### MacMillan

La editorial nos ha facilitado el software que usan para poder acceder a los libros de la editorial. Dicho software se ha integrado en Vitalinux de forma que se puede instalar en aquellos equipos que lo soliciten (mediante etiquetas por ejemplo)


### SM

Desde Vitalinux facilitamos la instalación de la aplicación de Savia Digital de SM que permite descargar y ver los libros diponibles para el usuario a través de dicha plataforma. No se puede instalar de forma automática ya que requiere de un proceso de instalación interactivo...el usuario tendrá que instalar la plataforma en cada equipo que se quiera. Si se trata de otros libros de SM que no van a través de la plataforma se pueden considerar como los del último apartado de ésta página


### Santillana

Desde Vitalinux facilitamos la instalación de la aplicación de Aula Virtual de Santillana que permite descargar y ver los libros diponibles para el usuario a través de dicha plataforma. No se puede instalar de forma automática la plataforma...el usuario tendrá que instalar la misma pero se ha facilitado el proceso. Si se trata de otros libros Santillana que no van a través de la plataforma se pueden considerar como los del último apartado de ésta página


### Libros de Frances (Parachute, Adosphere, Vitamine...) y otros

Los libros que son puramente web, como los indicados y algunos de otras materias, se pueden tener disponibles de forma única en el servidor caché y podemos crear un lanzador en el escritorio/equipo que se quiera para poder acceder a ellos de forma cómoda.
Ésto dependerá del libro y de como se estructure. Tendremos que hacer un estudio del mismo si no nos lo hemos encontrado hasta la fecha.


*Nota sobre flash: Algunos de los libros que hemos visto (la mayoría) usan flash. Si no queremos tener problemas en el uso de los mismos deberemos usar el navegador Firefox. Recordar que Google Chrome ha dejado de dar soporte y funcionlidad a flash y es posible que nos encontremos con problemas usando dicho navegador). El lanzador que creamos desde soporte abre Firefox*


## ¿Cómo recuperar el GRUB y el MBR?

En ocasiones (p.e. arranques duales con Windows) puede resultar necesario recuperar el gestor de arranque GRUB o el MBR del disco. Es decir, tras llevar a cabo una instalación dual se debería ver un gestor de arranque similar al que se muestra en la siguiente imagen, pero por diversas razones es posible que no se muestre (*no se ha indicado correctamente la ubicación del gestor de arranque, reinstalación de Windows, etc ...*):


Para dar solución al problema anterior lo más recomendable es hacer uso del software **boot-repair** (*reparación de arranque*) en **modo Live desde tu distro Linux** favorita.  Por ejemplo:

1.  Arrancar el equipo afectado con Vitalinux en modo live desde un USB Bootable, y posteriormente instalar **boot-repair** (*la última ISO de Vitalinux ya viene con **boot-repair** preinstalado*).
1.  En caso de trabajar en modo live con otra distro diferente es posible que tengas que descargar **boot-repair**: [Proyecto Boot Reapir](https://sourceforge.net/projects/boot-repair-cd/)
Una vez tengamos disponible **boot-repair** (*reparación de arranque*) en nuestra distro Linux en modo live lo arrancaremos:


1.  Lanzamos una terminal, **CONTROL + ALT + T**, y escribimos **sudo boot-repair**
1.  En Vitalinux, al disponer de **synapse** podemos intentar **CONTROL + ESPACIO** y escribir **reparación de arranque**

![](img/vitalinux-dualizando-con-uefi-lanzador-boot-repair.png)
<p>
</p>

![](img/boot-repair-opciones-avanzadas.png)

Una vez abierto **boot-repair**, desde sus opciones avanzadas podremos decidir entre reparar/reinstalar el GRUB o el MBR.


1.  Es recomendable seguir los pasos recomendados, por lo que seleccionaremos **Reparación Recomendada**

![](img/vitalinux-dualizando-con-uefi-boot-repair1.png)
1.  Será necesario seleccionar el texto/comandos propuestos en una terminal y ejecutarlos.  Para ello abriremos una terminal, **CONTROL + ALT + T**, suplantaremos al superAdministrador **root** del sistema ejecutando el comando **sudo su** y pegaremos los comandos indicados.

![](img/vitalinux-dualizando-con-uefi-boot-repair2.png)
<p>
</p>

![](img/vitalinux-dualizando-con-uefi-boot-repair3.png)
1.  Al final nos sugerirá **Cargar el reporte a pastebin** para poder auditar el proceso y conocer si ha sucedido algo extraño en el proceso anterior.  Indicaremos **Si** sin más.

![](img/vitalinux-dualizando-con-uefi-boot-repair4.png)
1.  Una vez terminado el proceso de reparación simplemente reiniciaremos el equipo para comprobar que ya tenemos el menú de arranque correctamente establecido 

![](img/vitalinux-dualizando-con-uefi-boot-repair5.png)

Si todo ha ido bien, al reiniciar deberemos ver un menú similar al siguiente, desde el cual ya podremos lanzar Windows o Linux:


En el caso de que el menú mostrado por el gestor de arranque no nos guste o deseemos personalizarlo, podemos hacerlo mediante la aplicación **Grub Customizer**.  Para ello arrancaremos nuestro Vitalinux, ya sea el que tenemos instalado en disco físico o en modo Live (*Vitalinux tiene preinstalada esta aplicación de personalización del Grub*):


1.  Lanzaremos el Grub Customizer haciendo uso de **synpase** tecleando **CONTROL + ESPACIO** y escribiendo **customizer**:

![](img/vitalinux-dualizando-con-uefi-lanzando-grub-customizer.png)
1.  Una vez lanzada la aplicación, desde sus pestañas principales podremos editar el texto del menú que se muestra al iniciar el equipo, y el orden en que aparecen:

![](img/vitalinux-dualizando-con-uefi-grub-customizer1.png)
<p>
</p>

![](img/vitalinux-dualizando-con-uefi-grub-customizer2.png)
1.  Desde la pestaña referente a **Configuración de la apariencia** podremos incluso personalizar la imagen de fondo del menú de arranque (*resolución recomendada de 640x480*)

![](img/vitalinux-dualizando-con-uefi-grub-customizer3.png)
1.  Si todo ha ido bien, tras realizar y guardar la configuración anterior, al reiniciar el equipo se debería mostrar el nuevo aspecto del menú del gestor de arranque definido:

![](img/vitalinux-dualizando-con-uefi-tras-boot-repair-grub-customizer3.png)

## ¿Como recuperar datos de un equipo que necesito formatear?

Para recuperar datos tan sólo será necesario arrancar el equipo desde un USB Bootable (*creado a partir de la ISO de Vitalinux*) con Vitalinux en **modo live**.  Una vez iniciado haremos lo siguiente:

1.  Abriremos el explorador de archivos: **Tecla Super/Windows + E**
1.  Desde el explorador de archivos, a través del menú lateral **Lugares**, abrir las particiones del disco o discos de la máquina donde buscar los archivos a respaldar, tal como se puede apreciar en la siguiente figura:
## ¿Cómo instalar Software?

A la hora de instalar software tendremos dos opciones:


<li> **Desde la línea de comandos**.  Para ello tan sólo será necesario abrir una terminal (*CONTROL + ALT + T*) y ejecutar el siguiente comando: 
1.  **apt-get install *nombre-programa***
Con la finalidad de instalar la última versión del programa deseado se recomienda siempre actualizar los repositorios de software en primer lugar:
1.  **apt-get update &amp;&amp; apt-get install *nombre-programa***
</li>
<li> **Desde una aplicación gráfica**. Para ello tenemos diferentes opciones: **synaptic**, **centro de software**, **appgrid**, etc.  Para saber más sobre todo ello se remite la la parte correspondiente del curso de Aularagon: [Indice de contenidos del curso](http://wiki.vitalinux.educa.aragon.es/index.php/Curso_Formación_en_Vitalinux_Aularagon/indice) e [Instalación de Software](http://wiki.vitalinux.educa.aragon.es/index.php/Curso_Aularagon/Parte_5)
</li>

## ¿Cómo compartir una impresora desde Linux?

Para compartir una impresora en Linux podemos hacer uso de **CUPS** o de **Samba**, en función de si los equipos clientes que quieran hacer uso de ella sean otros equipos Linux o Windows.  Desde las opciones de impresora tendremos la opción de compartirla, y posteriormente en los equipos cliente, la configuraremos **haciendo uso de la dirección IP del equipo que la sirve**.


## ¿Se puede congelar todo el software en Vitalinux?

A priori, esta práctica de mantenimiento de equipos usada habitualmetne en entornos Windows esta totalmente desaconsejada.  Es decir, el **software** de un equipo es algo **vivo** que está en contante evolución y mejora que necesita actualizarse con la finalidad de dar solución a problemas detectados en ese software o con la finalidad de añadir nuevas funcionalidades.  Congelar el software sería equivalente a tener un equipo obsoleto y sin sentido.  Por esta razón, en Vitalinux sólo se ofrencen dos opciones de congelacón:

-  Congelación del Escritorio. 
-  Congelación de los directorios principales del perfil del usuario.
### Servicio de Congelación en Vitalinux

Actualmente se encuentra muy extendido en los centros educativos el uso de software encargado de la **congelación del equipo** con la finalidad de evitar degradaciones del sistema.  **Esto es un grabe error** por las siguientes razones:

1.  El **software/aplicaciones son algo vivo** que están en permanente evolución y mejora, razón por la cual no tiene ningún sentido **la congelación al estilo Windows**.  Es necesario permitir que las aplicaciones se actualicen con la finalidad de solucionar bugs/errores/problemas detectados por los propios desarrolladores de las aplicaciones
1.  Junto con el uso de la congelación, también se suele hacer uso de **software antivirus**. Esto es un **error mayúsculo** ya que no tiene ningún sentido instalar un antivirus y no tenerlo actualizado por culpa de la congelación.
1.  **La congelación al estilo Windows es algo perjudicial para la red informática** ya que al no permitir que las actualizaciones que se descargan e instalan en el equipo sean efectivas.  Es decir, la congelación esta provocando que todas las veces que el equipo se inicie, se vuelva de nuevo a tratar de descargar, instalar y actualizar las actualizaciones de nuevo sin ningún éxito.  En el caso de que se trate de una aula de informática con varios equipos este problema es más fácil de detectar ya que al iniciarse se puede comprobar que la conexión a Internet se ve afectada (*va más lenta al estar todos los equipos simultáneamente descargándose las actualizaciones*) y el equipo tarda mucho más tiempo en estar en condiciones de empezar a trabajar (*la descarga e instalación de las actualizaciones que se produce al arrancar el equipo colapsa parte de la potencia de procesamiento del equipo, CPU, provocando que el equipo se note más lento durante el inicio de sesión, en la interacción con el usuario, aumentando su tiempo de respuesta*)
Como solución de compromiso en **Vitalinux** se ofrece la opción de **Congelación** del equipo pero sólo en su aspecto, no en su software.  Es decir, en el caso de optar por la **Congelación de Vitalinux** debemos tener claro que estamos congelando los datos del usuario, su perfíl, pero no las aplicaciones instaladas.  **Las aplicaciones no se congelan permitiendo su correcta actualización**, evitando de esta forma todos los problemas que acontecen en Windows.  En concreto existen dos modalidades de congelación: **(1) Congelar únicamente el Escritorio** o **(2) Congelación total del perfil del usuario**.  Para poder hacer uso de esta funcionalidad es necesario asignar a los equipos Vitalinux la etiqueta migasfree **"SRV-CONGELARESCRITORIO"** o **"SRV-CONGELADORTOTAL"**, dependiendo si optamos por la primera o segunda modalidad.


A modo de ejemplo, si optáramos por la primera opción **(1)** de congelación percibiríamos que el Escritorio es inmutable (*el fondo de Escritorio, los elementos que contiene, su aspecto, etc.*), pero podríamos alterar el contenido del resto de carpetas del usuario (*Documentos, Descargas, etc.*) y las aplicaciones que tiene instaladas (*instalar nuevas aplicaciones, desinstalar cualquier aplicación y actualizar las que sean necesarias*).


En el caso de que optáramos por la segunda opción **(2)** de congelación ofrecida en Vitalinux podríamos advertir que cualquier cosa que guardemos en cualquier carpeta de nuestro perfil (*Documentos, Descargas, Vídeos, Música, etc.) se perdería, al igual que cualquier modificación que hiciéramos del Escritorio.  Por contra, las aplicaciones del sistema estaría sin congelar (*instalar nuevas aplicaciones, desinstalar cualquier aplicación y actualizar las que sean necesarias*).  Puntualizar que esta congelación no impide que los estudiantes y docentes puedan guardar su información, ya que o bien pueden guardarlo en su **pendrive**, o bien lo pueden guardar de manera centralizada en un pequeño servidor accesible desde cualquier equipo vitalinux del centro.*




**¿La congelación Total en Vitalinux no me permite guardar nada dentro de mi perfil de usuario?**\nEn realidad sólo se congela el Escritorio, y las carpetas de uso habitual (Documentos, Descargas, Vídeos, Música, etc.).  La carpeta raíz del perfil (*/home/docente, /home/estudiante, /home/aularagon, etc.*) y sus carpetas ocultas (***CONTROL + H**, para ver los directorios ocultos, los que empiezan por un punto "."*)</p></td>




### ¿Cómo puedo hacer prácticas de instalación de software sin que persistan en Vitalinux?

En algunas asignaturas se estudia y practica con el sistema operativo (*instalación/desinstalación de software, instalación de impresoras, configuración de la red, creación de usuarios, etc*). Con los sistemas de congelación al estilo Windows (*p.e. deepfreeze*) era posible deshacer todos los cambios realizados durante esas prácticas al reiniciar. ¿Se puede hacer algo similar en Vitalinux?.


Para ese tipo de prácticas se aconseja el uso de máquinas virtuales con **VirtualBox**.  Este programa te permite crear instantáneas del sistema (*guardar estados del software de la máquina Virtual en determinados momentos*) y poder regresar a esos estados de software en el momento que se desee.  **VirtualBox** es un programa muy potente y sencillo de usar.  


Otra opción sería indicar a **migasfree** que deshiciera todos los cambios, pero habría que definir claramente que es lo que se quiere deshacer (*se podría dar la orden de desintalación de software no deseado, de echar atrás cambios de configuración realizados, etc.*).


## ¿Qué pasa si apagamos un equipo Vitalinux sin que el cliente Migasfree haya terminado la comunicación con el servidor Migasfree?

A priori **no pasa nada por apagar o cerra sesión en Vitalinux** sin que el **cliente Migasfree** haya terminado la comunicación con el **servidor Migasfree**.  Esta situación ya se ha tenido en cuenta de tal forma que la próxima vez que en Vitalinux se vuelva a iniciar sesión por parte del **cliente Migasfree** éste termine todas las tareas que quedaron pendientes (*instalación de software, desinstalación de software, actualización de softare, tareas específicas programadas, etc ...*).


## Error 500 al Actualizar contra Migasfree

Si al intentar conectarse el Equipo cliente Vitalinux contra Migasfree aparece un **error 500** puede ser debido a que **el Computer_Name** no es correcto.  Para solucionarlo:

1.  Abre una terminal: CONTROL+ALT+T
1.  Suplanta al root: sudo su
1.  Edita el archivo de configuración de migasfree: /etc/migasfree.conf
1.  Busca la linea "Computer_Name=..." y deja únicamente los 12 primeros caracteres. Por ejemplo: Computer_Name=07:70:65:12:23:AA
1.  Cierra nano guardando los cambios: CONTROL+X y después ENTER
1.  Prueba a actualizar desde la terminal migasfree, comprobando que ya se conecta (o para ver si sigue dando el error): migasfree -u
## ¿Cómo evitar el anillo o depósito de Claves al registrar una red Wireless?

Vitalinux, al basarse en Ubuntu, hace uso de de un depósito de claves para evitar que el usuario tenga recordar las diferentes claves que actualmente deben introducirse para acceder a determinados recursos (*claves de acceso a redes Wireless, claves de acceso a recursos compartidos, etc.*).  De esta forma un usuario del sistema puede almacenar en dicho depósito todas las claves que le interesen y no tener que aprendérselas de memoria.  No obstate, con la finalidad de evitar que cualquier **usuario malintencionado** pueda hacer uso de dichas claves simplemente iniciando sesión el equipo, es necesario definir una **clave de acceso al anillo o depósito de claves**, de tal forma que sabiendo una única clave de acceso podemos tener acceso a un conjunto de claves sin saberlas de memoria.


Por todo lo anterior, cuando un usuario en Vitalinux/Ubuntu se registra en una nueva red Wireless introduciendo su contraseña de acceso, esta se va a añadir a su anillo o depósito de claves, y por tanto, en caso de no haberse definido previamente, se le va a pedir al usuario que contraseña o password se desea para poder acceder posteriormente y consultar las claves/contraseñas/passwords almacenadas.  Esta última es la **clave o contraseña del depósito de claves**:


En el caso de las contraseñas de las redes Wireless, **si queremos evitar que el usuario tenga introducir la contraseña de desbloqueo del anillo o depósito de claves cada vez que el equipo Vitalinux se inicia y quiere conectarse a la red inalámbrica** (*la clave de la Wireless esta previamente almacenada en dicho deposito*) deberemos configurar esa red como global para todos los usuarios de Vitalinux.  Al hacer lo anterior, la contraseña de la red inalámbrica pasará a ser almacenada por el sistema Vitalinux para que cualquier usuario pueda hacer uso de la conectividad ofrecida por la red inalámbrica, en lugar de que este almacenada en el deposito de claves de un usuario concreto.  Para ello será necesario seguir los siguientes pasos:


1.  Configurar las **conexiones de red** de Vitalinux.  Para ello teclear **"CONTROL + ESPACIO"'** y escribir **"conexiones de red"**.  Según el perfil del usuario que lleve a cabo esta acción será necesario introducir en algún momento una contraseña de administrador

![](img/evitar-anillo-de-claves-wireless-conexiones-de-red.png)
1.  Seleccionar la red Wireless que deseamos que pueda ser usada por cualquier usuario de Vitalinux sin necesidad de tener almacenada en su deposito de claves la clave de esa red Wireless, y después pinchar sobre el botón **"Editar"** con la finalidad de poder editar la configuración asociada a esa red Wireless 

![](img/evitar-anillo-de-claves-wireless-conexiones-de-red-3.png)
1.  Ir a la **"pestaña General"** y seleccionar el **"checkbox"** que indica que **"Todos los usuarios deben conectarse a esta red"** Wireless 

![](img/evitar-anillo-de-claves-wireless-conexiones-de-red-4.png)

## ¿Qué implica tener activa en Vitlainux la etiqueta ENT-estudiante o ENT-docente?

Al tener marcada alguna de esas etiquetas podemos hacer tareas destinadas a los equipos que usen o bien docentes o bien estudiantes.  Es decir, puede ser que un docente llamado "arturo" trabaje bajo una cuenta de usuario que ha creado (p.e. "arturo").  Sólo a través de dicha etiqueta podemos actuar sobre ese equipo Vitalinux sabiendo que ese usuario "arturo" es en realidad un "docente", y no un "estudiante", y así de esta manera configurar lo que se nos pueda pedir que hagamos.


Por ejemplo, configurar los libros de inglés de Oxford en los equipos Vitalinux que usen los docentes de un centro (aquellos que tengan asignada la etiqueta ENT-docente).


## Para evitar que los docentes puedan modificar la configuración de impresoras e instalación de programas, ¿la opción más lógica es que entren con el usuario estudiante?

En principio da igual, ya que para poder hacer cualquier cambio en un equipo Vitalinux es necesario introducir la contraseña de administración, del docente o de alguna cuenta administrativa.  Es decir, si un docente inicia sesión de manera automática como usuario del sistema **"docente"**, si no sabe su contraseña asociada no va a poder hacer nada.  Es decir, la seguridad en ese aspecto radica en conocer la password administrativa.


En relación a esa **password** asociada a los usuarios con perfil de **Administrador** (*p.e. docente, dga, ...*), hay centros educativos que nos piden cambiar las contraseñas por defecto en todos sus equipos Vitalinux a través de migasfree (*nos envían de manera personal/confidencial a nuestro email las nuevas passwords deseadas para los usuarios del sistema Vitalinux*).  Una vez sabemos nosotros las nuevas contraseñas, de manera automátizada y transparente para los centros, **migasfree** actualiza las passwords en todos sus equipos.


## ¿Cambiar el idioma para un usuario es posible?

Puede ocurrir que queramos usar otro idioma que no sea el castellano para nuestro sistema (nos sentimos más cómodos con inglés, estamos trabajando en un entorno bilingüe, ...).
¿Es posible cambiar el idioma del sistema? Sin duda. Para ello:

-  Deberemos cerrar la sesión donde estemos (si tenemos el inicio de sesión automática) y a la hora de introducir usuario y contraseña para entrar al sistema seleccionar el usuario deseado y en el icono de idiomas que aparece arriba a la derecha seleccionar el idioma con el que arrancar -  **Importante**: la primera vez que arranque, el sistema nos preguntará si queremos cambiar los nombres de los directorios personales. Deberíamos mantener los nombres antiguos (en castellano) para que algunas de las funcionalidades de Vitalinux funcionen correctamente. Para ello simplemente indica "Keep Old Names" y marcha la casilla de "Don's ask me this again" para que no nos lo vuelva a preguntar -  A no ser que cambiemos de nuevo el idioma en el arranque del usuario, dicho usuario entrará con el nuevo idioma seleccionado en futuras sesiones (aunque esté activado el arranque automático)
### Idiomas

Por defecto todos los Vitalinux vienen con los idiomas castellano e inglés preinstalados por defecto. Si quisiéramos otros idiomas se podrían instalar sin problemas, o bien indicándolo a través de soporte para que se realice en todos nuestros ordenadores, o ejectuando en el equipo donde se desee lo siguiente por terminal:


## ¿Problemas con los Ajustes de Resolución del Monitor?

En el caso en que desees cambiar la resolución de salida (p.e. monitor o monitores, cañón o proyecto, etc.) en tu equipo Lubuntu/Vitalinux será tan sencillo como abrir "Ajustes del Monitor" (tecleas "CONTROL + ESPACIO" y escribes "Ajustes del Monitor"). Desde allí podrás tanto imponer una resolución para la sesión en la que te encuentras, como guardarla para que sea tenida en cuenta en posteriores inicios de sesión.


El problema detectado consiste en que en ocasiones tras guardar la resolución deseada en "Ajustes del Monitor" en los siguientes inicios de sesión no es tenida en cuenta.  Es decir, tras guardar la resolución deseada se crea dentro del perfil del usuario en ".config/autostart" un lanzador que trata de ejecutarse cada inicio sesión para imponer la resolución deseada, pero en el momento en que se ejecuta el entorno de Escritorio de Lubuntu/Vitalinux (LXDE) no le ha dado tiempo todavía a reconocer todas las interfaces gráficas que hay en el sistema y sus posibilidades (p.e. Resoluciones posibles a adoptar), por lo que lo no surte efecto.


Para dar solución a este problema de imposición de resolución gráfica, gracias a Migasfree, actuamos de la siguiente manera de manera automática y desatendida:


1.  Creamos a través de migasfree un acceso directo en el Escritorio o lanzador donde al pinchar sobre él se cambiará a la resolución deseada. Esta opción es deseado por aquellos centros (equipos de docentes) donde no siempre están proyectando la imagen, de tal forma, que sólo cuando se va a proyectar es cuando intencionadamente el docente pincha dos veces sobre dicho acceso directo del Escritorio (o CONTROL + ESPACIO ...)
1.  Configuramos el equipo para forzar esa resolución tras iniciar sesión, justo antes de que empiece la comunicación con el servidor Migasfree. Esta opción forzará la resolución elegida y guardada en cuanto el sistema, tras iniciar sesión, reconozca ya las interfaces gráficas y sus posibilidades.

## ¿Cómo subir archivos a Google Drive?

1.  Abres Google Drive y te situas en el directorio donde quieres subir los documentos
1.  Abres el explorador de archivos de Vitalinux y seleccionas los archivos o directorios que quieres subir
1.  Una vez seleccionados pinchas con el botón izquierdo del ratón sobre ellos manteniendo dicho botón pulsado (sin soltar el botón izquierdo del ratón), para hacer la mención de arrastrarlos 
1.  Para arrastraslos a Google Drive, al mismo tiempo que mantienes pulsado el botón izquierdo del ratón pulsas la combinación de teclas "ALT + TABULADOR" para navegar entre las aplicaciones abiertas hasta situarte sobre la ventana de la aplicación Google Drive. Una vez allí verás que Google Drive "te invita" a soltar el botón del ratón para que se peguen los documentos sobre el directorio de Google Drive seleccionado.

## Arquitectura de 32 bits o de 64 bits?

Muchas veces dudamos sobre cual es la arquitectura que tengo que descargar/instalar en nuestros equipos...si 32 o 64 bits. Una cosa es tener un sistema operativo (Linux, Windows...) de 32 bits o de 64 bits y otra cosa es que nuestro ordenador (la CPU) soporte sistemas operativos de 32 o de 64 bits. 
Lo primero es saber qué arquitectura soporta nuestra máquina, ya que...


### Hardware
-  Si nuestra CPU soporta 64 bits podremos instalar un sistema operativo de 32 bits o de 64 bits.
-  Si nuestra CPU no soporta 64 bits, solo podremos instalar un sistema operativo de 32 bits.
¿Como podemos saber si mi ordenador soporta o no dichas arquitecturas?


Por norma general, todas las CPU's modernas (desde la siguiente generación de Pentium IV) soportan 64 bits, pero nos tenemos que asegurar. Para ello podemos:

-  Buscar en la web nuestro procesador y comprobar que arquitectura soporta
<li> Ejecutar algún comando en Windows que nos identifique la arquitectura de la CPU. Para ello abrimos una terminal y ejecutamos
<dl><dd> ` echo %PROCESSOR_ARCHITECTURE% `</dd></dl></li>
<li> Desde Linux, abrimos una consola y ejecutamos 
<dl><dd> ` lscpu `
<dl><dd>En el apartado de modos de operación nos indicará que modos soporta</dd></dl></dd></dl></li>
### Rendimiento

Si la CPU soporta 64 bits encontraremos que el equipo funciona de forma mas óptima con un Sistema Operativo de 64 bits ya que podremos aprovechar al máximo las funcionaliades que nos ofrece la CPU. Si vamos a ejecturar aplicaciones que necesitan mucho cómputo será bueno contar con el sistema optimizado...
En el caso de querer contar con más de 4GB de RAM, había problemas en arquitecturas con 32 bits hasta que se introdujo PAE (que solucionó el límite teórico de 4GB para ampliarlo a 64GB. Linux lo soporta por defecto, por lo que podremos instalar 32 bits en equipos de mas de 4 GB de RAM.
A modo de ayuda, en pruebas que hemos realizado en equipos *antiguos* que soportan 64 bits (por ejemplo algunos Pentium IV) y no con mucha RAM (1GB de RAM), no encontramos diferencias entre Sistema Operativo de 32 o de 64 con un uso básico (ver párrafo anterior)


### Aplicaciones

Luego están las aplicaciones...hay aplicaciones que están preparadas para ejecutarse en Sistemas Operativos de 32 o 64 bits, pero nos podemos encontrar aplicaciones que solo funcionan en una arquitectura concreta. En éste último caso suelen ser aplicaciones antiguas que si hicieron para 32 bits. A día de hoy, podemos ejecturar aplicaciones de 32 bits en un equipo de 64 (Vitalinux lleva ya preparado el sistema para soportar ésta funcionalidad), pero aún así podemos encontrar problemas. 


También nos podemos encontrar que aplicaciones más modernas no liberan ejecutables para 32 bits...por ejemplo, Google  ya no actualiza su navegador Chrome para arquitecturas de 32 bits, quedándonos en éste caso sin poder actualizar dicho navegador


### Resumiendo
-  Si el equipo es relativamente moderno y sabemos que las aplicaciones que vamos a correr funcionan en ambas arquitecturas, se aconseja instalar 64 bits. Si tenemos más de 4 GB de RAM también será nuestra opción. 
-  Si el equipo es antiguo (pentium IV o similar), 32 bits.
De todas formas siempre podemos comprobar con los dos y sacar propias conclusiones....con Vitalinux reinstalar es muy rálido!!!!


## Ubuntu o Lubuntu

**Vitalinux** esta basado en **Lubuntu** con la finalidad de **aprovechar parte sus características de ligereza**.  A continuación se plantean posibles cuestiones que se nos podrían ocurrir.


### ¿Lubuntu es ligero por el software preinstalado y su Entorno de Escritorio?

Esta es una pregunta bastante ambigüa e imprecisa ya que dentro de Ubuntu existen multitud de distribuciones: **Ubuntu**, **Ubuntu Mate**, **Xubuntu**, **kubuntu**, **Edubuntu**, **Lubuntu**, etc.  Es decir, a consecuencia de que el software es libre existen múltiples opciones de distribución de **Ubuntu**, y cada una de estas distribuciones se caracteriza por tener un **Entorno de Escritorio** característico y un conjunto de aplicaciones preinstaladas que no tiene porque ser igual en todas las distribuciones.  **Lubuntu** se caracteriza por haber seleccionado el **Entorno de Escritorio** y **Aplicaciones** más ligeras que existen, pero tenemos que tener en cuenta que **Vitalinux** aún basándose en **Lubuntu**, no es tan ligero ya que se le han agregado aplicaciones como **Google Chrome** o las **LibreOffice** que no son las más ligeras dentro del área que ocupan.


### ¿Qué perderíamos y ganaríamos en el caso de que Vitalinux se basara en otra distribución de Ubuntu?

Básicamente, **perderíamos la ligereza de su Entorno de Escritorio**, y dependiendo de la distribución de Ubuntu que eligiéramos, ganaríamos en un **Entorno de Escritorio más amigable, más vistoso, más trabajado, ..." a costa de un consumo de recursos mayor.**





### Si tenemos ordenadores potentes en casa ... ¿nos merece la pena modificar el Entorno de Escritorio de Vitalinux/Lubuntu?

Si tenemos claro que entorno de Escritorio usar, ¡¡sí!!.  Simplemente tenemos que ir a nuestro gestor de software preferente (*p.e. synaptic*) e instalarlo.  Después cerrar sesión e indicar cual queremos que sea nuestro nuevo **Entorno de Escritorio**.





### Ordenadores con Win XP con Pentium 3GHz y 1 GB de RAM ... ¿se podrían reutilizar con Vitalinux?

A priori, ¡¡sí se podrían reutilizar!!  El único inconveniente que pueden presentar es que su placa base y procesador sean **NON-PAE**, lo cual sería un impedimento con la instalación de las actualizaciones del núcleo (*kernel*) del sistema Linux.  Lógicamente, si introdujéramos mejoras en su hardware, como por ejemplo, añadir un disco duro de estado sólido, se notaría muchísimo en su rendimiento, pero tendríamos que tener en cuenta que el coste que eso implicaría sería muy superior a el valor de cotización del propio equipo.


### ¿En vitalinux siempre se instala el software a través de gestores? ¿No puedes llevar un ejecutable en un pendriver para instalar un programa como en windows?

¡¡Si es posible!! Simplemente hay que pinchar con el botón derecho del ratón sobre el paquete software (*formato DEB*) que hayamos descargado e indicar que queremos instalarlo a través de **Gdebi** (*es un instalador de paquetes previamente descargados*).





### ¿Desde migasfree se puede instalar software que no esté en repositorios (*p.e. un DVD para dar clases de ingles en el aula*)

Migasfree puede hacer cualquier cosa que esté relacionada con el software.  Nosotros lo que hacemos es lo siguiente:

-  Si es un software de terceros que no está en los repositorios oficiales de Ubuntu (*p.e. Google Earth*): 1.  Lo descargamos de la Web de sus desarrolladores
1.  Lo subimos al servidor Migasfree
1.  Migasfree lo distribuye a los equipos que queramos-  Si es otro tipo de software (*p.e. un DVD para dar clases de inglés/francés en el aula*):1.  Instalamos el DVD en el servidor Caché que se coloca en los centros
1.  Mediante Migasfree, en los equipos que se desee creamos los lanzadores en el Escritorio y donde haga falta, para poder ejecutar la aplicación que hay en el servidor Caché
## ¿Cómo Customizar o personalizar el menú de opciones de arranque del Grub?

En el caso de que el menú mostrado por el gestor de arranque no nos guste o deseemos personalizarlo, podemos hacerlo mediante la aplicación **Grub Customizer**.  Para ello arrancaremos nuestro Vitalinux, ya sea el que tenemos instalado en disco físico o en modo Live (*Vitalinux tiene preinstalada esta aplicación de personalización del Grub*):


1.  Lanzaremos el Grub Customizer haciendo uso de **synpase** tecleando **CONTROL + ESPACIO** y escribiendo **customizer**:

![](img/vitalinux-dualizando-con-uefi-lanzando-grub-customizer.png)
1.  Una vez lanzada la aplicación, desde sus pestañas principales podremos editar el texto del menú que se muestra al iniciar el equipo, y el orden en que aparecen:

![](img/vitalinux-dualizando-con-uefi-grub-customizer1.png)
<p>
</p>

![](img/vitalinux-dualizando-con-uefi-grub-customizer2.png)
1.  Desde la pestaña referente a **Configuración de la apariencia** podremos incluso personalizar la imagen de fondo del menú de arranque (*resolución recomendada de 640x480*)

![](img/vitalinux-dualizando-con-uefi-grub-customizer3.png)
1.  Si todo ha ido bien, tras realizar y guardar la configuración anterior, al reiniciar el equipo se debería mostrar el nuevo aspecto del menú del gestor de arranque definido:

![](img/vitalinux-dualizando-con-uefi-tras-boot-repair-grub-customizer3.png)

## Drivers para las tarjetas wireless Broadcom

Las tarjetas wireless Broadcom dan algunos problemas a la hora de funcionar correctamente en Vitalinux (o mejor dicho, en Linux en general). Por defecto se instalan los drivers genéricos para dichas tarjetas pero no siempre funcionan de forma adecuada y es posible que tengamos que realizar alguna actuación para que dicha tarjeta sea reconocida por el sistema y podemos usarla para conectarnos a la red.
L primero es comprobar si el modelo de nuestra tarjeta es una Broadcom43XX (XX diferentes números, dependiendo del modelo)
Para ello abriremos una terminal `Ctrl+Espacio` y cuando nos salga la aplicación escribiremos y luego pulsaremos Enter:


Si nos aparece nuestro modelo podemos intentar la solución más sencilla y que suele funcionar que es escribir lo siguiente en la misma terminal (y acabarlo con Enter):


Una vez finalizado reiniciamos y esperamos a que funcione.
Si no funciona, podemos buscar soluciones más específicas. Para ello consultar [la siguiente página](http://blog.desdelinux.net/solucionar-problema-con-wifi-broadcom-43xx-en-ubuntu-despues-de-la-actualizacion/) con más información


[Referencia](http://askubuntu.com/questions/765584/is-it-possible-to-use-broadcom-bcm43142-wifi-in-ubuntu-16-04)


## ¿Cómo configurar una impresora USB en Vitalinux?

La configuración de una impresora en Linux/Vitalinux es muy sencillo.  A continuación se detallan los pasos necesarios para la instalación y configuración de una impresora local USB, aunque los pasos a seguir serían similares en el caso de que se tratara de una impresora o fotocopiadora en red.


1.  Conecta la impresora a la red eléctrica y al equipo para que éste la detecte 
<li>
Accederemos al **Panel de Control de gestión de Impresoras**.  Para ello **CONTROL + ESPACIO** y escribimos **"Impresoras"**
</li>

![](img/vitalinux-configurar-impresora-1.png)
<li>
Pinchamos sobre el botón asociado a **Añadir una nueva Impresora**
</li>
1.  Seleccionamos la **Impresora Detectada** por el sistema Linux que queremos instalar y configurar (*p.e. una impresora USB*).  En el caso de que se trate de una impresora o fotocopiadora en Red deberemos pinchar en **Buscar impresora de red** e indicar su dirección IP, y seleccionar el protocolo o **modo de conexión** usado para comunicarse con ella

![](img/vitalinux-configurar-impresora-2.png)

![](img/vitalinux-configurar-impresora-3.png)
<li>
Una vez el sistema haya autocomprobado que dispone del driver de comunicación adecuado para comunicarse con ese modelo de impresora, nos mostrará un dialogo con las **Opciones de Configuración de la Impresora**
</li>

![](img/vitalinux-configurar-impresora-4.png)
1.  Indicaremos un **Nombre** que identifique a la impresora (*evitaremos hacer uso de espacios en blanco*), una **Descripción** y una **Localización**, los cuales nos permitirán identificar ese modelo de impresora a posteriori 

![](img/vitalinux-configurar-impresora-5.png)
1.  Tras la configuración de la impresora se nos invitará a mandarle un trabajo de prueba y así comprobar su correcto funcionamiento 

![](img/vitalinux-configurar-impresora-6.png)
<li> A posteriori, desde el **Panel de Control de la gestión de Impresoras**, pinchando con el **botón derecho** del ratón sobre la impresora deseada podemos personalizar su comportamiento por defecto: *Tamaño de papel, Color o Blanco y Negro, Una cara o Doble cara, etc.*

![](img/vitalinux-configurar-impresora-7.png)
</li>
Como ***más vale un buen videotutorial que mil palabras*** a continuación se sugiere ver el [siguiente vídeo](https://youtu.be/yuUDWJwABbM) relacionado con la teoría de esta parte del curso: **Instalación y Configuración de Impresoras**


## ¿Problemas con algún modelo HPLaserJet 1005, 1018, 1020, 1102, 2015, ...?

Gracias a **Fernando Peña**, MIA el IES Miralbueno, a continuación daremos una solución a un conjunto de impresoras HP LaserJet para las cuales los drivers disponibles por defecto no funcionan.


En el **caso de que la detección de la impresora o posterior configuración no resulte exitosa**, es posible que tengamos que hacer uso del software privativo del fabricante para darle una solución.  Este puede ser el caso de los modelos HPLaserJet 1018, 1020, P1102, P1102W, etc.  En ese caso concreto, para que sirva de ejemplo, los pasos a seguir serían los siguientes:

****<center>¡¡Cuidado si la impresora es USB!!</center>\nUn detalle a tener en cuenta antes de empezar es que **si la impresora va por USB**, no hay que conectarla hasta que nos lo diga el asistente posterior de instalación. Si ya está conectada, en un momento de la instalación habrá que desconectar el cable USB y volver a conectarlo. Si la conexión es por red puede estar conectada desde el principio</p></td>




1.  Vamos a la página **[http://hplipopensource.com/hplip-web/index.html](http://hplipopensource.com/hplip-web/index.html)** 

![](img/ies-miralbueno-configurar-impresora-pantalla1.png)
1.  Pulsamos en **"Download HPLIP"** 
<li>
**Seleccionamos la distribución y versión de linux (*Ubuntu 14.04*)**, además del tipo y modelo de impresora. Nos lleva a otra pantalla donde nos da la opción de seguir o corregir. Pulsamos **"Next"** y nos lleva a otra pantalla para descargar lo necesario.  En algún punto de este proceso nos dirá que nuestra versión ya viene preparada para la impresora. Seguimos adelante.
</li>

![](img/ies-miralbueno-configurar-impresora-pantalla2.png)

![](img/ies-miralbueno-configurar-impresora-pantalla3.png)

![](img/ies-miralbueno-configurar-impresora-pantalla4.png)
<li>
Accedemos a otra pantalla con las instrucciones (*en inglés*), [http://hplipopensource.com/hplip-web/install/install/index.html](http://hplipopensource.com/hplip-web/install/install/index.html), y el botón de descargar.
</li>

![](img/ies-miralbueno-configurar-impresora-pantalla5.png)

![](img/ies-miralbueno-configurar-impresora-pantalla6.png)
<li> Descargamos, abrimos el terminal, nos vamos a la carpeta donde está la descarga y seguimos las instrucciones (*básicamente es elegir las opciones por defecto*)
</li>

![](img/ies-miralbueno-configurar-impresora-pantalla7.png)

![](img/ies-miralbueno-configurar-impresora-pantalla8.png)

![](img/ies-miralbueno-configurar-impresora-pantalla12.png)

## ¿Cómo configurar un escáner USB en Vitalinux?

La configuración de un escáner en Linux/Vitalinux es muy sencillo, ya que no se requiere hacer absolutamente nada.  En el caso de que por algún motivo el escáner no sea correctamente detectado por el sistema la aplicación encargada de escanear (*p.e. Simple Scan*) nos avisará de ello:


Como ***más vale un buen videotutorial que mil palabras*** a continuación se sugiere ver el [siguiente vídeo](https://youtu.be/-A6CX4exyeg) relacionado con la teoría de esta parte del curso: **Instalación y Configuración de Escáneres**



![](img/road-works.png)

