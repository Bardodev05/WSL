# 🐧 Guía de Instalación y Uso de Ubuntu en WSL (Windows Subsystem for Linux)

## 📌 Índice

1. [Introducción](#introducción)
2. [Requisitos](#requisitos)
3. [Instalación de WSL y Ubuntu](#instalación-de-wsl-y-ubuntu)
4. [Configuración de Ubuntu](#configuración-de-ubuntu)
5. [Comandos y su uso](#comandos-y-su-uso)
   - [🛡️ Gestión de Redes](#🛡️-gestión-de-redes)
   - [💡 Gestión de Procesos y Memoria](#💡-gestión-de-procesos-y-memoria)
   - [🔑 Gestión de Usuarios](#🔑-gestión-de-usuarios)
   - [💾 Gestión de Archivos](#💾-gestión-de-archivos)
6. [📄 Conclusión](#📄-conclusión)

---

## 📖 Introducción

Este documento proporciona una guía completa sobre cómo instalar y utilizar Ubuntu en Windows a través de WSL (Windows Subsystem for Linux). Además, se incluyen comandos útiles de Ubuntu con ejemplos prácticos para el manejo eficiente del sistema.

---

## ✅ Requisitos

- Windows 10 (versión 1903 o superior) o Windows 11.
- Conexión a Internet para descargar Ubuntu.

---

## 🔧 Instalación de WSL y Ubuntu

### 1️⃣ Instalar WSL

Abre **PowerShell** como administrador y ejecuta:

```sh
wsl --install
```

Este comando habilitará WSL y descargará Ubuntu por defecto. **Requiere un reinicio del sistema**.

### 2️⃣ Instalar una versión específica de Ubuntu (opcional)

1. Abre la **Microsoft Store**.
2. Busca **"Ubuntu"**.
3. Selecciona la versión deseada (ej. Ubuntu 20.04) y haz clic en **"Instalar"**.

---

## ⚙️ Configuración de Ubuntu

1. Busca **"Ubuntu"** en el menú de inicio y ábrelo.
2. Configura tu **nombre de usuario** y **contraseña** cuando se te solicite.
3. Actualiza Ubuntu ejecutando:

```sh
sudo apt update && sudo apt upgrade
```

---

## 🖥️ Comandos y su uso

### 🛜 Gestión de Redes

- **`ifconfig`** → Muestra la configuración de red.
  ```sh
  ifconfig
  ```

- **`ping [dirección]`** → Verifica la conectividad a un servidor remoto.
  ```sh
  ping google.com
  ```

- **`ip a`** → Muestra interfaces de red disponibles y su estado.
  ```sh
  ip a
  ```

---

### 💡 Gestión de Procesos y Memoria

- **`htop`** → Muestra la actividad del sistema en tiempo real.
  ```sh
  htop
  ```

- **`free -h`** → Muestra la memoria libre y usada.
  ```sh
  free -h
  ```

- **`ps aux`** → Lista los procesos en ejecución.
  ```sh
  ps aux
  ```

---

### 🔑 Gestión de Usuarios

- **`sudo adduser [nombre]`** → Crea un nuevo usuario.
  ```sh
  sudo adduser nuevo_usuario
  ```

- **`sudo userdel [nombre]`** → Elimina un usuario.
  ```sh
  sudo userdel usuario_a_eliminar
  ```

- **`sudo addgroup [nombre]`** → Crea un nuevo grupo.
  ```sh
  sudo addgroup nuevo_grupo
  ```

---

### 💾 Gestión de Archivos

- **`cd [directorio]`** → Cambia al directorio especificado.
  ```sh
  cd Documentos
  ```

- **`cp [origen] [destino]`** → Copia un archivo.
  ```sh
  cp archivo.txt copia_archivo.txt
  ```

- **`mv [origen] [destino]`** → Mueve o renombra un archivo.
  ```sh
  mv archivo.txt nuevo_nombre.txt
  ```

- **`rm [archivo]`** → Elimina un archivo.
  ```sh
  rm archivo.txt
  ```

⚠️ **Precaución**: La eliminación con `rm` es irreversible.

- **Crear un directorio**
  ```sh
  mkdir nueva_carpeta
  ```

---

## 📄 Conclusión

Con esta guía, puedes instalar y configurar Ubuntu en WSL de manera eficiente. Además, ahora conoces comandos básicos para gestionar redes, procesos, usuarios y archivos. ¡Disfruta de tu experiencia con Linux en Windows! 🚀

