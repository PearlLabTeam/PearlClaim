<img src="https://github.com/PearlLabTeam/PearlClaim/blob/main/images/smallers-logo.png" width=1500 height=700>

## Introducion

PearlClaim es un plugin esencial para la creación de Terrenos en su servidor, ofreciendo características avanzadas y un control completo sobre sus Tierras.
Puede editar absolutamente todo sobre el plugin, con un GUI/Menú avanzado, pero, super fácil de utilizar.

A pesar de estar en Modo Beta, estamos dedicados a mejorar el plugin y hacer de este uno de los mejores que pueda existir.
Cualquier comentario y/o informe de errores son bienvenidos y serán atendidos rápidamente. ¡Experimenta lo último en tecnología de Creación de Terrenos, y
disfruta con PearlClaim!

## Dependencias

Para el perfeco funcionamiento de PearlClaim, debe tener instalado:

- [Vault.jar](https://www.spigotmc.org/resources/vault.34315/)
- Un plugin de economía
- Un plugin de permisos

Algunos plugins de permisos recomendados son:

- [LuckPerms](https://luckperms.net/)
- [UltraPermissions](https://www.spigotmc.org/resources/ultra-permissions.42678/)
- [GroupManager](https://www.spigotmc.org/resources/groupmanager.38875/)

## Tabla de Contenido

- [Comandos y Permisos](https://github.com/PearlLabTeam/PearlClaim/blob/main/README_ES.md#Comandos-y-Permisos)
- [Configuraciones Generales](https://github.com/PearlLabTeam/PearlClaim/blob/main/README_ES.md#Configuraciones-Generales)
- [Creacion y Configuracion de Terrenos](https://github.com/PearlLabTeam/PearlClaim/blob/main/README.md#Creacion-y-Configuraciones-de-Terrenos)
- [Añadir Almacenes a los Terrenos](https://github.com/PearlLabTeam/PearlClaim/blob/main/README_ES.md#Añadir-Almacenes-a-los-Terrenos)
- [Mundos en Lista Negra](https://github.com/PearlLabTeam/PearlClaim/blob/main/README_ES.md#Mundos-en-Lista-Negra)
- [Procedente de Otros Plugins de Terrenos](https://github.com/PearlLabTeam/PearlClaim/blob/main/README_ES.md#Procedente-de-Otros-Plugins-de-Terrenos?)
- [API Uso](https://github.com/PearlLabTeam/PearlClaim/blob/main/README_ES.md#API-Uso)

## Nota

Tenga en cuenta que PearlClaim se encuentra en una Fase Beta y puede contener algunos errores. Si encuentra alguno, o tiene algún problema; lo invitamos a
unirse a nuestro servidor de Discord, donde estaremos más que encantados de ayudarle a resolver cualquier problema que presente.

Gracias por su comprensión y apoyo a medida que continuamos mejorando cada vez más la funcionalidad de PearlClaim. 

## Comandos y Permisos

Aquí está la lista de comandos disponibles de PearlClaim y sus respectivos permisos:

| Comando                                         | Descripción                                                                                                                                | Permiso                    |
|-------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------|----------------------------|
| /claim                                          | Abrir el menú de configuración de un Terreno si se encuentra en uno                                                                        | pearlclaim.use             |
| /claim sethome                                  | Establece el punto de teletransporte de tu Terreno                                                                                         | pearlclaim.sethome         |
| /claim create                                   | Crea un Terreno de tus Terrenos almacenados (Si tiene)                                                                                     | pearlclaim.create          |
| /claim config                                   | Abrir el menú de configuración de un Terreno si se encuentra en uno                                                                        | pearlclaim.config          |
| /claim flags                                    | Abre el menú de Flags del Terreno en el que te encuentras                                                                                  | pearlclaim.flags           |
| /claim storage                                  | Abre los almacenes que tengas en tu Terreno                                                                                                | pearlclaim.storage         |
| /claim delete                                   | Elimina el Terreno en el que te encuentras                                                                                                 | pearlclaim.delete          |
| /claim store                                    | Recoge y Almacene el Terreno en el que te encuentras                                                                                       | pearlclaim.store           |
| /claim members < + / - > < jugador >            | Añade o elimina a un jugador en el Terreno en el que te encuentras                                                                         | pearlclaim.modify.members  |
| /claim role < member/admin >                    | Modifica los roles de Miembro/Administrador del Terreno en el que te encuentras                                                            | pearlclaim.modify.roles    |
| /claim admin                                    | Abre el Menú de Configuración Administrativo                                                                                               | pearlclaim.admin           |
| /claim admin giveclaim < jugador > < terrenoID >| Da a un jugador un Terreno con la ID mencionada                                                                                            | pearlclaim.admin           |
| /claim admin import                             | Importa Terrenos/Protecciones de EpicProtections/Protection Stones (Si quieres que añadamos más plugins, háznolo saber en nuestro Discord) | pearlclaim.admin           |
| /claim admin reload                             | Recarga todos los archivos y vuelve a crear los archivos faltantes                                                                         | pearlclaim.admin           |
| <br><br>                                        | |                            |
| /claims list                                    | Ve la lista de tus Terrenos creados                                                                                                        | pearclaim.claims.list      |
| /claims tp <nombre del terreno>                 | Teletransportate a tu Terreno                                                                                                              | pearlclaim.claims.teleport |

<br><br>

### Permisos Adicionales

| Permiso | Descripción | Predeterminado |
|------------|-------------|---------|
| pearlclaim.admin | Permiso para anular y manipular cada terreno | op |
| pearlcalim.flag.* | Permiso para manipular cualquier flag | op |
| pearlclaim.flag.pvp | Permiso para manipular la flag de PVP | op |
| pearlclaim.flag.hostile_spawning | Permiso para manipular la flag de HOSTILE_SPAWNING | op |
| pearlclaim.flag.peaceful_spawning | Permiso para manipular la flag de PEACEFUL_SPAWNING | op |
| pearlclaim.flag.crop_growth | Permiso para manipular la flag de CROP_GROWTH | op |
| pearlclaim.flag.interact | Permiso para manipular la flag de INTERACT | op |
| pearlclaim.flag.containers | Permiso para manipular la flag de CONTAINERS | op |
| pearlclaim.flag.explosions | Permiso para manipular la flag de EXPLOSIONS | op |
| pearlclaim.flag.entity_interact | Permiso para manipular la flag de ENTITY_INTERACT | op |
| pearlclaim.flag.water_flow | Permiso para manipular la flag de WATER_FLOW | op |
| pearlclaim.flag.lava_flow | Permiso para manipular la flag de LAVA_FLOW | op |
| pearlclaim.flag.player_fly | Permiso para manipular la flag de PLAYER_FLY | op |
| pearlclaim.flag.set_home | Permiso para manipular la flag de SET_HOME | op |
| pearlclaim.flag.fire_spread | Permiso para manipular la flag de FIRE_SPREAD | op |
| pearlclaim.flag.pve | Permiso para manipular la flag de PVE | op |
| pearlclaim.role.edit | Permisos para modificar los permisos de un rol en un terreno | op |
| pearlclaims.claims.changename | Permiso para cambiar el nombre de tu terreno | op |

<br><br><br>

## Configuraciones Generales

Algunas configuraciones generales para administradores son:
<br>

### Esquema de Seleccion

La opción puede modificarse fácilmente con un simple click, como se puede observar en la imagen. Este proceso intuitivo
y sencillo permite a los administradores ajustar la configuración según sus preferencias de forma rápida y sencilla.

<img src="https://i.imgur.com/PSh4yki.png" width="" height="">
<img src="https://i.imgur.com/FVUiqCh.png" width="" height="">
<img src="https://i.imgur.com/NqPukWw.png" width="" height="">

### Creación Predeterminada de Terrenos

La opción "Creación Predeterminada de Terrenos" ofrece a los administradores la posibilidad de regular la generación automática de Terrenos para los jugadores nuevos
que se unan al servidor. Cuando está activa, si PearlClaim no detecta un archivo de datos de jugador para un jugador nuevo, generará uno y añadirá
automáticamente las reclamaciones por defecto definidas en el sistema. Esta función permite un proceso de generación de reclamaciones ficiente y sin
problemas para los jugadores nuevos.

<img src="https://i.imgur.com/jDVTBQO.png" width="" height="">
<br><br>La opción puede modificarse fácilmente con un simple click, como se puede observar en la imagen. Este proceso intuitivo y sencillo permite a los administradores ajustar la configuración según sus preferencias de forma rápida y sencilla.
<br><br><br>

### Cambio de Idioma

Esta opción permite a los administradores cambiar de idioma el plugin, lo que hace que toda la interfaz del plugin y sus mensajes, cambien al idioma seleccionado.

<img src="https://i.imgur.com/X6VJuIA.png" width="" height="">
<br><br>La opción puede modificarse fácilmente con un simple click, como se puede observar en la imagen. Este proceso intuitivo y sencillo permite a los administradores ajustar la configuración según sus preferencias de forma rápida y sencilla.
<br><br><br>

### Almacenamiento de Terrenos

Esta opción permite a los administradores la posibilidad de controlar el acceso al almacenamiento de todos los Terrenos dentro del sistema.
Cuando la opción se establece en "Desactivado", se bloqueará el acceso a los jugadores al almacenamiento de los Terrenos, sin afectar el contenido almacenados reales.

<img src="https://i.imgur.com/JYwc76w.png" width="" height="">
<br><br>La opción puede modificarse fácilmente con un simple click, como se puede observar en la imagen. Este proceso intuitivo y sencillo permite a los administradores ajustar la configuración según sus preferencias de forma rápida y sencilla.
<br><br><br>

### Almacenamiento de Terrenos Requiere Permisos

Esta opción determina si los jugadores requieren cierto permiso para acceder al almacenamiento a través de la interfáz gráfica del usuario (Menú). 
Cuando se establece en "Requerido", los jugadores deben poseer el permiso específico para poder generar el almacenamiento en el Menú. 
Por otro lado, si se establece en "No requerido", los jugadores podrán ver el botón de almacenamiento en el menú sin algún permiso. 
Sin embargo, es importante recordar que esta opción no afecta la capacidad de los jugadores de acceder al contenido del almacenamiento, por lo cual, 
seguirá siendo necesario el permiso específico.

<img src="https://i.imgur.com/ty2frbx.png" width="" height="">
<br><br>La opción puede modificarse fácilmente con un simple click, como se puede observar en la imagen. Este proceso intuitivo y sencillo permite a los administradores ajustar la configuración según sus preferencias de forma rápida y sencilla.
<br><br><br>

*Todas estas configuraciones pueden modificarse fácilmente desde el menú de configuración del plugin, lo que permite a los administradores configurarlo exactamente como desean.*
<br><br><br>

# Creacion y Configuracion de Terrenos

Crear y modificar reclamos nunca ha sido más fácil. PearlClaim ofrece un sistema de creación de terrenos en el juego para los creadores de servidores, 
proporcionando un enfoque más intuitivo y fácil de usar en comparación con otros complementos que requieren modificaciones manuales dentro de los archivos de configuración. 
Para crear un nuevo terreno, simplemente navegue hasta la interfaz de usuario del editor de reclamos haciendo click en el botón "Editor de terrenos" dentro de la configuración del administrador y luego seleccione el botón "Crear un Terreno". 
En cuanto a la modificación de un terreno específico, simplemente haga click en él para acceder a otra interfaz de usuario que contiene una variedad de opciones de personalización.

### Terreno Predeterminado

Esta opción permite a los administradores establecer un Terreno como predeterminado, lo que significa que se agregará a los terrenos almacenados de los jugadores nuevos.

<img src="https://i.imgur.com/iUWQZlT.png" width="" height="">
<br><br>La opción puede modificarse fácilmente con un simple click, como se puede observar en la imagen. Este proceso intuitivo y sencillo permite a los administradores ajustar la configuración según sus preferencias de forma rápida y sencilla.
<br><br><br>

### Modificar Almacenamiento

Esta opción abre un Menú separado que permite administrar la configuración del almacenamiento de terrenos. Información adicional puede encontrarse en la sección de "Creacion y Configuracion de Terrenos".

<img src="https://i.imgur.com/IKpKddo.png" width="" height="">

***Editor de almacenamiento de Terrenos***

<img src="https://i.imgur.com/C5VyhJe.png" width="" height="">
<br><br><br>

### Dar a Jugador

Permite a los administradores transferir el terreno a otro jugador especificando el nombre del jugador en el chat. 
Es importante tener en cuenta que cualquier actualización realizada en el terreno después de
que se haya transferido no se reflejará en los reclamos almacenados del jugador receptor.

<img src="https://i.imgur.com/EXw16Fz.png" width="" height=""><br><br>
<img src="https://i.imgur.com/yqd4CZD.png" width="" height=""><br><br>
<img src="https://i.imgur.com/naRxnMh.png" width="" height=""><br><br>
<img src="https://i.imgur.com/djGdTBi.png" width="" height="">
<br><br><br>

### Cambiar Radio

Permitir el ajuste del radio X, Y, y Z inicial del terreno.

<img src="https://i.imgur.com/GNyQtRi.png" width="" height=""><br><br>
<img src="https://i.imgur.com/4Lp6BiV.png" width="" height=""><br><br>
<img src="https://i.imgur.com/Wqwc9aN.png" width="" height=""><br><br>
<img src="https://i.imgur.com/GlkIqsj.png" width="" height="">
<br><br><br>

### Permitir Mejora

Esta opción determina si los jugadores pueden mejorar sus terrenos con la moneda del juego.

<img src="https://i.imgur.com/zXPvm0H.png" width="" height=""><br><br>
Si se establece en **MEJORABLE**, deberás proporcionar el precio para el costo de mejora por bloque y el radio máximo de mejora para todas las dimensiones (X, Y, y Z).
<img src="https://i.imgur.com/iDlBA46.png" width="" height=""><br><br>
<img src="https://i.imgur.com/FiEz2wz.png" width="" height=""><br><br>

### Bloque de Solicitud de Creación

Especifica el bloque animado que acompañará al jugador al seleccionar el área para el terreno. Este bloque marcará el punto central del Terreno.

<img src="https://i.imgur.com/8nup5YJ.png" width="" height=""><br><br>
***Cuando se active, este botón inicia la apertura de una nueva interfaz gráfica de usuario con varias páginas. En este menú, el usuario podrá seleccionar
el material del elemento de animación.***

<img src="https://i.imgur.com/WpP8qtD.png" width="" height=""><br>

### Eliminar

Elimina el terreno y todas sus configuraciones.

<img src="https://i.imgur.com/PqwY4Ub.png" width="" height=""><br>

### Volver

Vuelve al menú principal

<img src="https://i.imgur.com/WxAbeBL.png" width="" height=""><br>
<br><br>

# Añadir Almacenes a los Terrenos
Nos complace presentar nuestro sistema de almacenamiento de última generación para tus tierras. Nuestro sistema ofrece una solución conveniente y eficiente para el almacenamiento virtual sin la necesidad de cofres físicos.

Con unos pocos clicks, puede personalizar cada aspecto del almacenamiento de su terreno, incluyendo el número de almacenamientos, su tamaño e incluso el contenido predefinido para un kit si se desea. Nuestro sistema crea un sistema de almacenamiento virtual que se copia en el terreno del jugador, dándole control total sobre sus necesidades de almacenamiento.

Además, tienes control completo sobre el aspecto de la interfaz gráfica de usuario (Menú) del almacenamiento a través del archivo StoragesGUI.yml. Si desea conectar un botón específico a una mochila, simplemente proporcione el ID de la mochila dentro del archivo.

Estamos seguros de que nuestro sistema avanzado de almacenamiento superará tus expectativas y te proporcionará la mejor experiencia posible. Gracias por considerar nuestro plugin.
<br><br>

### Para comenzar, simplemente haga click en el botón "Crear almacenamiento" ubicado en el Yunke.

<img src="https://i.imgur.com/xDaU8Sf.png" width="" height=""><br>

### Después de hacer click en el botón, se le pedirá que ingrese el nombre del almacenamiento, que servirá como identificador para vincular el almacenamiento al archivo StorageGUI.

<img src="https://i.imgur.com/15IHfvi.png" width="" height=""><br>

### Al proporcionar el nombre, deberá especificar el tamaño del almacenamiento, es decir, los espacios disponibles en el inventario.

<img src="https://i.imgur.com/QZ0LBx1.png" width="" height=""><br>

### Una vez que se haya ingresado la información necesaria, se generará un nuevo botón de almacenamiento dentro del Menú del editor de almacenamiento. Si desea incluir objetos predefinidos en el almacenamiento, simplemente colóquelos dentro del almacenamiento y se agregarán al almacenamiento del jugador al recibir el terreno. Si prefiere un almacenamiento vacío, simplemente omita este paso.

<img src="https://i.imgur.com/crMKUWh.png" width="" height=""><br>
<img src="https://i.imgur.com/QFI4sVI.png" width="" height=""><br><br><br>

# Mundos en Lista Negra
**Entendemos la necesidad de controlar y gestionar la creación de terrenos en ciertas regiones. Es por eso que nos enorgullece ofrecer nuestro sistema de Mundos en Lista Negra, que le permite deshabilitar la creación de terrenos en ciertos mundos.**

**Para utilizar este sistema, simplemente vaya al botón de Mundos en Lista Negra dentro de la interfaz gráfica (Menú) de configuración de administrador y seleccione el mundo en el que desea bloquear la creación de terrenos. ¡Es así de simple! Si el nombre del mundo se muestra en negrita, indica que la creación de terrenos está deshabilitada en ese mundo. Si no se muestra en negrita, la creación de terrenos está permitida en ese mundo.**

**Tenga en cuenta que esta opción se limita actualmente a bloquear la creación de terrenos en general, esperamos en un futuro, ampliar las opciones para incluir la posibilidad de bloquear el acceso para colocar cierto tipo de terreno en mundos específicos.**

**Esperamos que esta función le resulte útil para agilizar el proceso de gestión de terrenos.**

<img src="https://i.imgur.com/Kmj1Wfv.png" width="" height=""><br>
<img src="https://i.imgur.com/wbymNiD.png" width="" height=""><br>
<img src="https://i.imgur.com/RvhpncD.png" width="" height=""><br><br><br>

# Procedente de Otros Plugins de Terrenos
**Entendemos que el proceso de cambiar a un nuevo sistema de protecciones de terrenos puede ser desalentador, especialmente cuando tiene una cantidad muy grande de datos existentes. Es por eso que nos enorgullece ofrecer nuestro Sistema de Importación, diseñado para facilitar la transferencia de datos desde otros plugins de terrenos/protección a nuestro sistema.**

**Actualmente, admitimos la importación de ProtectionStones y EpicProtections, pero siempre estamos abiertos a agregar soporte para otros plugins. Si tiene una solicitud para un plugin específico, le invitamos a comunicarse con nosotros a través de nuestro canal de Discord.**

**Con nuestro Sistema de Importación en el juego, la transición a nuestro plugin de creación de terrenos es muy fácil. Simplemente seleccione el plugin desde el cual desea importar datos, inicie el proceso de importación y permita que nuestro algoritmo haga el resto. Es así de sencillo.**

**Estamos seguros de que nuestro Sistema de Importación hará que su transición a nuestro plugin de creación de terrenos sea una experiencia sencilla y sin esfuerzo. Esperamos que considere elegir nuestro plugin para sus necesidades de gestión de terrenos/protección.**

*( **IMPORTANTE:** Como está considerando usar nuestro sistema de importación, le recordamos amablemente que priorice la seguridad y la estabilidad de los datos de su servidor. Antes de continuar, es esencial que cree una copia de seguridad de su servidor para asegurarse de que cualquier consecuencia no deseada se pueda abordar fácilmente. En caso de que surjan problemas técnicos durante el proceso de importación, nuestro equipo de soporte dedicado estará disponible para ayudarlo a resolver el problema. Sin embargo, tenga en cuenta que, aunque nos esforzaremos por resolver cualquier problema relacionado con el código, es posible que no podamos restaurar los datos que se hayan perdido o dañado. Al tomar la precaución de crear una copia de seguridad de antemano, puede garantizar la seguridad de sus datos y minimizar cualquier posible interrupción en su servidor. (Gracias por considerar nuestro sistema de importación)*

![Demo](https://imgur.com/5DP5dwP.gif)
<br><br>

# API Uso
Próximamente...
