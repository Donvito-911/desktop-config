# Configuración PopOS!
## 1. Network drivers
Si el wifi no está sirviendo, hay que instalar los drivers correspondientes. Primero, debemos obtener el PCI ID,
```
lspci -nn -d 14e4:
```
En nuestro portatil dio 14e4:4331, debemos instalar (hay que estar conectado a internet via cable ethernet) el paquete correspondiente (para 14e4:4331 es firmware-b43-installer). Para más información con la tabla del PCI ID al paquete de instalación correspondiente, revisar <a href="https://askubuntu.com/questions/55868/installing-broadcom-wireless-drivers" >este blog</a>
```bash
sudo apt update && sudo update-pciids
sudo apt install firmware-b43-installer && sudo apt install linux-firmware
sudo reboot
```
## 2. Descargar Vivaldi
Ir a vivaldi descargas y descargar el archivo .deb
instalar en archivo:
```bash
sudo apt install /path/to/vivaldi-stable.deb
```
Ingresar y crear los perfiles correspondientes (Personal y Trabajo)

## 3. Cambiar wallpaper y foto de perfil
Ir al drive y descargar pirate vito y batalla de la cima (LOTR)

## 4. Instalar gnome extensions
Ir a https://extensions.gnome.org e instalar la extension. Descargar vitals y agregarla temperatura, memoria usada (en GB) y uso de procesador.
- Ir a extensions, pop shell setttings y eliminar el titulo de ventana.

## 5. Instalar gnome tweaks
```bash
sudo apt install gnome-tweaks -y
```
- Hacer swap de Ctrl y Bloq Mayus.

## 6. Instalar emacs.

```bash
sudo apt install emacs
```
