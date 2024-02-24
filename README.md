<h1 align="center">
	YTDLnis
</h1>

<h3 align="center">
	YTDLnis es un descargador de video/audio gratuito y de código abierto que utiliza yt-dlp para Android 6.0 en adelante.
</h3>
<h4 align="center">
	[Creado por Arturo Cervantes. Original en DEV]
</h4>

<div align="center">

[![Descarga en Github](https://custom-icon-badges.herokuapp.com/badge/Download-blue?style=for-the-badge&logo=download&logoColor=white)](https://github.com/Arturo254/YTDLnis/releases/tag/YTDLnis)

![CI](https://github.com/deniscerri/ytdlnis/actions/workflows/android.yml/badge.svg?branch=main&event=pull)
[![Vista previa de la versión](https://img.shields.io/github/release/deniscerri/ytdlnis.svg?maxAge=3600&include_prereleases&label=vista%20previa)](https://github.com/Arturo254/YTDLnis/releases)
[![descargas](https://img.shields.io/github/downloads/deniscerri/ytdlnis/total?style=flat-square)](https://github.com/Arturo254/YTDLnis/releases)
[![Estado de traducción](https://hosted.weblate.org/widgets/ytdlnis/-/svg-badge.svg)](https://hosted.weblate.org/engage/ytdlnis/?utm_source=widget)
[![comunidad](https://img.shields.io/badge/Discord-YTDLnis-blueviolet?style=flat-square&logo=discord)](https://arturo-cervantes.netlify.app/)
[![comunidad](https://img.shields.io/badge/Telegram-YTDLnis-blue?style=flat-square&logo=telegram)](https://t.me/ArturoNomas7271)
[![comunidad](https://img.shields.io/badge/Telegram-Actualizaciones-rojo?style=flat-square&logo=telegram)](https://t.me/ArturoNomas7271)

### Los enlaces anteriores son las únicas fuentes confiables de YTDLnis. Todo lo demás no está relacionado conmigo.

</div>

## 💡 Características:

- descarga archivos de audio/video de más de <a href="https://github.com/yt-dlp/yt-dlp/blob/master/supportedsites.md">1000 sitios web</a>
- procesa listas de reproducción
    - edita cada elemento de la lista de reproducción por separado, al igual que en un elemento de descarga normal.
    - selecciona un formato común para todos los elementos y/o selecciona varios formatos de audio en caso de que los estés descargando como video
    - elige una ruta de descarga para todos los elementos
    - elige una plantilla de nombre de archivo para todos los elementos
    - actualiza por lotes el tipo de descarga a audio/video/comando personalizado con un clic
- encola descargas y prográmalas por fecha y hora
    - también puedes programar varios elementos al mismo tiempo
- descarga varios elementos al mismo tiempo
- usa comandos y plantillas personalizados o entra en modo yt-dlp completo con un terminal integrado
    - puedes hacer copias de seguridad y restaurar plantillas para compartirlas con tus amigos
- soporte de COOKIES. Inicia sesión con tus cuentas y descarga videos privados/no disponibles, desbloquea formatos premium, etc.
- corta videos en función de marcas de tiempo y capítulos de video (Esta función de yt-dlp es experimental en el proyecto original)
    - puedes hacer cortes ilimitados
- elimina elementos de sponsorblock del elemento
    - incrustrarlos como capítulos en tu video
- incrusta subtítulos/metadatos/capítulos, etc.
- modifica metadatos como título y autor
- divide el elemento en archivos separados
- selecciona diferentes formatos de descarga
- tarjeta inferior directamente desde el menú de compartir, no es necesario abrir la aplicación
    - puedes crear un archivo txt y llenarlo con enlaces/listas de reproducción/búsquedas separadas por una nueva línea y la aplicación los procesará
- busca o inserta un enlace desde la aplicación
    - puedes apilar búsquedas para procesarlas al mismo tiempo
- registra las descargas en caso de problemas
- vuelve a descargar descargas canceladas o fallidas
    - puedes usar gestos para deslizar hacia la izquierda para volver a descargar y hacia la derecha para eliminar
    - puedes hacer clic largo en el botón de volver a descargar en la hoja de detalles para mostrar la tarjeta de descarga para más funcionalidades
- modo incógnito cuando no quieres guardar un historial de descargas o registros
- modo de descarga rápida
    - descarga inmediatamente sin tener que esperar que los datos se procesen. Desactiva la tarjeta inferior y comenzará al instante
- abre/comparte archivos descargados directamente desde la notificación final
- la mayoría de las características de yt-dlp están implementadas, se aceptan sugerencias
- Interfaz de Material You
- Opciones de personalización
- Funciones de copia de seguridad y restauración. (Casi todo se puede respaldar)
- Arquitectura MVVM con WorkManager


## 🔑 Connect with ReVanced

El nombre del paquete de la aplicación es "com.deniscerri.ytdl"

## 📝 Ayuda a Traducir en Weblate
<div align="center">
  <a href="https://hosted.weblate.org/engage/ytdlnis/">
    <img src="https://hosted.weblate.org/widgets/ytdlnis/-/strings/open-graph.png" alt="Estado de traducción" />
  </a>
</div>

<div align="center">
  <a href="https://hosted.weblate.org/engage/ytdlnis/">
    <img src="https://hosted.weblate.org/widgets/ytdlnis/-/multi-auto.svg" alt="Estado de traducción" />
  </a>
</div>

## ✔️🤖 Conéctate con Tasker / Macrodroid, etc.

Puedes usar intents en aplicaciones como Tasker o Macrodroid para enviar comandos a la aplicación y ejecutar una descarga sin interacción del usuario.
Variables aceptadas:

- <b>TYPE</b> -> puede ser: audio, video, comando.
- <b>BACKGROUND</b> -> puede ser: true, false. Si es true, la aplicación no mostrará la tarjeta de descarga y ejecutará la descarga en segundo plano.
- <b>COMMAND</b> -> si tu tipo preferido es audio/video o has definido la variable TYPE como uno de ellos, esto se agregará a tu cadena de comandos adicionales. Si el tipo es comando, se usará todo el comando que escribiste aquí para la descarga.

### Ejemplo de Tasker para descargar un audio en segundo plano
1. Crea una tarea de Envío de Intentos
2. Acción: android.intent.action.SEND
3. Categoría: Predeterminado
4. Tipo MIME: text/*
5. Adicional: android.intent.extra.TEXT: url (en lugar de url, escribe el enlace del video que deseas descargar)
6. Adicional: TYPE: audio
7. Adicional: BACKGROUND: true

## 😇 Contribuciones

Si deseas contribuir, por favor lee la sección de [Contribuciones](https://wa.me/5576847925) .

## 📄 Licencia

[GNU GPL v3.0](https://github.com/deniscerri/ytdlnis/blob/main/LICENSE)

⚠️ Advertencia <br>

Excepto por el código fuente con licencia GPLv3, se prohíbe a todos los demás usar el nombre 'YTDLnis' como aplicación de descarga, igualmente para sus derivados. Los derivados incluyen, pero no se limitan a bifurcaciones y compilaciones no oficiales.

## 🙏 Agradecimientos

- [yt-dlp](https://github.com/yt-dlp/yt-dlp) y sus colaboradores por hacer posible esta herramienta. Sin ellos, esta aplicación no existiría.
- [youtubedl-android](https://github.com/yausername/youtubedl-android) por portar yt-dlp a Android.
- [dvd](https://github.com/yausername/dvd) por mostrar cómo implementar youtubedl-android.
- [seal](https://github.com/JunkFood02/Seal) por ciertos elementos de diseño y funciones que quería usar al iniciar el desarrollo de esta aplicación.
- [decipher3114](https://github.com/decipher3114) por el icono de la aplicación.
  
y muchas otras personas desconocidas en foros de internet.  
