
# MSN

Este script de Python permite recibir mensajes de texto y archivos a través de Telegram y guardarlos automáticamente en el directorio del script. También permite enviar archivos a un usuario específico usando su `USER_ID`.  

---

## Características

- Guarda mensajes de texto enviados al bot en archivos `.txt` con timestamp.
- Guarda archivos recibidos (documentos, fotos, audios, videos, voice notes, stickers y animaciones) con su nombre original o un nombre generado automáticamente.
- Permite enviar archivos a un usuario específico mediante un comando de línea.
- Compatible con múltiples tipos de archivo de Telegram.
- Logs simples en la consola para seguimiento de actividad.

---

## Requisitos

- Python 3.6 o superior
- Biblioteca `pyTelegramBotAPI` (telebot)

Instalación de la dependencia:

```bash
git clone https://github.com/packarazy/msn.git
pip install pyTelegramBotAPI
```


---

Configuración

1. Crea un bot de Telegram usando @BotFather y obtén el TOKEN.


2. Obtén tu USER_ID (el ID del usuario al que quieres enviar archivos).


3. Edita las variables en el script:



TOKEN = "TU_TOKEN_AQUI"
USER_ID = 123456789  # Reemplaza con tu ID


---

Uso

1. Modo bot (escucha mensajes y archivos)

Ejecuta el script sin argumentos:

python3 bot.py

El bot iniciará y escuchará mensajes y archivos enviados.

Los mensajes de texto se guardarán como archivos .txt con nombre trino_YYYY-MM-DD_HH-MM-SS.txt.

Los archivos se guardarán con su nombre original o uno generado automáticamente según el tipo.


2. Modo envío de archivo

Puedes enviar un archivo al USER_ID directamente desde la línea de comandos:

python3 bot.py ruta/al/archivo.txt

El script verificará que el archivo exista y no esté vacío antes de enviarlo.

Se enviará al usuario especificado en USER_ID usando Telegram.



---

Estructura de archivos

bot.py → Script principal

Archivos guardados → en el mismo directorio que bot.py



---

Tipos de archivo soportados

Textos (text)

Documentos (document)

Fotos (photo)

Audios (audio)

Voice notes (voice)

Videos (video)

Animaciones/GIF (animation)

Stickers (sticker)



---

Notas de seguridad

Asegúrate de no compartir tu TOKEN públicamente.

Los archivos se guardan localmente en el mismo directorio que el script.

Para producción, considera mecanismos de backup o cifrado si manejas datos sensibles.



---

Contribuciones

Si quieres mejorar el bot:

1. Haz un fork del repositorio.


2. Crea tu branch: git checkout -b mi-rama


3. Haz tus cambios y haz commit.


4. Envía un pull request.




---

Licencia

Este proyecto está bajo la MIT License.

---

