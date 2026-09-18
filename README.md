# MTG Life Counter

Contador de vidas para Magic: The Gathering hecho con **HTML, CSS y JavaScript puros** (sin frameworks). Está pensado para **iPad 2** (iOS 9 / Safari 9) y se publica como sitio estático en **GitHub Pages**.

Inspirado en [lifecounter.app](https://lifecounter.app/), con la mesa a pantalla completa, daño de comandante, contadores, dados y temporizador.

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub e sube estos archivos (mantén `index.html` en la raíz).
2. En el repositorio: **Settings → Pages**.
3. En **Source** elige la rama `main` (o `master`) y la carpeta `/ (root)`.
4. Guarda y espera uno o dos minutos.
5. Abre la URL que GitHub muestra, por ejemplo `https://TU-USUARIO.github.io/lifecounter/`.

En el iPad 2 usa Safari para abrir esa URL. Si la página no carga, comprueba que termina en `/` y que Pages quedó en la raíz del repo.

## Pantalla completa en iPad 2

1. Abre la app en **Safari**.
2. Toca el botón **Compartir**.
3. Elige **Añadir a pantalla de inicio**.
4. Ábrela desde el icono: se ve a pantalla completa, sin la barra de Safari.

## Cómo se usa

- **Lado izquierdo / derecho** de cada jugador: resta o suma 1 vida.
- **Mantener pulsado** + o −: cambia de 10 en 10.
- **Tocar el número**: teclado para poner la vida exacta.
- **Deslizar izquierda / derecha**: daño de comandante de cada rival (letal a 21).
- **Menú (☰)**: nombre, color, partner, veneno, impuesto, energía, experiencia, storm, carga, eliminar/revivir.
- **Dados**: d4–d20, varias tiradas, moneda y high roll (quién empieza).
- **Turno y reloj**: controlan el ritmo de la mesa.
- **Cartas**: busca en Scryfall (hace falta internet).
- **Planar**: dado de Planechase (en blanco / caos / planeswalk).

La partida se guarda sola en el navegador (`localStorage`).

## Compatibilidad

Funciona sin build, sin `npm` y sin ES6 modules. Evita CSS Grid, `fetch`, `async/await` y Service Workers para que Safari del iPad 2 pueda ejecutarla. También anda en navegadores actuales.

## Probar en el PC

Sirve la carpeta con cualquier servidor estático, por ejemplo:

```bash
python -m http.server 8080
```

Luego abre `http://localhost:8080`.
