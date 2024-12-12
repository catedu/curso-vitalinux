{% notificacion_important title='¡Qué importantes son la RAM y CPU!' %}
De todas las características hardware de un equipo hay dos que merece la pena señalar por las siguientes razones:

<ol>
<li><b>RAM</b>: Cuando lanzamos/abrimos una aplicación o programa (p.e. firefox, libreoffice, gimp, etc.) este se copia del disco duro a la memoria RAM del ordenador, para posteriormente ser leida y ejecutada por el procesador o CPU del equipo.  Es decir, nuestra CPU nunca lee los programas a ejecutar directamente del disco duro sino de la memoria RAM, ya que esta última es mucho más rápida y por tanto mucho más eficiente.  Según esto, a medida que vamos abriendo aplicaciones estas se van copiando en memoria RAM y la van agotando.  Por esta razón, <b>la cantidad de memoria RAM determina la cantidad de programas que pueden ser ejecutados simultáneamente garantizando fluidez en su rendimiento</b>.  En el momento en que la memoria RAM se llena, para poder seguir abriendo aplicaciones es necesario intercambiar o llevar parte de su contenido al disco duro provocando de esta forma un decremento en su rendimiento de manera notable apreciando perdida de fluidez y de tiempo de respuesta.  A medida que se cierran aplicaciones abiertas estas son eliminadas de la memoria RAM dejando espacio libre para que posteriormente pueda ser ocupado por otras aplicaciones que sean lanzadas/abiertas.
<br>
Además, al hilo de todo lo anterior, podemos deducir que la rapidez de nuestro disco duro determinará lo rapidez con que se copia en memoria RAM y empieza a ejecutarse el programa por parte de la CPU.  Por esa razón, el uso de discos duros SSD (<i>de estado sólido, no mecánicos</i>) garantiza que las aplicaciones se carguen más rápidamente proporcionando una sensación de fluidez mucho mayor.
</li>
<li><b>CPU o procesador</b>: Es el elemento principal de un ordenador. Su velocidad de computo y potencia de procesamiento determinará lo rápido que se leen y ejecutan los programas que se han cargado en memoria RAM, determinando el rendimiento global del sistema. Mientras que los procesadores de baja gama (<i>Pentium, Atom, Celeron, AMD-E, etc.</i>) disparan su consumo y se saturan a poco que se les pide, los procesadores de alta gama (<i>i3, i5, i7, etc.</i>) son capaces de ejecutar aplicaciones pesadas sin alcanzar el 50% de su potencia. En concreto, el consumo de CPU se incrementa cuando lanzamos/abrimos una aplicación y cuando realizamos acciones o cambios en la aplicación ya abierta. Si las aplicaciones están abiertas pero en reposo (<i>el usuario no lleva a cabo ninguna acción</i>) la CPU estará totalmente ociosa.
</li>
Según todo lo anterior, y a modo de reflexión, cabría señalar que muchos de los modelos de mini portátiles que se repartieron en centros educativos hace más de una decada bajo el amparo del <b>programa Escuela 2.0</b> tienen un CPU muy flojita (<i>Atom</i>) y poca memoria RAM (<i>512/1024MB</i>), lo que provoca que se saturen en seguida.  Cambiar el disco duro HDD que incorporan por un SSD y ampliar su memoria RAM aportará mejoras en el arranque del sistema operativo, en la respuesta del equipo al lanzar aplicaciones y permitirá tener más aplicaciones abiertas sin penalizar en su rendimiento, pero siempre habrá que ser conscientes de que la CPU o procesador, al no poderse cambiar/mejorar, es el que es y se seguirá atragantando/saturando ante aplicaciones pesadas o que demanden mucho computo.
</ol>
{% endnotificacion_important %}

{% notificacion_task title='Lanzar Aplicaciones y efecto sobre la RAM y CPU del Sistema',
numexer='3.2',
req='Es necesario disponer de un equipo físico o virtual con Vitalinux instalado, además de haber leido los apartados referentes a <a href="../Parte_3-Entorno_de_Escritorio/Parte_3-Como_lanzar_aplicaciones.html">Cómo lanzar Aplicaciones</a> e información del <a href="../Parte_3-Entorno_de_Escritorio/Parte_3-Preferencias_del_escritorio.html">Widget del Escritorio</a>',
formatoentrega='En un documento ofimático escribe y pega las fotos o capturas de pantalla necesarias para justificar todo lo que se te pide a continuación. Si es posible expórtalo a <b>formato PDF</b> para garantizar su portabilidad, y adjúntalo como respuesta a la tarea solicitada. Por tanto, envía al tutor un único archivo <b>.pdf</b> que se nombrará siguiendo las siguientes pautas: <b>apellido1_apellido2_nombre_TareaX.pdf</b>.
<br>
Asegúrate que el nombre no contenga la letra ñ, tildes ni caracteres especiales extraños. Así por ejemplo la alumna <b>Begoña Sánchez Mañas</b>, debería nombrar esta tarea como: <b>sanchez_manas_begona_Tarea3.2.pdf</b>' %}

Como tarea te proponemos repasar algunas de las formas descritas para <b>lanzar aplicaciones</b>, y al mismo tiempo aprovechar para conocer que efecto tiene esto sobre <b>la CPU y la RAM</b> del sistema operativo <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Vitalinux</tt></span> gracias a la información suministrada por el <b>Widget</b> ubicado en el Escritorio.  En concreto se sugiere realizar las siguientes acciones:
<br>
<span style='font-size: 75%;font-weight:bold;font-style:italic'; font-size: 120%;>Nota sobre las capturas a presentar: No es necesario que presentes las capturas de cómo lanzas las aplicaciones usando los diferentes métodos propuestos...de hecho en algún caso será incompatible que lances la aplicación y a la vez tomes la captura de la pantalla</span>
<ol>
<li>
Inicia sesión gráfica en <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Vitalinux</tt></span>, espera a que finalice la comunicación con <b>Migasfree</b> (<i>el icono de Migasfree que hay en la parte derecha del panel del entorno de escritorio se pondrá en color grisaceo</i>), y anota aproximadamente el porcentaje de memoria RAM y CPU consumidas por el sistema operativo en reposo (<i>sin abrir o lanzar ninguna aplicación</i>) gracias a la información proporcionada por el Widget del Escritorio (<i>ver figura adjunta</i>). Si deseas tener información precisa de la cantidad de CPU y RAM que están consumiendo tu equipo puedes hacer uso de la aplicación <b>CPU-X</b> (<i>control+espacio y escribes <b>cpu-x</b></i>), tal como se muestra también en la imagen adjunta.
<i>Nota: Para poder acceder al Escritorio y visualizar el Widget de forma rápida, en lugar de ir minimizando una a una las diferentes ventanas que tengas abiertas puedes hacer uso del atajo de teclado <b>Super+D</b>, conde la tecla <b>Super</b> se corresponde con la tecla que tiene el logo de Windows situada a la izquierda de la barra espaciadora. Pulsando repetidas veces ese atajo podrás comprobar como se minimizan o restauran simultáneamente todas las ventanas abiertas.</i>

<br><br><div class="container">
<img class="coolimage" src="../img/parte3/vx-3.2-widget_escritorio-info_CPU_RAM.png" alt="Imagen no Localizada">
<div class="imagetext_type2"><i>Img:</i> <tt>El Widget del Escritorio nos informa del consumo de los recursos CPU y RAM</tt></div>
</div>

<br><br><div class="container">
<img class="coolimage" src="../img/parte3/vx-3.2-cpu-x-ram_cpu.png" alt="Imagen no Localizada">
<div class="imagetext_type2"><i>Img:</i> <tt>CPU-X nos proporciona información detallada de todos los recursos del sistema</tt></div>
</div><br>

</li>
<li>
Despliega el <b>Menú de Inicio Clásico</b> (<i>al estilo de Windows XP y Windows 7</i>), bien pinchando con el botón izquierdo del ratón o pulsando la tecla Super (<i>la tecla con el logo de Windows que hay a la izquierda de la barra espaciadora). Busca en en el submenú o categoría de aplicaciones <b>Sonido y Vídeo</b> la aplicación <b>Openshot</b> y abrela.  Esta aplicación te permite crear un vídeo a partir de imágenes, vídeos y música.  Advierte que todas las aplicaciones estan categorizadas en función de su utilidad (<i>Educación, Gráficos, Internet, Oficina, etc.</i>).  Minimiza la aplicación y observa el Widget del Escritorio para conocer en que porcentaje ha aumentado la memoria RAM y la CPU del sistema para saber cuanto consume dicha aplicación (<i>la finalidad es ver como afecta a los recursos del sistema el lanzar una aplicación, puede ser openshot o la que tu prefieras</i>). 
</li>
<li>
Teclea <b>CONTROL+ESPACIO</b>, escribe <b>Navegador Firefox</b> y confirma con la tecla <b>Intro</b> para abrir o lanzar dicha aplicación.  Advierte que esta forma de lanzar aplicaciones a través de <b>Albert</b> es mucho más rápida, cómoda, intuitiva y eficiente que acceder a ella a través del <b>Menú de Inicio Clásico</b> (<i>categoría Internet</i>).  Al igual que en el caso anterior, minimiza la aplicación y observa el Widget del Escritorio para conocer en cuanto ha aumentado la memoria RAM y CPU del sistema para saber cuanto consume el afamado navegador Web.  Abre varias pestañas (<i>teclea CONTROL+T</i>) y advierte su efecto sobre la memoria RAM y CPU.
</li>
<li>
Otra forma muy eficiente de lanzar una aplicación es a través de un atajo de teclado.  Un buen ejemplo es teclear la <b>Tecla de Windows (<i>tecla que se encuentra junto al ALT izquierdo</i>)+E</b> para acceder al <b>Explorador de Archivos</b> de <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Vitalinux</tt></span>.  Comprueba su funcionamiento y anota igualmente su consumo de CPU y RAM.
</li>
<li>
En ocasiones, al igual que en Windows, puede quedarse colgada alguna aplicación sin poder cerrarla.  En esos casos convendría <b>Matar</b> la aplicación como se sugiere a continuación.  Suponiendo que todavía mantienes abiertas las aplicaciones anteriores teclea <b>CONTROL+ESPACIO</b> y escribe <b>detener o matar programa</b>.  Al confirmar con la tecla <b>Intro</b> podrás advertir que el puntero del ratón cambia de forma y que al pinchar sobre cualquier aplicación abierta provoca su cierre (<i>¡¡Cuidado por que si pinchas sobre el Escritorio también cerrarás/matarás a éste!!</i>).

<br><br><div class="container">
<img class="coolimage" src="../img/parte3/vx-3.2-detener_matar_programa_vx3.png" alt="Imagen no Localizada">
<div class="imagetext_type2"><i>Img:</i> <tt>Podemos matar cualquier programa que se resista a cerrarse</tt></div>
</div><br>

</li>
<li>
Haz una breve reflexión, si lo consideras necesario, sobre la tarea realizada. Es importante advertir que hay aplicaciones que consumen prácticamente la misma cantidad de recursos que el propio sistema operativo (<i>los navegadores Web modernos Firefox o Chrome son un ejemplo de ello</i>).  Este es un aspecto sumamente importante ya que <span style='color: darkblue; font-weight: 600'; font-size: 120%;><tt>Vitalinux</tt></span> es un <b>sistema operativo ligero</b> con la finalidad de poder reutilizar equipos antiguos, pero de poco sirve que el sistema operativo lo sea si las aplicaciones que lanzamos sobre él no lo son, el equipo se acabará saturando al poner al límite sus recursos (<i>memoria RAM o CPU</i>). Es decir, en equipos con pocos recursos además de hacer uso de un sistema operativo ligero también deberíamos hacer uso de aplicaciones que lo fueran (<i>existen alternativas ligeras a toda aplicación.  Por ejemplo, Midori es un navegador Web que sería una alternativa ligera a Firefox o Chrome</i>).
</li>
<li>
De manera opcional, crea un atajo de teclado, tal como se muestra en el apartado correspondiente a <b>¿Cómo lanzar aplicaciones?</b>, de tal forma que se lance la aplicación <b>Libreoffice Writer</b> (<i>comando/orden: libreoffice --writer</i>) al pulsar la combinación de teclas <b>CONTROL+SHIFT+W</b> (<i>La tecla SHIFT es la tecla que se pulsa para escribir en mayúsculas</i>).
</li>
</ol>

{% endnotificacion_task %}
