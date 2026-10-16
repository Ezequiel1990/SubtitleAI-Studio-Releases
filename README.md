# SubtitleAI Studio para Windows

Editor de subtítulos con IA local: elegí un video, generá y revisá los subtítulos, guardá un SRT o una copia MP4 con el texto integrado.

## Descargar

[Descargar la última versión](https://github.com/Ezequiel1990/SubtitleAI-Studio-Releases/releases/latest)

Ejecutá el archivo terminado en `windows-x64-setup.exe`. La instalación es por usuario y crea un acceso directo con icono en el escritorio. No requiere instalar Python.

## Requisitos

- Windows 10 2004 o posterior, 64 bits.
- Al menos 8 GB libres para instalar, más el espacio para los modelos y videos.
- El paquete incluye Python, Qt, FFmpeg/FFprobe y bibliotecas de ejecución. Los modelos Whisper y Ollama se instalan aparte y no están incluidos en la descarga de aproximadamente 1,5 GB.
- Para descargar Whisper desde la app, desmarcá «Solo modelos ya instalados». Se reutilizan los modelos previamente descargados en tu perfil.
- La traducción requiere [Ollama](https://ollama.com/download/windows) y el modelo `qwen3:8b`. Si no necesitás traducción, podés generar los subtítulos en el idioma original.

## Actualizaciones

La app instalada busca nuevas versiones al abrirse. También podés usar Ayuda → Buscar actualizaciones. La descarga verifica tamaño y SHA-256; la instalación se inicia con tu aceptación y conserva las sesiones y archivos guardados. No se instala mientras hay una generación o exportación activa.

Los datos de trabajo se guardan en `%LOCALAPPDATA%/SubtitleAI Studio`, separados de los archivos del programa. Los videos se procesan localmente. El repositorio solo distribuye instaladores y metadatos; no recibe tus videos ni subtítulos.

El instalador de la primera versión todavía no tiene firma Authenticode. Los avisos de dependencias se encuentran en `_internal/resources/THIRD_PARTY_NOTICES.md` y `_internal/resources/licenses` dentro de la instalación.

En cada Release, `latest.json` y `SHA256SUMS.txt` son archivos de actualización y verificación; para instalar, descargá el `.exe`.
