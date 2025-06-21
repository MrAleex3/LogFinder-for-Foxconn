# 🔍 LogFinderFox

**LogFinderFox** es una herramienta desarrollada en AutoHotkey v1.1 que permite buscar y gestionar archivos de log de manera rápida y automatizada. Está diseñada para entornos de producción y calidad, permitiendo la localización, filtrado y copia de registros mediante distintos modos de búsqueda: simple, por filtro, múltiple o automática desde un archivo base.

- ✅ PPID
- 📆 Fecha específica
- 🟩 Estado (`PASS`, `FAIL`, etc.)
- 🧩 SystemID



## 🚀 Funcionalidades

- 🔍 **Búsqueda por PPID** con opción de filtrar por **fecha** o **estado** (`PASS` / `FAIL`).
- 🧩 **Búsqueda avanzada** con combinación de `PPID` y `Project Code`.
- 📋 **Soporte para múltiples PPIDs** al mismo tiempo, con creación de carpetas organizadas.
- ⚙ **Modo automático** que lee un archivo `.txt` con parámetros como **hora de referencia** y **estado** para cada PPID.
- ⏱ **Filtrado inteligente por hora (`End time`)** para seleccionar el archivo más cercano a una hora específica.
- 📁 **Copia organizada** en carpetas de resultados (`resultado`, `resultado_auto`, `resultado_automatico`).
- 🔒 Interfaz protegida contra errores comunes (serial vacío, modelo inválido, archivos inexistentes).
- 🎨 Incluye una interfaz limpia y organizada para el usuario.

## 📷 Interfaz

![image](https://github.com/user-attachments/assets/bce549b6-428b-46e7-b88a-ddeb62bf3810)


## 🧰 Requisitos

- **Windows 10** o superior.
- **AutoHotkey v1.1** instalado.
- **Acceso de red** al directorio configurado en `RutaDeLogs.ini`.

## 🗂️ Estructura

- `RutaDeLogs.ini`: Define el directorio donde se encuentran los archivos log a analizar.
- `BuscadorDeDB1.txt`: Contiene los parámetros de entrada para el modo automático.
- `LogFinderFox.ahk`: Script principal de la herramienta.
- `resultado/`, `resultado_auto/`, `resultado_automatico/`: Carpetas de salida generadas automáticamente según el modo usado.

## 📝 Licencia

Este proyecto está bajo la [Licencia MIT](LICENSE).

## 🙋 Autor

**Jose Alejandro**  
Foxconn México · Proyecto personal para portafolio
