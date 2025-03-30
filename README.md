# 🐧 Guía de Instalación y Uso de Ubuntu en WSL (Windows Subsystem for Linux)

## 📌 Índice

1. 📖 Introducción
2. 🛠️ Requisitos
3. 💻 Instalación de WSL y Ubuntu
4. ⚙️ Configuración de Ubuntu
5. 🖥️ Comandos y su uso
   - 🌐 Gestión de Redes
   - 🔄 Gestión de Procesos y Memoria
   - 👥 Gestión de Usuarios
   - 📂 Gestión de Archivos
6. ✅ Conclusión

---

## 📖 Introducción

Esta guía proporciona una descripción completa de cómo instalar y utilizar Ubuntu en Windows a través de WSL (Windows Subsystem for Linux). También se explican comandos esenciales de Ubuntu, su función y ejemplos de uso en tareas comunes.

---

## 🛠️ Requisitos

🔹 Windows 10 (versión 1903 o superior) o Windows 11.
🔹 Conexión a Internet para descargar Ubuntu.

---

## 💻 Instalación de WSL y Ubuntu

### 1️⃣ Instalar WSL

Abre PowerShell como administrador y ejecuta el siguiente comando:

```bash
wsl --install
```

🔹 Este comando habilitará WSL y descargará Ubuntu por defecto. Requiere reiniciar el sistema.

### 2️⃣ Instalar una versión específica de Ubuntu (opcional)

🔹 Abre la **Microsoft Store**, busca "Ubuntu" y selecciona la versión que prefieras (ej. Ubuntu 20.04). Luego, haz clic en "Instalar".

---

## ⚙️ Configuración de Ubuntu

1️⃣ Abre Ubuntu desde el menú de inicio.
2️⃣ Configura un nombre de usuario y contraseña cuando se te solicite.
3️⃣ Asegúrate de que Ubuntu esté actualizado ejecutando:

```bash
sudo apt update && sudo apt upgrade
```

---

## 🖥️ Comandos y su uso

### 🌐 Gestión de Redes

🔹 **ifconfig** - Muestra la configuración de red actual.
```bash
ifconfig
```
📌 Uso: Ver la dirección IP de tu máquina.

🔹 **ping [dirección]** - Verifica la conectividad con un servidor remoto.
```bash
ping google.com
```
📌 Uso: Comprobar si puedes conectarte a un sitio web.

🔹 **ip a** - Muestra todas las interfaces de red y su estado.
```bash
ip a
```
📌 Uso: Revisar el estado de las conexiones de red.

---

### 🔄 Gestión de Procesos y Memoria

🔹 **htop** - Muestra información en tiempo real de los procesos.
```bash
htop
```
📌 Uso: Monitorear el uso de CPU y memoria.

🔹 **free -h** - Muestra la cantidad de memoria libre y usada.
```bash
free -h
```
📌 Uso: Ver cuánta memoria está disponible.

🔹 **ps aux** - Lista todos los procesos en ejecución.
```bash
ps aux
```
📌 Uso: Identificar procesos que consumen recursos.

---

### 👥 Gestión de Usuarios

🔹 **adduser [nombre]** - Crea un nuevo usuario.
```bash
sudo adduser nuevo_usuario
```
📌 Uso: Agregar un usuario al sistema.

🔹 **userdel [nombre]** - Elimina un usuario existente.
```bash
sudo userdel usuario
```
📌 Uso: Eliminar una cuenta innecesaria.

🔹 **addgroup [nombre]** - Crea un nuevo grupo.
```bash
sudo addgroup nuevo_grupo
```
📌 Uso: Organizar usuarios en grupos.

---

### 📂 Gestión de Archivos

🔹 **cd [directorio]** - Cambia al directorio especificado.
```bash
cd Documentos
```
📌 Uso: Navegar entre carpetas.

🔹 **cp [origen] [destino]** - Copia un archivo o directorio.
```bash
cp archivo.txt copia_archivo.txt
```
📌 Uso: Crear una copia de seguridad de un archivo.

🔹 **mv [origen] [destino]** - Mueve o renombra un archivo.
```bash
mv archivo.txt nuevo_nombre.txt
```
📌 Uso: Renombrar un archivo o moverlo de ubicación.

🔹 **rm [archivo]** - Elimina un archivo.
```bash
rm archivo.txt
```
📌 Uso: Eliminar un archivo que ya no necesitas.

🔹 **rmdir [directorio]** - Elimina un directorio vacío.
```bash
rmdir carpeta/
```
📌 Uso: Borrar carpetas sin contenido.

🔹 **rm -r [directorio]** - Elimina un directorio y su contenido.
```bash
rm -r carpeta/
```
⚠️ ¡Cuidado! Esto borra todo dentro de la carpeta de forma permanente.

🔹 **mkdir [nombre]** - Crea un nuevo directorio.
```bash
mkdir nueva_carpeta
```
📌 Uso: Crear una carpeta para organizar documentos.

---

## ✅ Conclusión

Con esta guía, puedes instalar y configurar Ubuntu en WSL, además de utilizar los comandos esenciales para gestionar redes, procesos, usuarios y archivos. ¡Explora y domina Linux en tu sistema Windows! 🚀🐧

