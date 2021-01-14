# Explorador de Archivos en Vitalinux: Características y Funcionalidades {#ExploradorArchivosVitalinux}

En Linux existen diferentes exploradores de archivos: **Nautilus, konqueror, Thunar**, etc. Vitalinux, al basarse en la versión ligera de Ubuntu, **LUbuntu**, hace uso del que supuestamente del explorador que consume menor cantidad de recursos del sistema, llamado **pcmanfm**.


La forma más rápida y eficiente de lanzar este **Explorador de Archivos** es tecleando el atajo **Tecla de Windows + E** (*la tecla de Windows suele encontrarse en la fila inferior del teclado, a la izquierda de la barra espaciadora y la tecla ALT*), aunque puede lanzarse igualmente mediante el lanzador **Synapse**, tecleando **CONTROL + ESPACIO** y escribiendo **pcmanfm**, o directamente pinchando con el ratón sobre **el icono de la carpeta** que hay en **la barra inferior del Entorno de Escritorio**.

Entre sus características y funcionalidades más destacables podrían destacarse las siguientes:

1. Es software libre. Por esta razón cualquier programador puede reutilizar el código y mejorarlo, haciendo que de ello nos beneficiemos toda la comunidad de usuarios.
1. Permite la apertura de multiples pestañas, lo que facilita el movimiento de archivos entre diferentes directorios (*arrastrar y soltar*).  Para abrir una nueva pestaña puede teclearse la combinación **CONTROL + T**
1. Permite crear **marcadores** para acceder de una manera muy rápida a los directorios que elijamos.  Estos **marcadores** se pueden crear pulsando la combinación de teclas **CONTROL + D** estando situados dentro del directorio al cual queremos crear un acceso rápido

    {% coolimages_type2 url_image="../img/Explorador-archivos-marcadores-2.png" %}
    Pulsando CONTROL+D dentro del directorio deseado podemos crear un marcador asociado a dicho directorio que nos permitirá acceder a su contenido de una manera muy directa
    {% endcoolimages_type2 %}

1. Permite trabajar con un **panel doble** facilitando la copia y movimiento de archivos y directorios entre los paneles derecho e izquierdo

    {% coolimages_type2 url_image="../img/Explorador-archivos-panel-doble-2.png" %}
    Pulsando F3 en pcmanfm permite trabajar con un panel doble facilitando la copia y movimiento de archivos y directorios
    {% endcoolimages_type2 %}

1. Facilita la desconexión de los dispositivos de almacenamiento externos (*USB, CD/DVD, etc.*)
1. Soporta varios modos de vista de iconos: vista compacta, lista detallada y vista en miniatura. Para poder ver y cambiar entre los diferentes modos o vistas puede pulsarse las combinaciones **"CONTROL + 1"**, **"CONTROL + 2"**, **"CONTROL + 3"** o **"CONTROL + 4"**
1. Permite programar y añadir **Acciones** (*Action Scripts*) muy útiles que aumentan considerablemente las funcionales del navegador.  Esta es una característica es muy importante ya que el **Explorador de Archivos pcmanfm** detecta al vuelo el formato de un archivo (*p.e. PDF, TXT, EXE, etc.*) independientemente de la extensión que se le haya asignado, y en función de este nos muestra todas las **Acciones** que tiene configuradas para su manipulación.  Por ejemplo, en la siguiente figura se muestra como al pinchar con el botón derecho del ratón sobre una imagen de formato **PNG** nos aparecen una serie de funcionalidades (*comprimir imagen PNG, ver detalles de la imagen y crear replica en miniatura*) que no aparecerían si el archivo seleccionado hubiera sido una canción **MP3**. Estas **Acciones** se van añadiendo poco a poco a Vitalinux ya que son desarrolladas y testeadas por el equipo técnico de Vitalinux de manera altruista o a demanda de los centros

    {% coolimages_type2 url_image="../img/Explorador-archivos-actions-archivo.png" %}
    pcmanfm permite añadir pequeños programas que permiten añadir funcionalidades o Acciones al navegador para la manipulación de los archivos en función del tipo que sean, Mime Type
    {% endcoolimages_type2 %}

1. Permite suplantar al **root** o **Administrador de máximo rango del sistema**.  Esto puede resultar útil cuando la cuenta de usuario con la que se ha iniciado sesión en Vitalinux no tiene los privilegios/permisos necesarios para la manipulación de determinados ficheros.  Lógicamente, para poder hacer esta suplantación será necesario que la cuenta de usuario sea administrador del sistema (*p.e. **profesor**, pero no **alumno***).  Para hacer uso de esta funcionalidad tan sólo habrá que **pinchar con el botón derecho del ratón** sobre el archivo o directorio que queremos abrir con todos los privilegios y seleccionar la opción **Abrir como Root**

    {% coolimages_type2 url_image="../img/Explorador-archivos-abrir-como-root.png" %}
    La funcionalidad Abrir como Root del Explorador de Archivos pcmanfm permite a usuarios con perfil de administrador abrir archivos y directorios con todos los permisos necesarios para su manipulación
    {% endcoolimages_type2 %}
