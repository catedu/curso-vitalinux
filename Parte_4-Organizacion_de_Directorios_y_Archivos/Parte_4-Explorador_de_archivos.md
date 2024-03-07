# Explorador de Archivos en Vitalinux: Características y Funcionalidades {#ExploradorArchivosVitalinux}

Un **explorador de archivos** es una aplicación de software que permite a los usuarios navegar y gestionar los archivos y carpetas en su sistema de archivos. También se conoce comúnmente como administrador de archivos. La función principal de un explorador de archivos es proporcionar una interfaz gráfica de usuario (GUI) para que los usuarios puedan interactuar con los archivos almacenados en sus dispositivos de almacenamiento, como discos duros, unidades USB, tarjetas de memoria y otros dispositivos de almacenamiento.

Las características típicas de un explorador de archivos son:

1. Navegación: Permite a los usuarios moverse entre diferentes carpetas y unidades para acceder a archivos y directorios.
1. Visualización de archivos: Muestra una lista o una vista gráfica de los archivos y carpetas presentes en una ubicación específica.
1. Copiar, cortar y pegar: Facilita la manipulación de archivos permitiendo a los usuarios copiar, cortar y pegar archivos y carpetas.
1. Búsqueda: Proporciona funciones de búsqueda para encontrar archivos basados en nombres o criterios específicos.
1. Creación y eliminación: Permite a los usuarios crear nuevas carpetas, eliminar archivos y carpetas, y realizar otras operaciones de gestión de archivos.
1. Propiedades: Muestra información detallada sobre los archivos, como tamaño, tipo, fecha de modificación, etc.
1. Vista previa: Algunos exploradores de archivos permiten la vista previa de archivos, lo que significa que puedes ver el contenido de un archivo sin abrirlo completamente.

En Linux existen diferentes exploradores de archivos: **Nautilus, konqueror, Thunar, Dolphin**, etc. Vitalinux, en su versión 2, al basarse en la versión ligera de Ubuntu, **LUbuntu**, hace uso del que supuestamente del explorador que consume menor cantidad de recursos del sistema, llamado **Pcmanfm**. En cambio, Vitalinux 3 hace uso de **Nemo**, un explorador de archivos no tal ligero pero más personalizable y funcional.

La forma más rápida y eficiente de lanzar el **Explorador de Archivos** es tecleando el atajo **Tecla de Windows + E** (*la tecla de Windows suele encontrarse en la fila inferior del teclado, a la izquierda de la barra espaciadora y la tecla ALT*), aunque puede lanzarse igualmente mediante el lanzador de aplicaciones **Albert**, tecleando **CONTROL + ESPACIO** y escribiendo **explorador de archivos**, o directamente pinchando con el ratón sobre **el icono de la carpeta** que hay en **la barra o panel del Entorno de Escritorio**.

Entre sus características y funcionalidades más destacables podrían destacarse las siguientes:

1. Es software libre. Por esta razón cualquier programador puede reutilizar el código y mejorarlo, haciendo que de ello nos beneficiemos toda la comunidad de usuarios.
1. Permite la apertura de multiples pestañas, lo que facilita el movimiento de archivos entre diferentes directorios (*arrastrar y soltar*).  Para abrir una nueva pestaña puede teclearse la combinación **CONTROL + T**
1. Permite crear **marcadores** para acceder de una manera muy rápida a los directorios que elijamos.  Estos **marcadores** se pueden crear pulsando la combinación de teclas **CONTROL + D** estando situados dentro del directorio al cual queremos crear un acceso rápido

    {% coolimages_type2 url_image="../img/parte4/marcadores.png" %}
    Pulsando CONTROL+D dentro del directorio deseado podemos crear un marcador asociado a dicho directorio que nos permitirá acceder a su contenido de una manera muy directa
    {% endcoolimages_type2 %}

1. Permite trabajar con un **panel doble** facilitando la copia y movimiento de archivos y directorios entre los paneles derecho e izquierdo

    {% coolimages_type2 url_image="../img/parte4/paneles.png" %}
    Pulsando F3 en el explorador de archivos te permite trabajar con un panel doble facilitando la copia y movimiento de archivos y directorios
    {% endcoolimages_type2 %}

1. Facilita la desconexión de los dispositivos de almacenamiento externos (*USB, CD/DVD, etc.*)
1. Soporta varios modos de vista de iconos: vista compacta, lista detallada y vista en miniatura. Para poder ver y cambiar entre los diferentes modos o vistas puede pulsarse las combinaciones **"CONTROL + 1"**, **"CONTROL + 2"**, **"CONTROL + 3"** o **"CONTROL + 4"**
1. Permite programar y añadir **Acciones** (*Action Scripts*) muy útiles que aumentan considerablemente las funcionales del navegador.  Esta es una característica es muy importante ya que el **Explorador de Archivos** detecta al vuelo el formato de un archivo (*p.e. PDF, TXT, EXE, etc.*) independientemente de la extensión que se le haya asignado, y en función de este nos muestra todas las **Acciones** que tiene configuradas para su manipulación.  Por ejemplo, en la siguiente figura se muestra como al pinchar con el botón derecho del ratón sobre una imagen de formato **PNG** nos aparecen una serie de funcionalidades (*comprimir imagen PNG, ver detalles de la imagen y crear replica en miniatura*) que no aparecerían si el archivo seleccionado hubiera sido una canción **MP3**. Estas **Acciones** se van añadiendo poco a poco a Vitalinux ya que son desarrolladas y testeadas por el equipo técnico de Vitalinux de manera altruista o a demanda de los centros

    {% coolimages_type2 url_image="../img/parte4/opciones_archivos.png" %}
    El explorador de archivos de Vitalinux permite añadir pequeños programas que permiten añadir nuevas funcionalidades o Acciones para la manipulación de los archivos en función del tipo o extensión que tengan
    {% endcoolimages_type2 %}

1. Permite suplantar al **root** o **Administrador de máximo rango del sistema**.  Esto puede resultar útil cuando la cuenta de usuario con la que se ha iniciado sesión en Vitalinux no tiene los privilegios/permisos necesarios para la manipulación de determinados ficheros.  Lógicamente, para poder hacer esta suplantación será necesario que la cuenta de usuario sea administrador del sistema (*p.e. **docente**, pero no **estudiante***).  Para hacer uso de esta funcionalidad tan sólo habrá que **pinchar con el botón derecho del ratón** sobre el archivo o directorio que queremos abrir con todos los privilegios y seleccionar la opción **Abrir como Root**

    {% coolimages_type2 url_image="../img/parte4/abrir_como_root.png" %}
    La funcionalidad Abrir como Root del Explorador de Archivos permite a los usuarios del sistema suplantar al administrador para abrir archivos y directorios con todos los permisos necesarios para su manipulación
    {% endcoolimages_type2 %}

