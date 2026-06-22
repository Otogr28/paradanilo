# Custom Companions — para Danilo 🐺

Mini-paquete para probar el mod **Custom Companions** (mod propio) con todas sus
dependencias. Solo tenés que instalar Forge y copiar la carpeta `mods/`.

---

## 1. Versión exacta que tenés que instalar

| Cosa | Versión |
|------|---------|
| **Minecraft** | **1.20.1** |
| **Forge** | **1.20.1 - 47.4.0** (o cualquier 47.4.x) |
| **Java** | **17** (lo pide Minecraft 1.20.1). En Windows, el instalador `.exe` de SKlauncher ya trae Java incluido. |

> ⚠️ **Tiene que ser 1.20.1 con Forge.** Si instalás otra versión de Minecraft
> (1.21, 1.20.4, etc.) o Fabric/NeoForge, los mods **no cargan** y el juego crashea.

Descargá el **instalador de Forge** desde la web oficial:
**https://files.minecraftforge.net/net/minecraftforge/forge/index_1.20.1.html**
→ buscá la versión **47.4.0** → botón **"Installer"**.

---

## 2. Qué hay en este paquete

Carpeta `mods/` con **10 archivos `.jar`** (Custom Companions + sus 9 dependencias).
**Todos van sí o sí**, no saques ninguno:

| Archivo | Qué es |
|---------|--------|
| `customcompanions-0.1.70.jar` | **El mod principal** (los compañeros) |
| `geckolib-forge-1.20.1-4.8.3.jar` | Motor de modelos/animaciones (obligatorio) |
| `ars_nouveau-1.20.1-4.12.7-all.jar` | Dependencia |
| `curios-309927-6418456.jar` | Slots de accesorios (dep) |
| `epic-fight-20.14.17-mc1.20.1-forge.jar` | Sistema de combate (dep) |
| `ldlib-626676-7809449.jar` | Librería (dep) |
| `more-bows-and-arrows-888468-6843671.jar` | Dependencia |
| `monolib-968432-7974599.jar` | Librería (dep) |
| `pk-craft-1382404-7902624.jar` | Dependencia |
| `mixinextras-forge-0.4.1.jar` | Librería de mixins (dep) |

> 📌 Estas mismas versiones son las que corren en el server, así que están probadas
> y son compatibles entre ellas. No las mezcles con otras versiones.

---

## 3. Tutorial: instalar todo en SKlauncher

> Basado en la documentación oficial de SKlauncher
> (https://docs.skmedix.pl/modding/mod-loaders/forge).

### Paso 1 — Tener SKlauncher y abrir Minecraft 1.20.1 una vez
1. Si no lo tenés, bajá SKlauncher de la web **oficial**: **https://skmedix.pl/downloads**
   (Windows: el **Setup `.exe`** ya trae Java incluido, es lo más fácil. Linux/Mac: el `.jar`).
2. Abrí SKlauncher, logueate, y en el selector de versiones elegí **`release 1.20.1`**
   y dale **Play una vez**. Dejá que cargue hasta el menú principal y cerrá el juego.
   *(Esto crea la carpeta del juego y el perfil base de 1.20.1 — Forge lo necesita.)*

### Paso 2 — Instalar Forge 1.20.1 - 47.4.0
1. Abrí el instalador de Forge que bajaste (`forge-1.20.1-47.4.0-installer.jar`).
   Si te pide con qué abrirlo → con **Java**.
   *(Si hacés doble clic y no pasa nada, abrí una terminal en esa carpeta y corré:
   `java -jar forge-1.20.1-47.4.0-installer.jar`)*
2. En la ventana del instalador, elegí **"Install client"**.
3. Fijate que la ruta de instalación apunte a tu carpeta de Minecraft (`.minecraft`).
   - Windows: `C:\Users\TU_USUARIO\AppData\Roaming\.minecraft`
   - Si usás SKlauncher con esa carpeta por defecto, ya está bien.
4. Dale **OK** y esperá el mensaje de éxito ("successfully installed").

### Paso 3 — Que SKlauncher detecte el Forge
1. Volvé a abrir **SKlauncher**.
2. En el selector de versiones ahora va a aparecer una opción nueva que dice
   **`forge`** (algo como `1.20.1-forge-47.4.0`). **Seleccionala.**

### Paso 4 — Copiar los mods
1. Andá a tu carpeta de Minecraft (`.minecraft`) y buscá (o creá) la carpeta **`mods`**.
   - El nombre tiene que ser **exactamente `mods`**, en minúsculas. No `Mods` ni `mod`.
2. Copiá **los 10 `.jar`** de la carpeta `mods/` de este paquete **adentro** de esa
   carpeta `mods` de tu `.minecraft`.

   > ⚠️ **Si en SKlauncher configuraste un "Game Directory" / carpeta de juego custom**
   > para este perfil, entonces la carpeta `mods` va **adentro de esa carpeta custom**,
   > no en `.minecraft`. Es el error #1 por el que "no detecta los mods".

### Paso 5 — Jugar
1. En SKlauncher, con la versión **forge** seleccionada, dale **Play**.
2. En la pantalla de título, abajo a la izquierda tiene que decir que cargó Forge,
   y en **Mods** (botón del menú) deberían aparecer Custom Companions y las deps.

---

## 4. Si algo falla

- **"no se ve la versión forge" en SKlauncher** → cerrá y volvé a abrir SKlauncher;
  asegurate de que el instalador de Forge apuntó a la **misma** `.minecraft` que usa
  SKlauncher.
- **Crashea al cargar** → casi siempre es porque **falta un `.jar`** o porque instalaste
  **otra versión** que no es 1.20.1 / Forge 47.4.x. Verificá que estén los **10** jars.
- **"Incompatible / wrong Minecraft version"** → estás en una versión que no es 1.20.1.
- **Pantalla "Mojang/Java"** o error de Java → necesitás **Java 17** instalado.

Cualquier cosa, mandale captura del crash a Oto. 🎮
