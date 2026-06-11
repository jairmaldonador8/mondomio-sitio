# Festival de Fin de Cursos — Mondomío Kínder

Landing page de una sola página para el Festival de Fin de Cursos (tema Zootopia). Incluye las tres funciones del día: Babies (10:30 AM), Maternal (11:30 AM) y Kids (12:30 PM, con ceremonia de graduación).

## Estructura

```
mondomio-festival/
├── index.html            ← la página
└── assets/
    ├── img/              ← logo e ilustraciones (PNG)
    └── fonts/            ← fuentes Uniform (woff2)
```

Todo usa rutas relativas, así que funciona tal cual en cualquier hosting estático.

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub (por ejemplo `festival-mondomio`).
2. Sube **el contenido de esta carpeta** (que `index.html` quede en la raíz del repo, no dentro de otra carpeta).
3. En el repo ve a **Settings → Pages**.
4. En **Source** elige la rama `main` y la carpeta `/ (root)`. Guarda.
5. En 1–2 minutos tu sitio queda en `https://TU-USUARIO.github.io/festival-mondomio/`.

### Por terminal (opcional)

```bash
cd mondomio-festival
git init
git add .
git commit -m "Landing Festival de Fin de Cursos"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/festival-mondomio.git
git push -u origin main
```

Luego activa GitHub Pages en Settings → Pages como arriba.

## Notas

- Toda la información se ve aunque el navegador tenga JavaScript desactivado; las animaciones de aparición son solo un extra.
- Falta la **fecha** del festival (no venía en los materiales). Para agregarla, busca en `index.html` la sección "Horario del día" (`id="funciones"`) o "Detalles" (`id="detalles"`).
- Las tres funciones están en la sección "Horario del día"; cada tarjeta lleva a su programa (`#prog-babies`, `#prog-maternal`, `#prog-kids`). La graduación de Kids está en `id="graduacion"`.
