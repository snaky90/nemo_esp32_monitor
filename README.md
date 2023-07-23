# NeMo - Adquisición de datos usando ESP32

## DESCRIPCION
Este repositorio contiene el código fuente necesario para compilar el binario relativo al sistema de adquisición de datos del monitor de neutrones (NeMo)  
Se incluyen además las configuraciones necesarias para generar un contenedor con el entorno IDF para el desarrollo del proyecto.


## HERRAMIENTAS USADAS
Este proyecto ha sido desarrollado usando contenedores Docker y por funcionalidad ejecutandose a través de un sistema GNU/Linux dada la dificultad existente para conectar contenedores con los puertos serie en sistemas MacOS y Windows, por lo que las herramientas y pasos especificados se basarán en las herramientas aqui expuestas.  
Las herramientas usadas han sido actualizadas a las ultimas versiones disponibles a Julio de 2023

- Debian GNU/Linux 12 Bookworm
- Visual Studio Code + Plugins [ Docker, DevContainers, Remote SSH ]
- Docker Engine 24.0.4
- Espressif IDF v4.4.5 (containerized)
- Componentes Esp-IDF-Lib 

## PREPARACION DEL ENTORNO
### LANZAMIENTO DEL CONTENEDOR DE DESARROLLO
En la carpeta .devcontainer se encuentran los archivos necesarios preconfigurados para lanzar el contenedor de desarrollo.  
Dado que necesitamos la libreria de componentes Esp-IDF-Lib requerimos de clonar la ultima version de su repositorio y guardarla dentro de .devcontainer
> cd .devcontainer  
git clone https://github.com/UncleRus/esp-idf-lib.git

Una vez hecho ese paso, lanzar el contenedor de desarrollo desde Visual Studio Code, este se creará, empezará a funcionar y la interfaz de VSCode estará dentro del contenedor.