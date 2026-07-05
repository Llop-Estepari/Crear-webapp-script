# crear-webapp

**`crear-webapp` es una herramienta CLI en Bash diseñada para entornos Arch Linux que transforma sitios web en aplicaciones de escritorio independientes utilizando el motor de Chromium.**

## Requisitos

El script requiere tener instalados los siguientes paquetes de los repositorios oficiales de Arch Linux:

```bash
sudo pacman -S chromium
```


## Instalación global
Para configurar este script como un comando global del sistema operativo:

 1. Asegúrese de que el directorio ~/.local/bin existe y está en su variable $PATH.

 2. Mueva el archivo y otorgue permisos de ejecución:

```bash
mkdir -p ~/.local/bin
mv crear-webapp ~/.local/bin/
chmod +x ~/.local/bin/crear-webapp
```

## Modo de uso
### Opción 1: Pasar argumentos por parámetro
```bash
crear-webapp "Nombre de la App" [https://ejemplo.com](https://ejemplo.com)
```
### Opción 2: Modo interactivo
Si ejecuta el comando sin argumentos, el script solicitará los datos automáticamente:

```bash
crear-webapp
```

## Directorios utilizados
El script opera de forma local dentro del directorio del usuario actual ($HOME):

Archivos de lanzamiento: ~/.local/share/applications/

Iconos descargados: ~/.local/share/icons/
