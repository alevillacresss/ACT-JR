# ACT-JR
# Instalación y Ejecución de la Aplicación

Este documento proporciona instrucciones detalladas para la instalación y ejecución de la aplicación en entornos Windows y Linux.

## Requisitos Previos

Antes de comenzar, asegúrate de contar con lo siguiente:
- Python 3 instalado en tu sistema.
- Acceso a una terminal o línea de comandos.

## Instalación de Python 3

### Windows
1. Descarga la última versión de Python desde [python.org](https://www.python.org/downloads/windows/).
2. Ejecuta el instalador y marca la opción **"Add Python to PATH"**.
3. Finaliza la instalación y verifica con:
   ```sh
   python --version
   ```

### Linux
1. Abre una terminal y ejecuta:
   ```sh
   sudo apt update && sudo apt install python3 -y
   ```
2. Verifica la instalación con:
   ```sh
   python3 --version
   ```

## Instalación y Activación de pip

### Windows
1. Pip suele instalarse junto con Python. Para verificar, ejecuta:
   ```sh
   python -m pip --version
   ```
2. Si no está instalado, usa:
   ```sh
   python -m ensurepip --default-pip
   ```

### Linux
1. Instala pip con el siguiente comando:
   ```sh
   sudo apt install python3-pip -y
   ```
2. Verifica la instalación con:
   ```sh
   pip3 --version
   ```

## Creación y Activación de un Entorno Virtual

### Windows
1. Crea el entorno virtual:
   ```sh
   python -m venv venv
   ```
2. Activa el entorno virtual:
   ```sh
   venv\Scripts\activate
   ```

### Linux
1. Crea el entorno virtual:
   ```sh
   python3 -m venv venv
   ```
2. Activa el entorno virtual:
   ```sh
   source venv/bin/activate
   ```

## Instalación de Dependencias

Con el entorno virtual activado, instala las dependencias del proyecto con:
```sh
pip install -r requirements.txt
```

## Ejecución de la Aplicación

1. Asegúrate de que el entorno virtual esté activado.
2. Ejecuta la aplicación con:
   ```sh
   python app.py
   ```

## Notas
- Si usas Linux y el comando `python` no funciona, intenta con `python3`.
- Si encuentras problemas de permisos en Linux, puedes usar `sudo` antes de algunos comandos.
