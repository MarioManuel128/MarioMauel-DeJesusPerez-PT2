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
