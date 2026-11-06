# 🎮 Prototipos de Videojuegos con IA — Pygame

¡Bienvenido a mi colección de videojuegos interactivos! Este repositorio contiene dos prototipos desarrollados en Python utilizando la librería **Pygame**. Ambos proyectos han sido compilados en archivos ejecutables portátiles (`.exe`) para Windows, listos para jugar sin necesidad de instalar intérpretes ni dependencias externas.

---

## 🚀 Cómo descargar y jugar (Windows)

1. Dirígete a la sección de **[Releases](https://github.com)** ubicada en la columna derecha de esta página.
2. Descarga el paquete comprimido **`Juegos_IA.zip`** del lanzamiento más reciente.
3. Descomprime el archivo `.zip` en cualquier directorio de tu computadora.
4. Abre la carpeta resultante y ejecuta cualquiera de los archivos `.exe` para iniciar la simulación.

---

## 🕹️ Catálogo de Juegos y Controles

### 1️⃣ Mario Game Prototipo (1er Nivel)
Una recreación fiel al estilo arcade retro que emula las físicas y mecánicas clásicas del legendario plataformas en un nivel lineal de 3000 píxeles de extensión, con scroll de cámara inteligente y potenciadores activos.

* **Mecánicas:** Bloques de monedas rompibles, flores de fuego funcionales, eliminación de enemigos por colisión vertical (pisada) y abismos reactivos con pérdida de vidas.
* **⌨️ Controles:**
  * **Caminar a la Izquierda:** Flecha Izquierda `←` o Tecla `A`
  * **Caminar a la Derecha:** Flecha Derecha `→` o Tecla `D`
  * **Saltar:** Barra Espaciadora `Espacio`, Flecha Arriba `↑` o Tecla `W`
  * **Disparar Bolas de Fuego (Estado Fire):** Tecla `F` o Teclas `Shift` (Izquierdo / Derecho)
  * **Pausar / Reanudar:** Tecla `P`
  * **Reiniciar Nivel:** Tecla `R`

### 2️⃣ Coyote vs Correcaminos: Desierto ACME
Un juego de persecución estratégica con vista aérea que te permite experimentar el eterno conflicto de los dibujos animados mediante dos modalidades de juego dinámicas.

* **Mecánicas:** Cuenta con un **Modo 1 Jugador contra una IA Predictiva** (que analiza las últimas 30 trayectorias del jugador para interceptarlo en su ruta) y un **Modo 2 Jugadores Locales**. Incluye potenciadores de velocidad (Alpiste) y trampas explosivas desplegables (Cajas ACME).
* **⌨️ Controles:**
  * **Jugador 1 (Escape / Caza):** Flechas Direccionales `←` `↑` `↓` `→`
  * **Jugador 2 (Modo Local):** Teclas `W` (Arriba), `A` (Izquierda), `S` (Abajo), `D` (Derecha)
  * **Pausar:** Tecla `P` o Tecla `Esc`
  * **Menú de Pausa (Opciones):** Tecla `Enter` (Reanudar) o Tecla `M` (Volver al menú)
  * **Pantalla de Game Over:** Tecla `R` (Reintentar partida rápida) o Tecla `M` (Menú Principal)

---

## 🛠️ Tecnologías e Implementación Técnica

* **Lenguaje Base:** Python 3.12 (Entorno de ejecución estable para desarrollo de videojuegos de baja latencia).
* **Motor Gráfico y de Audio:** `pygame` y `pygame.mixer` para el manejo seguro de canales de sonido simultáneos (BGM y SFX).
* **Compilación:** Estructura modular compatible con `PyInstaller` mediante un sistema de resolución dinámica de rutas absolutas (`sys._MEIPASS`), previniendo errores de lectura de assets multimedia en Windows.

