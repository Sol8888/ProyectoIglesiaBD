# ProyectoIglesiaBD

Este proyecto es una aplicación Flask para gestionar información de una iglesia.

---

## 🚀 Instalación de Flask en Visual Studio Code

### 1️⃣ Abre VS Code

- Usa el atajo `Ctrl + ñ` para abrir la terminal integrada.
- O ve a `Terminal > New Terminal`.

### 2️⃣ Crea un entorno virtual
python -m venv venv
### 3️⃣ Activa el entorno virtual
.\venv\Scripts\Activate.ps1
### ⚠️ Problema común: error de permisos
Si al intentar activar el entorno virtual ves un error como:

.\venv\Scripts\Activate.ps1 : File C:\Users\...\Activate.ps1 cannot be loaded because running scripts is disabled on this system.

Entonces debes cambiar la política de ejecución de PowerShell:

Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Presiona S (o Y) para confirmar.

Ahora intenta activar de nuevo:

.\venv\Scripts\Activate.ps1
4️⃣ Instala Flask

pip install flask

---
### 🛠️ Configuración del proyecto 

### 1️⃣ Abre la base de datos creada

Dentro de la base de datos se deben crear los primeros dos usuarios
Para ello en SQL Managment Studio ingresa a la base de datos, click derecho en usuarios dentro de tablas y seleccionar los primeros 200.
Se deben crear usuarios con dos roles:
- A : Administrador
- U : Usuario

### 2️⃣ Config Json

Dentro del archivo config.json se debe colocar:

{
  "name_server": "nombre de tu servidor", //Importante colocar el de tu servidor actual 
  "database": "SistemaCatequesisQuito",
  "username": "CVCGrupo1",
  "password": "CVCGrupo1",
  "controlador_odbc": "SQL Server"
}
