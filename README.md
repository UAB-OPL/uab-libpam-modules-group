# Paquete DEB uab-libpam-modules-group

Paquete que configura el modulo pam-group como necesario para la autenticacion.
Este modulo permite configurar la pertenencia a grupos de forma automatica

# Generar el esqueleto inicial

```
DEBFULLNAME="Jordi Román Mejias" dh_make --email Jordi.Roman@uab.cat -i -c gpl3 --native -p uab-libpam-modules-group-1.0
```

# Como Crear el paquete DEB a partir del codigo de GitHub
Para crear el paquete DEB será necesario encontrarse dentro del directorio donde localizan los directorios que componen el paquete.  Una vez allí, se ejecutará el siguiente comando (es necesario tener instalados los paquetes apt-get install debhelper devscripts):

```
apt-get install debhelper devscripts
/usr/bin/debuild --no-tgz-check -us -uc
```

# Como Instalar el paquete generado uab-libpam-modules-group*.deb:
Para la instalación de paquetes que estan en el equipo local puede hacerse uso de ***dpkg*** o de ***gdebi***, siendo este último el más aconsejado para que se instalen también las dependencias correspondientes.

```
dpkg -i *.deb
```

