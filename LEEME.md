# Recorrido 3D 🎯

App de puntuación para recorridos de tiro con arco 3D. Funciona en Android y en iPhone, se instala en la pantalla de inicio y funciona **sin conexión**.

## Publicarla en GitHub Pages (una sola vez, unos 5 minutos)

1. Entra en <https://github.com> e inicia sesión (o créate una cuenta gratuita).
2. Arriba a la derecha pulsa **＋ → New repository**.
   - **Repository name:** `recorrido3d`
   - Márcalo como **Public**.
   - Pulsa **Create repository**.
3. En el repositorio recién creado pulsa **uploading an existing file** (o **Add file → Upload files**).
4. Descomprime el ZIP en tu ordenador y **arrastra todo su contenido** a la página. Arrastra los archivos y la carpeta `icons`, no la carpeta que los contiene:
   - `index.html`
   - `manifest.webmanifest`
   - `sw.js`
   - `.nojekyll`
   - la carpeta `icons` completa
   - `LEEME.md`
5. Pulsa **Commit changes**.
6. Ve a **Settings → Pages**.
   - En **Source** elige **Deploy from a branch**.
   - En **Branch** elige **main** y la carpeta **/ (root)**, y pulsa **Save**.
7. Espera 1 o 2 minutos y recarga esa página. Aparecerá la dirección de tu app:
   **`https://TU-USUARIO.github.io/recorrido3d/`**

> El archivo `.nojekyll` empieza por un punto y en algunos ordenadores está oculto. Si no lo ves no pasa nada: la app funciona igual sin él.

## Instalarla en el móvil

**Android (Chrome):** abre la dirección y pulsa **Instalar** en la pantalla de Jornadas, o usa el menú ⋮ → **Instalar aplicación**.

**iPhone (Safari):** abre la dirección en **Safari**, pulsa **Compartir** (□↑) → **Añadir a pantalla de inicio**.

Después ábrela siempre desde el icono de la diana. En iPhone, los datos de la app instalada y los de Safari están separados.

Pasa el enlace por WhatsApp a los demás anotadores para que también la instalen.

## Cómo se usa en una tirada

1. **Jornadas → Nueva jornada.** Pon un nombre, la patrulla y el número de dianas (24 por defecto, 32 u otro).
2. **Tiradores.** Añade a cada tirador con su modalidad, sexo y edad. El orden de la lista es el orden en que aparecen al puntuar (con ↑ lo cambias).
3. **Puntuar.** En cada diana toca dos valores por tirador. La flecha más alta se coloca sola en primer lugar.
   - Para corregir, toca la flecha que está mal y luego el valor correcto.
   - ✕ borra las dos flechas de ese tirador en esa diana, y **↶ Deshacer** recupera el último cambio.
   - Al tocar el número de diana se abre el mapa con todas las dianas.

### Dos anotadores por patrulla
1. El anotador 1 crea la jornada y añade los tiradores.
2. Después pulsa **Tiradores → Pasar la patrulla al 2º anotador**, que le envía un mensaje de WhatsApp.
3. El anotador 2 abre la app y pulsa **Importar patrulla de WhatsApp**. Pega el mensaje y elige **Crear jornada con estos tiradores**.
4. Los dos anotan por separado durante el recorrido.
5. Al acabar, uno envía su patrulla (**Clasificación → Enviar patrulla**) y el otro la importa con **Comprobar con mis puntuaciones**. La app muestra las dianas que no coinciden y, en cada una, eliges qué valor se queda.

### Juntar todas las patrullas (organizador)
Cada patrulla envía su mensaje al organizador. Este, en su jornada, pulsa **Importar** y elige **Añadir a la clasificación**. Si una patrulla manda una versión más nueva, sus datos se actualizan sin duplicarse.

### Resultados
- Clasificación **general** o **por categorías** (modalidad + sexo + edad), con podio.
- **Desempate:** gana quien tenga más 11 y, si siguen empatados, más 10.
- Al tocar un tirador se abren sus estadísticas: media, porcentaje de 11, fallos, mejor diana y un gráfico de puntos por diana.
- Puedes compartir la clasificación como **texto** o como **imagen** por WhatsApp, o exportarla en **CSV** (se abre en Excel).

## Copias de seguridad
Los datos se guardan **solo en el móvil**. En **Ajustes → Exportar copia** puedes guardar un archivo, que luego se recupera con **Restaurar**.

## Si cambias la app más adelante
Cuando cambies `index.html`, edita también `sw.js` y sube el número de versión de la primera línea (por ejemplo, `recorrido3d-v1.0.0` → `recorrido3d-v1.0.1`). Así los móviles descargan la versión nueva. Puede hacer falta cerrar la app y abrirla dos veces.
