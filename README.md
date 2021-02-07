# openVAS
Instalación automatizada OpenVAS en Debian 10

Prerrequisitos:
editar /etc/sudoers

Cambiar línea
Defaults        secure_path="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin:/opt/gvm/sbin"

Añadir usuario actual

Añadir 
### Allow the user running ospd-openvas, to launch openvas with root permissions
gvm ALL = NOPASSWD: /opt/gvm/sbin/openvas
gvm ALL = NOPASSWD: /opt/gvm/sbin/gsad

Guardar



editar /etc/profile
Editer el segundo PATH
PATH="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/games:/usr/games"

Guardar.

Hay que cerrar sesión del usuario actual.
