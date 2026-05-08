# Proyecto Intranet - KevinHdez

## Servicios instalados

- Apache2
- BIND9
- OpenLDAP
- VSFTPD

## Instalación paquetes

sudo apt install bind9 slapd vsftpd apache2

## DNS

Configuración de la zona centro.local en:

/etc/bind/db.centro.local

## LDAP

Base DN:

dc=centro,dc=local

Usuarios:
- KevinHdez
- profKevinHdez

## Apache

VirtualHost:
intranet.centro.local

Rutas:
- /public
- /profesores
- /alumnos

## FTP

Ruta publicación:
/srv/ftp/publicaciones

## Pruebas realizadas

- nslookup correcto
- ldapsearch correcto
- autenticación LDAP funcionando
- subida FTP correcta

