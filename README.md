# Semana-10-POO
# 📦 Sistema de Gestión de Inventarios en Python

Este proyecto implementa un sistema de gestión de inventarios utilizando **Programación Orientada a Objetos (POO) en Python**.  
Fue desarrollado como parte de la **Semana 10 de la asignatura de POO**, aplicando conceptos de clases, objetos, encapsulación y modularidad.  

---

## ✨ Características Principales

- Registro de productos en el inventario.
- Actualización de información de productos existentes.
- Eliminación de productos.
- Visualización del inventario completo.
- Organización en **módulos**:
  - `producto.py` → Define la clase `Producto`.
  - `inventario.py` → Define la clase `Inventario` y sus métodos de gestión.
  - `main.py` → Interfaz de usuario en consola para interactuar con el sistema.

---

## 🆕 Actualización: Sistema Mejorado con Archivos y Excepciones

En esta nueva versión, el sistema se mejora para ser más **robusto y persistente**, implementando las siguientes funcionalidades:

### 📂 Almacenamiento en Archivos
- Los cambios realizados en el inventario (agregar, actualizar, eliminar) ahora se guardan en un archivo `inventario.txt`.
- Permite **persistencia de datos**, de modo que el inventario no se pierde al cerrar el programa.

### 📥 Recuperación de Inventarios
- Al iniciar el programa, se carga automáticamente la información de `inventario.txt`.
- Si el archivo no existe, se crea automáticamente.

### ⚠️ Manejo de Excepciones
- Se manejan errores comunes en la manipulación de archivos:
  - `FileNotFoundError`
  - `PermissionError`
  - Errores por archivos corruptos
- El sistema notifica al usuario en caso de éxito o fallo en operaciones con archivos.

### 💻 Interfaz de Usuario Mejorada
- Ahora la consola muestra mensajes más claros:
  - Confirmaciones cuando un producto es añadido al archivo.
  - Advertencias cuando ocurre un error en la lectura o escritura.
