# 🚀 LiamWinmer Proton Layer

¡Bienvenido a **LiamWinmer**, una capa de compatibilidad personalizada para Steam Play (Steam Deck / Linux) basada en GE-Proton!

Este proyecto intercepta el lanzamiento de los juegos, genera un registro de actividad en el escritorio (`liamwinmer_log.txt`) y ejecuta los juegos utilizando el motor de GE-Proton.

---

## 🛠️ Guía de Instalación

Para que esta capa funcione en tu sistema, sigue estos sencillos pasos:

### 1. Requisitos Previos
Debes tener instalado **GE-Proton11-1** en tu Steam Deck o PC. Puedes instalarlo fácilmente usando la aplicación **ProtonUp-Qt** desde la tienda Discover en el Modo Escritorio.

### 2. Descargar e Instalar LiamWinmer
1. Descarga el código de este repositorio de GitHub.
2. Abre tu gestor de archivos (Dolphin) y ve a la siguiente ruta (activa los archivos ocultos con `Ctrl + H`):
   `~/.steam/steam/compatibilitytools.d/`
3. Crea una nueva carpeta llamada exactamente `LiamWinmer`.
4. Pega dentro de esa carpeta todos los archivos que descargaste de este repositorio (`proton`, `compatibilitytool.vdf`, `toolmanifest.vdf`, etc.).

### 3. Vincular el motor de GE-Proton (¡El paso clave!)
Como este repositorio no incluye los archivos pesados del motor, debes copiarlos de tu sistema:
1. Ve a la carpeta de tu instalación de GE-Proton. Normalmente está en:
   `~/.steam/steam/compatibilitytools.d/GE-Proton11-1/`
2. Copia la carpeta llamada **`files`**.
3. Vuelve a tu carpeta `LiamWinmer` y **pega** la carpeta `files` ahí dentro.

### 4. Dar permisos de ejecución
Abre una terminal (Konsole) y ejecuta el siguiente comando para asegurarte de que el script puente tenga permisos:
```bash
chmod +x ~/.steam/steam/compatibilitytools.d/LiamWinmer/proton
