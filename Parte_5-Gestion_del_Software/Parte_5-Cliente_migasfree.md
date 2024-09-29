# Cliente Migasfree

## Contenido

- [Cliente Migasfree](#cliente-migasfree)
  - [Contenido](#contenido)
  - [Análisis de la comunicación con el Servidor Migasfree](#AnalisisComunicacionMigasFree)
    - [Interfaz](#Interfaz)
    - [Análisis de la comunicación entre el Cliente y Servidor Migasfree](#AnalisisComunicacionClienteServidor)
    - [Forzar Actualización contra Migasfree](#ActualizacionContraMigasfreConsola)
  - [Etiquetas Migasfree](#EtiquetasMigasfree)
    - [¿Qué son y para qué sirven las etiquetas Migasfree?](#EtiquetasMigasfree)
    - [Asignación de Etiquetas Migasfree](#AsignacionEtiquetasMigasfree)
    - [Comprobación de Etiquetas Migasfree](#ComprobacionEtiquetasMigasfree)
    - [Consideración especial](#ConsideracionEspecial)
  - [Habilitar o deshabilitar el cliente](#habilitar-o-deshabilitar-el-cliente)
  - [Video formativo](#video-formativo)

**Vitalinux EDU DGA** lleva como sistema base un **Lubuntu** (<i>una de las versiones ligeras de ubuntu con escritorio LXDE</i>), una personalización al entorno educativo y lo más importante: un **cliente Migasfree**. Este cliente permite a Lubuntu comunicarse con un servidor central controlado por los técnicos informáticos del proyecto de Software Libre para que a través de éste puedan gestionarse todos los equipos <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Vitalinux</tt></span>:


-  **Instalación/Desinstalación/Actualización del Software**
-  **Configuración del equipo de manera remota y desatendida**: 
    -  *Hora de Apagado*
    -  *Personalización del entorno de Escritorio* (_fondo de Escritorio, lanzadores, tema de iconos, etc._)
    -  Instalación y Configuración de *Impresoras/Fotocopiadoras*
    -  Instalación y configuración de *Libros digitales*
    -  Instalación de extensiones y personalización de los navegadores Web
    -  Configuración de las <b>redes Wireless</b> en los equipos portátiles
    -  Creación de cuentas de usuario con perfiles personlizados (_idioma, permisos, etc._)
    -  etc.  
-  **Detección y resolución de incidencias**
-  **Generación del Inventario** de todo el software y hardware de los Equipos
-  ...

¡¡Y todo ello **de manera completamente desatendida**!!  Esto facilita la labor de los coordinadores de medios informáticos de los centros y del docenteado ya que de esta forma se pueden desentender de este tipo de tediosas tareas y dedicarse realmente a su trabajo (_enseñar_).

Se puede ver más en profundidad todo en la [documentación oficial de migasfree](https://fun-with-migasfree.readthedocs.io/es/master/).

Ésta parte del curso pretende aclarar un poco más como se lleva a cabo el proceso de comunicación entre los equipos <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Vitalinux</tt></span> y el servidor <b>Migasfree</b>, sin entrar en detalles complejos o de programación.

## Análisis de la comunicación con el Servidor Migasfree {#AnalisisComunicacionMigasFree}

Cada vez que el equipo inicia una sesión gráfica, si éste tiene comunicación con Internet y el servidor Migasfree está activo, comienza una comunicación entre el cliente Migasfree, <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Vitalinux</tt></span>, y el <b>servidor Migasfree</b>.

No obstante, antes de establecerse propiamente la comunicación con el servidor Migasfree, el sistema realiza una serie de comprobaciones/acciones, como por ejemplo:

-  Comprobar si hay acceso a Internet (*para conectar después con Migasfree*)
-  Comprobar si hay conexión con el servidor caché que se coloca en los centros educativos (*para poder usarlo a posteriori*)
-  Intentar reparar instalaciones de software que se quedaron a mitad o rotas en sesiones anteriores
-  ...

Después se lanza propiamente la comunicación con el servidor Migasfree. A continuación se analizará que ocurre en dicha comunicación y como forzar para que se realice en cualquier otro momento.

### Interfaz {#Interfaz}

Como hemos dicho, cuando la máquina arranca se desencadena el proceso anterior. Podemos ver que se está ejecutando a través del icono de la barra inferior de tareas. Si aparece el **triángulo verde** significa que se están realizando acciones en ese momento y que no se ha terminado la comunicación con el servidor Migasfree:

![Migasfree client - Actualizando](../img/parte5/migasfreeclient-play.png "Migasfree Client - Ejecución")

Una vez haya terminado todo el proceso (*comprobaciones y posterior comunicación con el servidor*) podremos advertir que el icono referente a **Migasfree** cambia:

![Migasfree client - Finalizado](../img/parte5/migasfreeclient-end.png "Migasfree Client - Terminado")

También podemos encontrarnos con otros iconos que nos indiquen otras situaciones: *es necesario reiniciar*, *se ha detectado un problema*, etc.  En el caso de visualizar estos otros iconos, podremos pulsar sobre dicho icono para que nos de más información.


Igualmente, si pulsamos sobre el **icono de Migasfree** podremos ver otras opciones como son:

-  **Volver a lanzar el proceso de actualización**
-  **Información Global** del equipo
-  **Wiki** Acceder a la documentación oficial de Vitalinux
-  **Conocer nuestra identificación**. El número que identifica al equipo de forma unívoca y que aparece en el Widget del escritorio como CID
-  **Ver la consola** (*detalles*)

![Migasfree client - opciones](../img/parte5/migasfreeclient-options.png "Migasfree Client - Menú de Opciones")

### Análisis de la comunicación entre el Cliente y Servidor Migasfree {#AnalisisComunicacionClienteServidor}

A continuación veremos en detalle el proceso de comunicación entre nuestro Vitalinux (*cliente Migasfree*) y el servidor Migasfree. En concreto, una vez que se conecta con el servidor Migasfree se desencadenan las siguientes acciones:

**(1) Conectando al servidor migasfree...**

En primer lugar se comprueba que hay **conectividad** con el servidor migasfree, **migasfree.educa.aragon.es**.

**(2) Obteniendo propiedades... / Evaluando atributos... / Subiendo atributos...**

El servidor Migasfree le dice que le tiene que facilitar una información: **PROPIEDADES**. El cliente (*Vitalinux*) recopila dicha información en relación a propiedades que lo caracterizan (*el valor de la propiedad se llama **atributo**, y son **características software y hardware***), y que le permiten al servidor **identificarlo y clasificarlo**.

**(3) Ejecutando fallas... / Subiendo fallas...**

En el lado del servidor se programan **pequeños programas** llamados **"fallas"**. Estas fallas se asignan a los equipos en función de sus propiedades, atributos o etiquetas (*recordaremos que es una **Etiqueta Migasfree** en la siguiente sección*). De esta forma, en función de la información recolectada en el paso anterior, y la que ya tiene Migasfree en su base de datos decide cual de estas fallas se ejecutan en el equipo cliente. Las fallas permitirán cosas como:

-  **Realizar comprobaciones**: si no queda espacio en disco, si hay errores en instalación
-  **Arreglar pequeños Bugs**
-  **Aplicar configuraciones**: cambiar fondo de Escritorio, crear Accesos directos en el Escritorio a determinadas aplicaciones, crear archivos y directorios, etc.
-  **Configurar impresoras**
-  **Gestionar contraseñas de usuarios**
-  '*Gestionar contraseñas de redes Wireless*
-  .... ¡¡¡Cualquier cosa que nos queramos imaginar cuyo procesamiento requiera menos de un par de minutos!!!

**(4) Creando repositorios... / Obteniendo los metadatos de los repositorios...**

Un repositorio es un sitio centralizado en Internet donde se almacena software disponible para ser instalado en un equipo. El servidor Migasfree en función de las propiedades, atributos y etiquetas del equipo le asocia unos repositorios u otros para que su software asociado **este disponible**.

**(5) Desinstalando paquetes... / Instalando paquetes obligatorios... / Actualizando paquetes...**

En este punto, el servidor Migasfree da la orden al equipo cliente de desinstalación, instalación y actualización del software que se le haya indicado previamente a Migasfree. De ésta forma el equipo:

-  Tendrá el software actualizado (se corrigen errores y se mejora la funcionalidad)
-  Tendrá el software base que se le especificó
-  No tendrá el software que no queremos que tenga
*¿Podremos instalar otro software o quitar software que no queramos?* **POR SUPUESTO** (*si tenemos permisos de administrador sobre la máquina*). Con lo anterior solo forzamos a un perfil de software BASE. 

**(6) Subiendo el historial del software... / Subiendo el inventario del software...**

Por último, el servidor Migasfree registra o inventaria el cambio que se haya podido producir en el software instalado en el equipo, de tal forma que a posteriori se puede saber que ha sucedido con los programas disponibles en el equipo.

### Forzar Actualización contra Migasfree {#ActualizacionContraMigasfreConsola}

A modo de curiosidad, para actualizar el equipo contra migasfree de una manera expicita, sin tener que esperar al próximo reinicio e inicio de sesión gráfica, deberemos llevar a cabo una de las dos siguientes acciones:

* De manera gráfica: pinchando sobre el <b>icono de Migasfree</b> situado en la parte derecha de la barra o panel del entorno de Escritorio y seleccionar la opción de <b>Forzar actualización</b>.

![Migasfree client - Fozar Actualización](../img/parte5/migasfreeclient-forceupgrade.png "Migasfree Client - Forzar Actualización")

* Desde la línea de comandos abriendo una terminal (<i>CONTROL+ALT+T</i>) y tecleando lo siguiente:

```bash
$ sudo migasfree --update
# migasfree -u
```

## Etiquetas Migasfree {#EtiquetasMigasfree}

### ¿Qué son y para qué sirven las etiquetas Migasfree? {#EtiquetasMigasfree}

Las etiquetas Migasfree son utilizadas para clasificar los equipos según un criterio personal/de centro. Por ejemplo, mediante estas etiquetas podemos etiquetar a un equipo para que quede asociado a un centro educativo específico, para saber si el usuario que va a usar dicho equipo es un estudiante o un docente o para indicar que el equipo requiere de algún tipo de servicio específico (*carpetas compartidas, congelación del Escritorio, etc.*).


De esta forma, haciendo uso de estas etiquetas podemos distinguir a los equipos por centro al que pertenecen e instalar únicamente el software solicitado por dicho centro. Podemos además tener **etiquetas jerarqueizadas**, de forma que podemos agrupar los equipos de forma más lógica y sencilla. Por ejemplo, podríamos tener un centro con las siguientes necesidades:

- Una etiqueta para todos los equipos del centro (supongamos que de Primaria): PRI-MICENTRO
- Otra etiqueta para identificar a los equipos de un departamento: PRI-MICENTRO.INGLES
- E incluso una para identificar un aula (son ejemplos, cada centro decide su estructura): PRI-MICENTRO.INGLES.AULA1

De ésta forma, simplemente etiquetando a un equipo como **PRI-MICENTRO.INGLES.AULA1**, ya no hace falta etiquetarlo como de **INGLES** o de **MICENTRO** ... automáticamente le afectarán las condiciones que hayamos definido para esos grupos.


{% notificacion_alert title='¿Cuántas etiquetas Migasfree puede tener asignadas mi equipo?', logotext='¡¡Aclaración!!' %}
Un equipo puede tener asignadas multiples etiquetas mientras no entren en conflicto entre ellas, aunque sean redundantes.  Es decir:
<ol> 
<li>
Un equipo <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Vitalinux</tt></span> puede tener asignadas dos etiquetas de dos centros educativos (<i>p.e. dos etiquetas de dos centros de primaria PRI-CENTRO1 y PRI-CENTRO2), pero si por un casual el <b>CENTRO1</b> ha demandado forzar la desinstalación de un programa que si ha requerido el <b>CENTRO2</b>, cada vez que el equipo inicie sesión, tras conectarse contra Migasfree se estará desinstalando e instalando de nuevo ese software.
</li>
<li>
Un equipo puede tener marcadas las etiquetas <b>PRI-MICENTRO</b>, <b>PRI-MICENTRO.INGLES</b>, y <b>PRI-MICENTRO.INGLES.AULA1</b>, aunque es altamente redudante, ya que simplemente marcando la última, <b>PRI-MICENTRO.INGLES.AULA1</b>, ya esta diciendo a Migasfree que tiene implicitamente también las dos primeras.
</li>
</ol>

{% endnotificacion_alert %}



### Asignación de Etiquetas Migasfree {#AsignacionEtiquetasMigasfree}

Tras la instalación de Vitalinux en un equipo y en el caso de que haya conexión con Internet, la primera vez que se inicie en ese equipo una sesión gráfica se ejecutara una breve post instalación a través de la cual podremos asignarle al equipo las etiquetas que deseemos

Entre las muchas etiquetas disponibles deberemos tener en cuenta lo siguiente para su asignación:

-  **SRV-CONGELARESCRITORIO:** Esta opción mantendrá el escritorio congelado para evitar que los usuarios guarden o modifiquen cosas en él. Dicha congelación se basa en la comparación entre lo que hay en el escritorio del usuario y un patrón que se localiza en /etc/skel/Desktop/, de tal forma que todo aquello que haya de más respecto al patrón es eliminado. Por tanto, para añadir cosas al Escritorio será necesario modificar el patrón.
-  **SRV-CONGELADORTOTAL:** Esta opción mantendrá congelado tanto el escritorio como el resto de directorios del perfil del usuario (Documentos, Imágenes, etc.). Dicha congelación se basa en la comparación entre lo que hay en los directorios del perfil del usuario y un patrón que se localiza en /etc/skel-directorios-congelados/, de tal forma que todo aquello que haya de más respecto al patrón es eliminado. Por tanto, para añadir cosas a los directorios del perfil del usuario será necesario modificar el patrón.
-  **SRV-CARPETASCOMPARTIDAS**: Esta opción permite tener acceso a varias carpetas compartidas por el servidor caché que se localiza en los centros.
-  **SRV-NAVEGADORINCOGNITO:** Esta etiqueta modificará el comportamiento de nuestros navegadores web (firefox y chrome), provocando que se incien en modo incógnito.
-  **SRV-GIR-VIRTUALIZADO:** Esta etiqueta instalará la aplicación GIR, pero requiere de un equipo que soporte Virtualización. 
-  **SRV-VIRTUABOX:** Esta etiqueta modificará instalará el software necesario para poder ejecutar máquinas virtuales con VirtualBox.
-  **SRV-CONTROL-EQUIPOS-******: Esta etiqueta sirve para desplegar un servicio de control y herramientas de comunicación de aula con epoptes.
-  **PRI/SEC-”Nombre del centro”:** Esta etiqueta permite indicar a qué centro pertenece el equipo, para que este pueda descargar el software y los recursos que le corresponden de una manera personalizada.

Estas etiquetas podrán ser modificadas en cualquier momento si se desea, para ello deberemos ir a **Inicio → Vitalinux → Migasfree → Modificación de Etiquetas Migasfree**, o más fácilmente tecleando <b>CONTROL+ESPACIO</b> y escribir <b>Modificar etiquetas Migasfree</b>.

![Modificar Etiquetas Migasfree](../img/parte5/modificar-etiquetas-migasfree.png "Es posible modificar las etiquetas Migasfree en cualquier momento")

{% notificacion_alert title='¿Cuál es el etiquetado perfecto?', logotext='¡¡Aclaración!!' %}

Por lo general, si un centro ha realizado una correcta planificación del etiquetado, con marcar una única etiqueta ya es suficiente, y asociar a dicha etiqueta todas las acciones que quiere programas sobre ese equipo.  Por ejemplo, un equipo puede tener asignado una etiqueta denominada <b>SEC-MICENTRO.AULAINF.SALA1</b> y estar configurado el servidor Migasfree para que todo equipos que tenga dicha etiqueta se le configure los siguiente:
<ul>
<li>Lista de programas a instalar y desintalar</li>
<li>Usuario con el que iniciará la sesión gráfica de manera automática</li>
<li>Lista de cuentas de usuario y perfiles que debe tener configuradas el equipo (<i>con perfil de inglés para clases de inglés, frances, etc.</i>)
<li>Hora de apagado</li>
<li>Páginas de inicio que deberían mostrar los navegadores Web al iniciarse</li>
<li>Lista de extensiones que deberían instalarse en los navegadores Web</li>
<li>Impresoras que deberían configurarse en el equipo</li>
<li>Acceso a determinados libros digitales</li>
<li>etc.</li>
</ul>

{% endnotificacion_alert %}

### Comprobación de Etiquetas Migasfree {#ComprobacionEtiquetasMigasfree}

Al igual que podemos asignar las etiquetas mediante el ejectuable Modifiación de Etiquetas, podemos comprobar las etiquetas que tenemos con **Consultar y Comprobar Etiquetas Migasfree**

![Comprobar Etiquetas Migasfree](../img/parte5/tags-consultar.png "Podemos consultar las etiquetas asignadas a nuestro equipo")

### Consideración especial {#ConsideracionEspecial}

Existe una etiqueta "especial", y es la denominada **ENT-CASA**. Dicha etiqueta se creó con la idea de que alguien pueda usar Vitalinux en casa, pero quiera tener un "perfil" similar al de un centro. Pero si marcamos dicha etiqueta se desencadenarán algunas acciones importantes a tener en cuenta:

-  No será posible acceder al equipo de forma remota para soporte sin intervención, de forma que garantizamos su privacidad
-  No se tendrán en cuenta ciertas acciones como el cambio de passwords u otras que afecten a un centro de forma carácterística.

## Habilitar o deshabilitar el cliente

El cliente migasfree se arranca como hemos dicho de forma automática cada vez que arrancamos la máquina o iniciamos sesión. Es posible que nos interese en un momento dado deshabilitar ésta característica ya que por ejemplo estamos de viaje y no queremos consumir datos de nuestra conexión 3G, o nuestra red va muy lenta o por cualquier otro motivo. Para éstos casos podemos deshabilitar el cliente simplemente ejectuando CTRL-ESPACIO + Habilitar Deshabilitar...

![Habilitar o deshabilitar el cliente Migasfree](../img/parte5/enable-disable-migasfree.png "Podemos habilitar o dehabilitar el cliente Migasfree")

Mientras el equipo tenga deshabilitado el cliente, NO se recibirán actualizaciones de software, no se podrá actuar de forma automática y desatendida, y no se recibirán los errores que se produzcan.

***Recuerda pues habilitarlo de nuevo para tener éstas funcionalidades*** simplemente ejecutando de nuevo el programa.

{% notificacion_important title='¡Migasfree nos facilita la reconstrucción del equipo!' %}
Además de facilitarnos <b>Migasfree</b> la configuración de todo lo anterior, también nos facilitará en un futuro el que tengamos que formatear el equipo.  Es decir, <b>Migasfree</b> registra a los equipos quedandose con el identificador de su placa base, un identificador que es único para todo equipo (<i>sería como el DNI de los equipos, a nivel mundial</li>), lo que hace que cuando un equipo se tenga que formatear e instalar <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Vitalinux</tt></span>, éste será recordado por Migasfree y le asignará de manera automática la etiqueta Migasfree que ya tenía y toda su configuración asociada. De esta forma, <b>¡¡¡reconstruir un equipo ante un desastre es cuestión de minutos!!!</b>
{% endnotificacion_important %}

## Video formativo

Puedes encontrar mas información en la **Píldora formativa del cliente migasfree**:

{% youtube %}https://youtu.be/dz06XQ1J2h0{% endyoutube %}