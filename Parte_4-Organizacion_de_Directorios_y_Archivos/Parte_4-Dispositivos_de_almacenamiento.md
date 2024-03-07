# Dispositivos de Almacenamiento

## Contenido

- [1 Gestión de Unidades de Almacenamiento Externas](#GestionUnidadesAlmacenamientoExternas)
- [2 Administración Básica de los Dispositivos de Almacenamiento](#AdministracinBasicaDispositivosAlmacenamiento)
    - [2.1 Montar y Quitar](#MontarQuitar)
    - [2.2 Cambiar nombre del Dispositivo](#CambiarnombreDispositivo)
    - [2.3 Formatear un dispositivo](#Formatearundispositivo)

## Gestión de Unidades de Almacenamiento Externas {#GestionUnidadesAlmacenamientoExternas}

Vitalinux, como cualquier otro sistema operativo, permite trabajar con unidades de almacenamiento externas tales como **CDs/DVDs** o **memorias USB**.  Una vez insertado un CD/DVD o memoria USB, Vitalinux lo detectará y nos abrirá dicho dispositivo de almacenamiento o nos indicará una acción a realizar.  Al mismo tiempo se crearán un **acceso directo en el Escritorio** y un nuevo **marcador en el explorador de archivos** para poder acceder rápidamente a él.

Vitalinux no asigna una letra (D:\, E:\, etc.) a estas unidades de almacenamiento para identificarlas y acceder a su contenido, sino que crea nuevas ramas dentro del **árbol del sistema de archivos de Vitalinux**.  Concretamente, Vitalinux creará un directorio con el nombre del usuario dentro de **/media** (*p.e. si el usuario es **docente**, se creará el directorio **/media/docente***), y a su vez dentro de él se creará un subdirectorio por cada unidad de almacenamiento externa cuyo nombre coincidirá con la etiqueta que tenga asignada el dispositivo de almacenamiento.  Por ejemplo, si el usuario **docente** pincha una memoria USB identificada con la etiqueta **misdatos**, en Vitalinux se creará el directorio **/media/docente/misdatos** que contendrá todo el contenido del USB.

En el caso de que queramos desconectar de manera segura la unidad de almacenamiento externa USB podrá hacerse pinchando con el botón derecho del ratón sobre el acceso directo a dicha memoria que se creo en el Escritorio y seleccionando la **Acción** llamada **Extraer la unidad de forma segura**.  También es posible el desmontaje en modo seguro pinchando sobre el ***iconito*** de **eject** que aparece junto al **marcador del explorador de archivos** referente a dicha memoria o usando la aplicación disponible en el área de notificaciones en la barra de tareas para todos los dipositivos de almacenamiento.

## Administración Básica de los Dispositivos de Almacenamiento {#AdministracinBasicaDispositivosAlmacenamiento}

Hay dos tareas administrativas básicas cuando trabajamos con dispositivos de almacenamiento externo tipo "pincho"

1. **Cambiar el nombre** del dispositivo. Ésta operación nos va a permitir tener el dispositivo perfectamente identificado (sobre todo ahora que contamos con varios de ellos) de forma que vamos a poder reconocerlo fácilmente cuando insertamos varios
2. **Formatear** el dispositivo. Operación recomendable para borrar toda la información disponible y poder empezar a usarlo "limpio"...entre otras.
Para ejecutar éstas y otras acciones disponemos de varias herramientas o trucos, pero nos vamos a centrar en una herramienta muy sencilla disponible en Vitalinux llamada **Discos**. Para arrancar la aplicación, simplemente tecleamos la combinación **CTRL+ESPACIO** y escribimos **Discos** y lo podremos lanzar. Resaltar en éste punto lo fácil e intuitivo que podemos encontrar todo con Synapse

### Montar y Quitar {#MontarQuitar}

La acción de cambiar el nombre, igual que pasará con Formatear y otras, requiere que el dispositivo esté **desmontado**. ¿Qué significa ésto?.
Un pincho que está físcamente insertado y reconocido pero que nadie pueda acceder (<i>copiar, leer, crear directorios ni nada</i>).

{% notificacion_alert title='¿Desmontar o Quitar dispositivo?', logotext='¡¡Ojo!!' %}
Aqui se diferencia entre desmontar un dispositivo de forma segura o Quitar un dispositivo de forma segura. Éste último realiza las dos acciones: desmontar y quitarlo físicamente para el ordenador. En el caso de un DVD el Sistema hasta abre y expulsa de verdad el DVD, pero en el caso de un pincho de momento los ordenadores no pueden escupirlos...
{% endnotificacion_alert %}


### Cambiar nombre del Dispositivo {#CambiarnombreDispositivo}

Abrimos la herramienta de **discos** (con nuestro pincho insertado por ejemplo, aunque lo podemos insertar una vez abierto el programa), teclenado **CTRL+ESPACIO** y escribiendo **Discos**.
Veremos una interfaz como la que se adjunta en la captura. Aquí es importante reconocer los elementos

{% coolimages_type2 url_image="../img/Zonas-disco.png" %}
Herramienta de Discos
{% endcoolimages_type2 %}

1. En ésta zona podremos seleccionar el Disco con el que queremos trabajar. En éste caso tenemos el Disco Duro normal de la instalación, un lector de DVD y lo que es un pincho de 4GB.
2. Según el disco que tengamos seleccionado, en la zona 2 nos aparecerá un detalle del mismo: Modelo, Tamaño, Tipo de Particionado, Número de Serie del Disco, Particiones realizadas en el disco y su tipo....
3. En la zona 3 tendremos (al igual que con la ruleta de arriba) una serie de acciones a realizar.
Nos centramos en éste punto, ya que aquí es donde podremos desmontar el disco para cambiar el nombre. Para ello:

    *  Seleccionamos el pincho y lo desmontamos. Fijaros que en la zona 2 puedo ver que mi pincho se llama FF4GR.

    {% coolimages_type2 url_image="../img/Nombrediscos1.png" %}
    Desmontar el disco
    {% endcoolimages_type2 %}

    *  Al desmontar habrá desaparecido el acceso desde el escritorio a nuestro dispositivo. Pero podemos Editar sistema de archivos 

    {% coolimages_type2 url_image="../img/Nombrediscos2.png" %}
    Editar la particion para cambiar el nombre
    {% endcoolimages_type2 %}

4. Una vez que cambie el nombre, veremos que en la zona 2 ya aparece nuestro nuevo nombre: MIPINCHO, y puedo montarlo si quiero para tener acceso a él. Si lo hago me aparecerá un acceso al pincho en el escitorio y en el navegador de archivos con el nuevo nombre

    {% coolimages_type2 url_image="../img/Nombredisco3.png" %}
    Montar de nuevo el dispositivo
    {% endcoolimages_type2 %}

### Formatear un dispositivo {#Formatearundispositivo}

A veces un pincho empieza a dar problemas, va algo lento, no funciona muy bien o simplemente tiene muchas cosas o no sabemos que hay y queremos darle una buena limpia. Para ello lo mejor: **formatear**.

Ésta acción eliminará todo archivo que hubiera. Además vamos a poder elegir un **tipo de formato**, importante si queremos que nuestro pincho se accesible desde otros dispositivos. Los formatos disponible son:

-  FAT. Es el formato más compatible. Se puede leer en todos los Sistemas Operativos (windows, Linux, Mac..) y en todos los dispositivos: reproductores, televisiones y demás. La desventaja que tiene es que es algo antiguo, no es muy eficiente y no se lleva bien con tamaños grandes de pinchos y archivos...pero será nuestra mejor elección si queremos máxima compatibilidad. Sin embargo, si podemos nos iremos a...
-  NTFS. Es la evolución que sacó Microsoft. Es mucho mejor sistema que FAT, mas seguro y soluciona los problemas del anterior. Sin embargo podemos tener problemas con versiones muy antiguas de windows o dispositivos que no acepten éste formato. 
-  Ext4. Si solo vamos a usar el pincho en sistemas Linux, a todas luces es la mejor opción, pero normalmente buscaremos ser lo más compatible y nos iremos a una de las dos opciones anteriores...

Para llevar a cabo el Formateo, iremos a la misma aplicación de Discos y

*  **Seleccionamos el pincho** y lo desmontaremos si estaba montado

{% coolimages_type2 url_image="../img/parte4/discos_desmonta.png" %}
Desmontar el disco
{% endcoolimages_type2 %}

*  Ahora seleccionaremos la opción de Formatear

{% coolimages_type2 url_image="../img/parte4/discos_formatea.png" %}
Click Formatear
{% endcoolimages_type2 %}

* En las opciones, el sistema nos va a permitir
    1.  Hacer un borrado rápido o uno más lento y seguro que elimina todo a conciencia
    1.  El tipo de Sistema de Archivos
    1.  Podemos darle en éste momento un nombre, por si lo queremos renombrar (lo que hicimos en el punto anterior)

{% coolimages_type2 url_image="../img/parte4/discos_formatea_opciones.png" %}
Opciones de Formateo
{% endcoolimages_type2 %}

Luego solo quedará montarlo si queremos volver a usarlo.
