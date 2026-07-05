# Python Starter Project

Este es un proyecto base de Python configurado para ejecutarse fácilmente usando Docker o un entorno virtual local.

## 🛠️ Prerrequisitos

Para ejecutar este proyecto, necesitarás instalar algunas herramientas. Elige según cómo prefieras ejecutar la aplicación.

### Descarga de Herramientas

1. **Docker y Docker Compose** (Recomendado): Te permite ejecutar la aplicación en un contenedor aislado, sin preocuparte de instalar configuraciones complejas en tu sistema.
   - [Descargar Docker Desktop (Windows, macOS, Linux)](https://www.docker.com/products/docker-desktop/)
   - *Nota para usuarios de Linux: En algunas distribuciones, también se puede instalar Docker Engine y Docker Compose directamente desde el gestor de paquetes de tu sistema operativo.*

2. **Python**: Necesario si prefieres ejecutar el proyecto localmente sin Docker.
   - [Descargar Python (Windows, macOS, Linux)](https://www.python.org/downloads/)
   - *Asegúrate de marcar la opción "Add Python to PATH" durante la instalación en Windows.*

3. **Git**: Para el manejo de versiones.
   - [Descargar Git](https://git-scm.com/downloads)

---

## 🚀 Ejecución del Proyecto

### Opción 1: Usando Docker (Recomendado)

El uso de Docker simplifica y estandariza la ejecución. Estos pasos funcionan exactamente igual para **Windows**, **macOS** y **Linux**.

1. Asegúrate de tener **Docker Desktop** abierto y corriendo en segundo plano.
2. Abre tu terminal o consola (PowerShell/CMD en Windows, Terminal en macOS/Linux).
3. Navega al directorio raíz del proyecto y ejecuta:

   ```bash
   docker-compose up --build
   ```

Este comando construirá la imagen, instalará las dependencias (si agregas algo a `requirements.txt`) y ejecutará el archivo `main.py`.

### Opción 2: Ejecución Local (Entorno Virtual)

Si prefieres usar Python nativamente en tu máquina, sigue estas instrucciones dependiendo de tu sistema operativo:

#### 💻 En Windows:

1. Abre una terminal (Símbolo del sistema o PowerShell) en el directorio del proyecto.
2. Crea el entorno virtual (solo necesitas hacerlo la primera vez):
   ```cmd
   python -m venv venv
   ```
3. Activa el entorno virtual:
   ```cmd
   .\venv\Scripts\activate
   ```
4. Instala las dependencias:
   ```cmd
   pip install -r requirements.txt
   ```
5. Ejecuta el código:
   ```cmd
   python main.py
   ```

#### 🍎🐧 En macOS y Linux:

1. Abre tu terminal en el directorio del proyecto.
2. Crea el entorno virtual (solo necesitas hacerlo la primera vez):
   ```bash
   python3 -m venv venv
   ```
3. Activa el entorno virtual:
   ```bash
   source venv/bin/activate
   ```
4. Instala las dependencias:
   ```bash
   pip install -r requirements.txt
   ```
5. Ejecuta el código:
   ```bash
   python3 main.py
   ```
