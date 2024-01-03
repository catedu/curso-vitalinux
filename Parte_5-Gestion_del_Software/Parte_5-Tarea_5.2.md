{% notificacion_task title='Gestión de Software a través de Migasfree',
numexer='5.2',
req='Es necesario haber leído todo lo referente al <a href="./Parte_5-Cliente_migasfree.html">Cliente Migasfree</a>, y su <a href="./Parte_5-Gestion_del_software_mediante_migasfree.html">Gestión remota y desatendida</a>',
formatoentrega='En un documento ofimático escribe y pega las fotos o capturas de pantalla necesarias para justificar todo lo que se te pide a continuación. Si es posible expórtalo a <b>formato PDF</b> para garantizar su portabilidad, y adjúntalo como respuesta a la tarea solicitada. Por tanto, envía al tutor un único archivo <b>.pdf</b> que se nombrará siguiendo las siguientes pautas: <b>apellido1_apellido2_nombre_TareaX.pdf</b>.
<br>
Asegúrate que el nombre no contenga la letra ñ, tildes ni caracteres especiales extraños. Así por ejemplo la alumna <b>Begoña Sánchez Mañas</b>, debería nombrar esta tarea como: <b>sanchez_manas_begona_Tarea5.2.pdf</b>' %}

Para terminar con esta parte del curso de iniciación a <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Vitalinux</tt></span> asociada a la <b>Gestión del Software</b> veremos la capacidad que tiene <b><span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Migasfree</tt></span></b> para controlar todo su software.  Como ya se ha dicho en múltiples ocasiones, la característica más importante de <b>Vitalinux</b>, y que le diferencia del resto de distribuciones Linux actuales, es que incorpora un <b>cliente <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Migasfree</tt></span></b>.  En concreto, este <b>cliente <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Migasfree</tt></span></b> garantiza que cada vez que arranca <b>Vitalinux EDU DGA</b>, tras iniciar sesión, se establece una comunicación con el servidor <a href="http://migasfree.educa.aragon.es">migasfree.educa.aragon.es</a> del programa de <b>Software Libre</b> de la DGA, y a través de dicha comunicación Vitalinux deja en manos de <b><span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Migasfree</tt></span></b> todo su software para que éste último decida que hacer (<i><span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Migasfree</tt></span> provocará en el equipo Vitalinux todo aquello que se le haya encomendado previamente</i>).  A grandes rasgos, <b><span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Migasfree</tt></span></b> tiene identificado al equipo Vitalinux en base a un identificador unívoco llamado CID (<i><b>Computer ID</b> que puede consultarse a través del Widget del Escritorio</i>), y a un conjunto de <b>Etiquetas <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Migasfree</tt></span></b> que se le pueden asignar.
<br>
En concreto, mediante la realización de la siguiente tarea se pretende comprender un poco mejor la forma en que se comunica <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Vitalinux</tt></span> con <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Migasfree</tt></span> y la posibilidad de personalización del equipo en función de las etiquetas <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Migasfree</tt></span> asignadas:
<br><i>Nota:Para la realización de ésta tarea es imprescindible que el equipo tenga conexión a Internet, ya que nos estamos comunicando con el servidor migasfree del proyecto</i>
<ol>
<li>
<b>Cliente <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Migasfree</tt></span></b>. Una vez se inicia sesión en Vitalinux abre la <b>consola del cliente <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Migasfree</tt></span></b> y observa los mensajes que se producen. Para poder moverte con el <b>"scroll"</b> (<i>arriba y abajo</i>) deberás esperar a que termine el proceso.  Durante la sincronización con Migasfree se ejecutan un conjunto de scripts/programas/fallas que lo personalizan, y se instalan/desinstalan/actiualizan programas/software.  La ejecución de las fallas y la actualización del software del sistema se lleva a cabo durante el primer inicio de sesión gráfico que se realice a lo largo del día.  Si tu equipo Vitalinux arranca a lo largo del día más de una vez, por defecto, omitirá las acciones anteriores.  Para fozar todas estas acciones de forma manual debes pinchar con el botón del ratón sobre el icono de Migrasfree ubicado en el panel inferior y elegir la opción referente a forzar una actualización contra Migasfree.  Haz dos capturas de pantalla correspondientes a:
</li>
    <ol type="A">
    <li>
    Cuando se ejecuta a través de <b><span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Migasfree</tt></span></b> la falla <b>CONF-SOFT-LIBREOFFICE</b> encargada de configurar aspectos de personalización de Libreoffice.
    </li>
    <li>
    Cuando <b><span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Migasfree</tt></span> da la orden de actualizar el software del sistema</b>.
    </li>
    </ol>
<li>
Comprobación de <b>Etiquetas <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Migasfree</tt></span></b>. Comprueba que etiquetas asignaste cuando hiciste la post-instalación. Si no marcaste ninguna, lo cual es posible al marcar que ibas a usar el equipo fuera del entorno educativo, estará marcada la etiqueta de <b>ENT-CASA</b>. Haz una captura de pantalla con dicho listado. Más tarde asignaremos otra para instalar software.  <b>Importante</b>: Si sólo quieres conocer las <b>etiquetas Migasfree</b> del equipo puedes teclear <b>CONTROL+ESPACIO</b> y teclear <b>Consultar y comprobar etiquetas migasfree</b>, pero si quieres tener una información más completa de la configuración de red y etiquetado <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Migasfree</tt></span> de tu Vitalinux puedes teclear <b>CONTROL+ESPACIO</b> y escribir <b>Información Global del Sistema</b>
</li>

<li>
Por último se propone asignar una nueva <b>etiqueta Migasfree</b> a tu equipo Vitalinux y ver que efectos le provoca:
</li>
<ol type="A">
<li>
Asegurate de que tu equipo Vitalinux ha terminado la comunicación con <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Migasfree</tt></span> (<i>tiene que desaparecer el <b>triángulo verde</b> que aparece tras iniciar sesión sobre el símbolo de <b><span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Migasfree</tt></span></b> que encontrarás en la parte derecha de la barra/panel inferior del Entorno de Escritorio de Vitalinux</i>)
</li>
<li> Modifica la lista de <b>Etiquetas <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Migasfree</tt></span></b> que tiene asignadas tu equipo Vitalinux. Para ello pulsa <b>"CONTROL + ESPACIO"</b> y teclea <b>"Modificar Etiquetas ..."</b>.  Podrás comprobar que te habrá aparecido una ventana con una lista de etiquetas posibles a asignar.  Añade a las que ya tengas seleccionadas una específica del curso llamada <b>"PER-AULARAGON"</b>.  Para que se vea algo del potencial, podrás observar que la asignación de esta etiqueta va a provocar que:
</li>
    <ul>
    <li>
    En el Escritorio del usuario aparezcan tres nuevas carpetas
    </li>
    <li>
    Que se instalen nuevas aplicaciónes para las prácticas posteriores, y una por ejemplo llamada <b>Calibre</b> pensada para el tratamiento de e-books
    </li>
    <li>
    Que se haya instalado una extensión en o chromium-browser o google-chrome (por defecto se instala chromium-versión libre de Google Chrome) llamada screencastify, que te puede permitir hacer videotutoriales. Depués de un primer arranque del navegador, puede tardar en aparecer la extensión (mientras se instala por primera vez).
    </li>
    </ul>
<li>
Comprueba el efecto de la asignacióna anterior, advirtiendo que te han aparecido tres carpetas nuevas en el Escritorio y que dispones de esta nueva aplicación: <b>"CONTROL + ESPACIO"</b> y teclea <b>"Calibre ..."</b>
</li>

</ol>

</ol>


{% endnotificacion_task %}
