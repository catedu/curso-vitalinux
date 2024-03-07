# Propietarios y Permisos

## Contenido

- [1 Usuarios de Vitalinux](#UsuariosdeVitalinux)
- [2 Perfil del Usuario en Linux. Permisos](#PerfilUsuarioLinuxPermisos)

## Usuarios de Vitalinux {#UsuariosdeVitalinux}

A diferencia de otros sistemas operativos como Windows, por cuestiones de seguridad, las distribuciones Linux como Ubuntu (y Vitalinux se basa en ella) no permiten iniciar sesión en el sistema con **la cuenta de root o superusuario**.  De esta forma Linux se asegura de que si un **software malicioso** accede al sistema (*virus, gusano, etc.*) no tendrá privilegios en la sesión iniciada para afectar al sistema de ficheros del equipo, pudiendo alterar únicamente a las carpetas y archivos que le pertenecen al usuario que ha iniciado sesión.


En **Vitalinux** por defecto ya vienen preconfiguradas tres cuentas de usuario para poder trabajar con él en los centros educativos:

1.  Usuario **dga**: perfil de usuario con el que se inicia por primera vez Vitalinux y con el que se realiza la post-instalación.  Su **password** por defecto es **careidga**.  Puede realizar tareas administrativas (*p.e. instalar nuevo software, configurar impresoras, etc.*) mediante la previa introducción de su password.
1.  Usuario **docente**: perfil de usuario recomendado para los **docentes** de los centros.  Su **password** por defecto es **careidga**.  Puede realizar tareas administrativas (*p.e. instalar nuevo software, configurar impresoras, etc.*) mediante la previa introducción de su password.
1.  Usuario **estudiante**: perfil de usuario recomendado para los **estudiantes** de los centros.  Su **password** por defecto es **estudiante**.  **No puede** realizar tareas administrativas.

Éstas tres cuentas se crearon como configuración básica para un centro, pero en cualquier momento **se pueden crear** las cuentas de usuarios que se creen necesarias para poder trabajar con el sistema de forma más personalizada/granular. 
Para ello podemos **crear cuentas**:

-  Del sistema. Similares a la de docente/estudiante/dga y con los permisos necesarios
-  Hacer uso de una Base de Datos de usuarios centralizada tipo **LDAP** (y aconsejable en el caso de querer trabajar con muchas cuentas de usuario).
Cuando marcamos en la post-instalación que un equipo se va a emplear a **casa**, lo primero que se sugiere es crear una cuenta de usuario, ya que se entiende que la figura de estudiante/docente no tiene sentido en un ordenador personal.

{% notificacion_important title='¿Al ser públicas las credenciales de los usuarios hay problemas de seguridad?' %}
Como es obvio, al ser información pública la password de los usuarios <b>docente</b> y <b>dga</b> (<i>careidga</i>), si éstas no se cambian existe un riesgo de seguridad muy importante en Vitalinux ya que son cuentas con privilegios de administración.  Para subsanarlo se recomienda lo siguiente:
<ul>
<li>
Si va a hacerse uso de los perfiles de los usuarios <b>docente</b> y <b>estudiante</b> dentro de un <b>Centro Educativo</b>, se deberían <b>modificar las passwords</b>, al menos de los usuarios <b>docente</b> y <b>dga</b>.  Para facilitar esta tarea en los centros ( nos podemos encontrar con cientos de equipos donde modificar la contraseña), Vitalinux puede cambiar las <b>passwords</b> de manera desatendida y automatizada como el resto de configuraciones...genial, no?.  Por esta razón, cuando un centro va a instalar Vitalinux en sus equipos indican previamente a los responsables del programa cuales quieren que sean sus nuevas passwords. Ni que decir tiene que el cambio de passwords general se puede llevar a cabo en cualquier momento: por ejemplo para un nuevo curso, cuando la contraseña se ha visto "comprometida", cambio de profesorado...
</li>
<li>
Si va a hacerse uso de Vitalinux en <b>Casa</b>, o fuera de un <b>Centro Educativo</b>, conviene en la <b>post-instalación</b>, tal como vimos en la teoría del curso, <b>crear un nuevo usuario administrador con una password personalizada</b> y eliminar las cuentas de usuario preconfiguradas que ya existen.
</li>
{% endnotificacion_important %}


## Perfil del Usuario en Linux. Permisos {#PerfilUsuarioLinuxPermisos}

Cada usuario en Vitalinux tan sólo es propietario del **perfil** que le pertenece.  Se entiendo por **perfil** el conjunto de directorios y archivos del cual es el propio usuario el propietario, y que por defecto se corresponde con el contenido del directorio ubicado en **/home/*&lt;nombre-usuario&gt;***.  Por ejemplo, el usuario **docente** es propietario de todo lo que cuelga de **/home/docente** y el usuario **estudiante** de lo que hay en **/home/estudiante**.

{% coolimages_type2 url_image="../img/Sistema-archivos-perfis-usuario-sin-ocultos.png" %}
El perfil de un usuario esta compuesto por un conjunto de directorios visibles que le pertenecen y que puede modificar
{% endcoolimages_type2 %}

{% coolimages_type2 url_image="../img/Sistema-archivos-perfis-usuario-con-ocultos.png" %}
El perfil de un usuario también esta compuesto por un conjunto de directorios y archivos ocultos que se pueden visualizar pulsando la combinación CONTROL + H
{% endcoolimages_type2 %}

Esto significa que fuera del perfil que le pertenece al usuario, este puede tener limitados los **permisos de lectura, escritura y ejecución**, estando estos presentes en todo archivo y directorio del sistema.  Estos permisos nos vienen a decir lo siguiente:

1.  Permiso de **lectura**: en el caso de tratarse de un archivo, este permiso te permite abrirlo y ver su contenido.  En el caso de tratarse de un directorio este permiso nos indica que podemos ver los archivos y subdirectorios que contiene.
1.  Permiso de **escritura**: nos indica que podemos modificar el contenido del archivo o directorio.
1.  Permiso de **ejecución**: en el caso de tratarse de un archivo, este permiso nos indica que si archivo es un programa vamos a poder ejecutarlo.  En el caso de tratarse de un directorio este permiso nos indica que podemos abrir/acceder a la carpeta.
Para poder consultar **quien es propietario** de un directorio o archivo simplemente hay que pinchar con el botón derecho del ratón sobre él y seleccionar la opción **Propiedades**, y en la ventana que nos aparezca, pinchar sobre la **pestaña permisos**.

{% coolimages_type2 url_image="../img/parte4/vx-permisos_directorio.png" %}
Pinchando con el botón derecho del ratón sobre un archivo o directorio podemos consultar sus Propiedades/permisos
{% endcoolimages_type2 %}

