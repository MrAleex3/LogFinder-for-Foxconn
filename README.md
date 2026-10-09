# LogFinderFox

Herramienta desarrollada en AutoHotkey v1.1 para buscar y gestionar archivos de log de forma rápida y automatizada. Está pensada para entornos de producción y calidad: permite localizar, filtrar y copiar registros mediante distintos modos de búsqueda, ya sea simple, por filtro, múltiple o automática desde un archivo base.

Los filtros disponibles son PPID, fecha específica, estado (`PASS`, `FAIL`, etc.) y System ID.

![Interfaz](https://github.com/user-attachments/assets/bce549b6-428b-46e7-b88a-ddeb62bf3810)

## Características

- Búsqueda por PPID, con opción de filtrar por fecha o estado (`PASS` / `FAIL`).
- Búsqueda avanzada que combina PPID y Project Code.
- Soporte para varios PPID al mismo tiempo, con carpetas organizadas por resultado.
- Modo automático que lee un archivo `.txt` con parámetros como hora de referencia y estado para cada PPID.
- Filtrado por hora (`End time`) para seleccionar el archivo más cercano a una hora específica.
- Copia organizada en carpetas de resultados (`resultado`, `resultado_auto`, `resultado_automatico`).
- Validaciones para los errores más comunes: serial vacío, modelo inválido o archivos inexistentes.

## Requisitos

- Windows 10 o superior.
- AutoHotkey v1.1 instalado.
- Acceso de red al directorio configurado en `RutaDeLogs.ini`.

## Estructura

- `RutaDeLogs.ini`: define el directorio donde están los archivos de log a analizar.
- `BuscadorDeDB1.txt`: parámetros de entrada para el modo automático.
- `LogFinderFox.ahk`: script principal de la herramienta.
- `resultado/`, `resultado_auto/`, `resultado_automatico/`: carpetas de salida generadas según el modo usado.

## Licencia

Este proyecto está bajo la Licencia MIT.

## Autor

Alejandro Espinoza
Foxconn México
