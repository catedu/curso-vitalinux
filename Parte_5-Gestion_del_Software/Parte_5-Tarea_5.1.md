{% notificacion_task title='Gestión de Software en Vitalinux',
numexer='5.1',
req='Es necesario haber leído todo lo referente a gestión del software en Vitalinux mediante <a href="./Parte_5-Gestor_de_software_synaptic.html">Synaptic</a>, <a href="./Parte_5-Aplicaciones_windows_sobre_vitalinux.html">Wine y PlayOnLinux</a>',
formatoentrega='En un documento ofimático escribe y pega las fotos o capturas de pantalla necesarias para justificar todo lo que se te pide a continuación. Si es posible expórtalo a <b>formato PDF</b> para garantizar su portabilidad, y adjúntalo como respuesta a la tarea solicitada. Por tanto, envía al tutor un único archivo <b>.pdf</b> que se nombrará siguiendo las siguientes pautas: <b>apellido1_apellido2_nombre_TareaX.pdf</b>.
<br>
Asegúrate que el nombre no contenga la letra ñ, tildes ni caracteres especiales extraños. Así por ejemplo la alumna <b>Begoña Sánchez Mañas</b>, debería nombrar esta tarea como: <b>sanchez_manas_begona_Tarea5.1.pdf</b>' %}

En la presente tarea repasaremos como <b>instalar y desinstalar aplicaciones</b> nativas de Linux y Windows (si fuera necesario...pero hay que considerar alternativas libres siempre!) mediante <b>Synaptic</b>, <b>Vitalinux Play</b> y/o <b>Wine</b>.  Para ello seguiremos los siguientes pasos:
<br><br>
<ol>

<li>
Gestión de Software desde <b>Vitalinux Play</b>. Recuerda que para instalar apliaciones mediante Vitalinux Play deberás tener conexión a Internet.  Abre la aplicación <b>Vitalinux Play</b>, busca aplicaciones por <b>nivel educativo</b> indicándolo en el campo de búsqueda (<i>primaria, secundaria, bachillerato, etc.</i>), o por <b>área de conocimiento</b> (<i>matemáticas, música, tecnología, etc.</i>), e instala/desinstala alguna de las aplicaciones filtradas.  Comprueba lo cómodo que instalar y desinstalar software desde este almacén.
Nota: El listado completo de todas las aplicaciones disponibles en Vialinux Play lo puedes encontrar la web de documentación del proyecto Vitalinux (<a href="https://docs.vitalinux.educa.aragon.es/recursos/Apps.html#aplicaciones-disponibles-en-vitalinux-play">Apps Vitalinux Play</a>).
</li>

<br><br>

<li>
<b>Synaptic</b> es una otra aplicación que permite gestionar el software (<i>instalar y desinstalar aplicaciones</i>). Igualmente es necesario tener conexión a Internet.  A modo de ejemplo, en la presente tarea se propone instalar una aplicación como el editor de audio <b>audacity</b> o la pizarra virtual <b>openboard</b>. Podrías instalar con Vitalinux Play, pero lo vas a probar con Synaptic para ver la diferencia y porque todo no está en Vitlainux Play. Para ello:
</li>

<ul>
<li>
Asegurate de que tu equipo Vitalinux ha terminado la comunicación con Migasfree, en el caso de que se haya iniciado una sincronización con él (<i>tiene que desaparecer el <b>triángulo verde</b> que aparece tras iniciar sesión en Vitalinux sobre el símbolo de <b>Migasfree</b> que encontrarás en la parte derecha de la barra/panel inferior del Entorno de Escritorio de Vitalinux</i>)
</li>
<li>
Accede a <b>Synaptic</b> (<i><b>CONTROL+ESPACIO</b> y tecleas <b>synaptic</b></i>)
</li>
<li>
Pulsa sobre el botón <b>"Recargar"</b> de <b>Synaptic</b> para actualizar el software disponible en los repositorios u origenes de software configurados en Vitalinux
</li>
<li>
Busca <b>audacity (u openboard)</b> a través de <b>Synaptic</b>
</li>
<li>
Una vez localizado pincha con el botón derecho del ratón sobre él y selecciona la opción <b>instalar</b>
</li>
<li>
Por último pincha sobre el botón <b>Aplicar</b> para que se apliquen los <b>cambios solicitados a Synaptic</b>, y cierralo.
</li>
<li>
Para terminar, abre <b>Audacity (u Openboard)</b> (<i><b>CONTROL+ESPACIO</b> y tecleas <b>audacity</b></i>) y prueba la aplicación
</li>
<li>
Con el fin de repasar el <i><b>Cómo desinstalar aplicaciones</b></i>, vuelve a abrir <b>synaptic</b> y desinstala la aplicación anterior.  Para ello buscala mediante su buscador, pincha con el botón derecho sobre ella y elige la opción de <b>desintalar</b>.  Al igual que al instalar, será necesario darle al botón <b>Aplicar</b> para que surta efecto la desintalación.
</li>
<!-- <li>
Como en ocasiones <i>más vale un buen videotutorial que mil palabras</i> a continuación se sugiere ver el siguiente vídeo relacionado con este asunto (<i>es una parte del videotutorial completo: <a href="https://www.youtube.com/watch?v=8tBh8yz1FHY%7C">Gestión del Software en Vitalinux</a><i>):
<br>
<div style="text-align: center;">
<iframe width="560" height="315" src="https://www.youtube.com/embed/1nni5ikg11Q" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>
</li> -->
</ul>

<br><br>
<li>
Tal como se ha explicado en la parte teórica <b>WinE</b> surge con la finalidad de facilitar al usuario final el paso de <b>Microsoft Windows</b> a <b>Linux</b> permitiéndonos la instalación y ejecución de programas creados para Windows en nuestro sistema operativo Linux/Vitalinux. De esta forma, en caso de no encontrar ninguna alternativa en software libre a las aplicaciones privativas que usamos en Windows (<i>siempre es aconsejable buscar software alternativo de código libre/abierto</i>), gracias a Wine, vamos poder instalar y trabajar con nuestra aplicación Windows. A modo de ejemplo, como tarea se propone instalar un programa de Windows en Vitalinux:
</li>
<ol type="A">
<li>
Localiza algún instalador de alguna aplicación Windows (*.exe) con la que estés muy familiarizado, del que no encuentras una alternativa libre en Vitalinux, y que por tanto, te gustaría instalar en Vitalinux. En el caso de no disponer de ningún instalador te proponemos a modo de ejemplo <a href="https://migasfree.educa.aragon.es/cosas-centros/windows-software/mecanet/mecanet-24-04-18.zip">Mecanet</a> (<i>aplicación para aprender mecanografía, su última versión sólo disponible para Windows</i>), <a href="https://migasfree.educa.aragon.es/cosas-centros/windows-software/sebran/sebran.zip">Sebran</a> (<i>12 juegos infantiles para la iniciación a lectoescritura y matemáticas</i>), <a href="https://migasfree.educa.aragon.es/cosas-centros/windows-software/tinycad/TinyCAD_3.00.02.zip">TinyCAD</a> (<i>diagramas de circuitos electrónicos</i>), <a href="https://migasfree.educa.aragon.es/cosas-centros/windows-software/CROCCLIP/CROCCLIP.zip">crocodile</a> (<i>simulación circuitos electrónicos</i>), <a href="https://migasfree.educa.aragon.es/cosas-centros/windows-software/relatran/setup.zip">relatran</a> (<i>simulador de mecanismos</i>) o <a href="https://migasfree.educa.aragon.es/cosas-centros/windows-software/convertall/convertall-0.8.0-install-user.zip">convertall</a> (<i>conversor entre magnitudes físicas</i>) [<i>Una vez descargado el archivo ZIP lo podrás descomprimir, y extraer el archivo ejecutable .exe, pinchando con el botón derecho del ratón sobre el fichero ZIP y seleccionado la opción de descomprimir</li>].
</li>
<li>
Pincha con el botón derecho del ratón sobre el archivo instalador anterior e indica que quieres abrirlo con <b>WinE</b> (<i>Cargador de programas de Windows</i>) o lo puedes lanzar también con doble-click. Comprobarás que a continuación se configurará Wine (acepta si te pide instalar complementos o librerías adicionales) y comenzará su instalación al estilo Windows (<i>siguiente, siguiente, siguiente, ...</i>). Es decir, instala la aplicación como si estuvieras en Windows.
</li>
<li>
Abre la aplicación como cualquier otra. Por ejemplo, <b>CONTROL+ESPACIO</b> y teclear el nombre de la aplicación (<i>sebran, crocodile, tinyCAD, etc.</i>). Es posibles que los iconos no se hayan actualizado o no aparezcan en el momento y necesite reiniciarse el equipo o reinciar la sesión gráfica. Comprueba el correcto funcionamiento de la aplicación Windows sobre Vitalinux.
</li>
<li>
Como cualquier otra aplicación de Vitalinux, para cerrarla puedes teclear: <b>ALT+F4</b>
</li>
</ol>
</ol>

<br><br>
Llegado este punto habrás advertido que <b>WinE</b> nos permite la instalación de aplicaciones Windows en Linux, pero presenta algunos inconvenientes entre los cuales cabría destacar los siguientes:
<li>
A priori, <b>Wine no nos garantiza un 100% de probabilidad de que una aplicación Windows se instale de manera exitosa sobre Linux</b>. En ocasiones la aplicación Windows que queremos instalar depende de algún parche de Windows (<i>Service Pack</i>) o librería que no esta disponible en nuestro Wine provocando una instalación fallida.
</li>
<li>
<b>Determinadas aplicaciones Windows requieren una determinada versión de Wine (<i>1.6, 1.7, 2...</i>) para funcionar</b>. Esto es un gran problema, ya que a priori sólo podemos tener instalada una única versión de Wine.
</li>
<li>
Para instalar una aplicación sobre Wine previamente tenemos que buscarla por Internet, fiarnos de ella, y descargarla. En ocasiones, el software de Windows que nos descargamos esta <b>infectado</b> o realiza acciones que desconocemos afectando al correcto funcionamiento de nuestro sistema.
</li>

</ol>
{% endnotificacion_task %}
