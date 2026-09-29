# Participantes Automation

Repositorio canónico reconstruido desde el proyecto real `Participantes` de Google Drive.

## Propósito observado
El programa toma una transcripción de Whisper, carga un prompt de instrucciones y automatiza su envío a ChatGPT mediante Selenium y Microsoft Edge. Después intenta extraer la respuesta y guardarla como archivo de texto.

## Tecnologías observadas
- Python
- Selenium WebDriver
- Microsoft Edge / Selenium Manager
- pyperclip

## Estructura
- `main.py`: resolución de entradas, ejecución y guardado del resultado.
- `config.py`: versión portable de la configuración; las rutas privadas de la estación original se sustituyeron por variables de entorno y rutas relativas.
- `src/selenium_runner.py`: carga de archivo, envío del prompt y extracción de la respuesta.

## Variables de entorno opcionales
- `PARTICIPANTES_INSTRUCCIONES`
- `PARTICIPANTES_WHISPER`
- `PARTICIPANTES_SALIDA`

## Exclusiones
No se versionan perfiles del navegador, cookies, sesiones, drivers `.exe`, caches ni archivos de entrada/salida locales.
