# MarioMauel-DeJesusPerez-PT2

# Manual d’instal·lació de Nextcloud

# Preparación del entorno en IsardVDI

Para instalar Nextcloud he utilizado una máquina virtual creada en IsardVDI.
Primero accedí a la plataforma con mi usuario y seleccioné la opción de crear una nueva máquina virtual. Elegí una plantilla de Ubuntu como sistema operativo, ya que es compatible y estable para montar un servidor web. Una vez creada la máquina, la inicié desde IsardVDI y accedí al escritorio remoto.

# Instalación de la pila necesaria

Dentro de la máquina virtual, actualicé el sistema y luego instalé los componentes necesarios para Nextcloud: servidor web (Apache), base de datos (MariaDB o MySQL) y PHP con sus módulos.
Tras la instalación, comprobé que el servidor web funcionaba correctamente accediendo a la IP de la máquina desde el navegador.

# Descarga y despliegue de Nextcloud

A continuación descargué la última versión de Nextcloud desde la página oficial. Descomprimí el paquete en el directorio del servidor web (por ejemplo, /var/www/html/nextcloud) y ajusté los permisos de los archivos para que el servidor pudiera acceder a ellos sin problemas.
Con esto dejé preparada la parte de archivos de la aplicación.

# Configuración de la base de datos

Después configuré la base de datos para Nextcloud.
Accedí al gestor de base de datos (por ejemplo, mysql) y creé una base de datos específica para Nextcloud, junto con un usuario y una contraseña propios. Esta separación permite que Nextcloud tenga su propio espacio de datos y mejora la seguridad y el control.

# Asistente de instalación web

Una vez preparados los archivos y la base de datos, abrí un navegador (desde la propia VM o desde otra máquina de la red) y accedí a la URL de la máquina virtual donde estaba Nextcloud.
Se cargó el asistente de instalación, donde introduje el usuario administrador, la contraseña y los datos de la base de datos que había creado. Tras completar el asistente, el sistema terminó la instalación y me mostró la interfaz principal de Nextcloud.

# Verificación del funcionamiento

Por último, comprobé que la instalación funcionaba correctamente iniciando sesión con el usuario administrador y accediendo a las secciones principales (archivos, configuración, etc.).
También verifiqué que se podía acceder a Nextcloud desde otras máquinas de la misma red, usando la IP de la máquina virtual. De esta forma confirmé que la instalación mediante IsardVDI era correcta y que el servidor estaba listo para el resto de configuraciones de la práctica.

# Demostración del funcionamiento

# Subir archivos

![Logo de Markdown](/captura1.png)

En este apartado explico cómo añadir documentos al servidor. Para ello accedí a la sección Files y utilicé la opción de subir archivos. Seleccioné un documento desde mi ordenador y comprobé que aparecía correctamente en la lista. Con esta prueba verifiqué que Nextcloud guarda los archivos sin errores y que el sistema funciona correctamente en su tarea más básica.

# Crear carpetas

![Logo de Markdown](/captura2.png)

Aquí muestro cómo organizar el contenido dentro del espacio de usuario. Para ello utilicé la opción + New y seleccioné Folder para crear nuevas carpetas. Añadí varias, como Documents o Images, y confirmé que se creaban sin problemas. Este paso demuestra que el usuario puede estructurar su información dentro del servidor.

# Creación de usuarios

# Crear tres usuarios

![Logo de Markdown](/captura3.png)

En esta parte creé tres cuentas distintas dentro del panel de administración: un administrador, un editor y un visualizador. A cada usuario le asigné un nombre, una contraseña y un grupo específico. Esto me permitió comprobar cómo se gestionan las cuentas y cómo se diferencian los roles dentro del sistema.

# Administración de archivos

# Organización de carpetas y archivos

![Logo de Markdown](/captura4.png)

En este apartado organicé el contenido del servidor creando una estructura de carpetas más completa. Añadí directorios como Personal documents, Shared work y Resources, y moví archivos dentro de cada uno para mantener un orden lógico. Esto demuestra que el sistema permite gestionar y estructurar el contenido de forma eficiente.

# Políticas de seguridad

![Logo de Markdown](/captura5.png)

Accedí a la sección Sharing dentro de la administración y activé medidas de seguridad como la caducidad automática de los enlaces públicos y la obligación de usar contraseña al compartir archivos. Estas opciones aumentan la seguridad del servidor y evitan accesos no autorizados.

# Acceso desde una máquina cualquiera de la red

# Configuración de acceso remoto

![Logo de Markdown](/captura6.png)

Para comprobar el acceso desde otra máquina, primero obtuve la dirección IP del servidor ejecutando el comando ip a. Después, desde otro dispositivo conectado a la misma red, introduje esa IP en el navegador y accedí a la página de inicio de sesión de Nextcloud. Esto demuestra que el servicio es accesible desde la red local y que funciona correctamente fuera de la máquina principal.
