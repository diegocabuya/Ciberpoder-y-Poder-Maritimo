# Cómo subir el sitio al repositorio

Este paquete contiene la portada del proyecto, el README y todos los materiales
organizados en carpetas. Sigue **una** de estas dos vías.

---

## Opción A — Por la web (la más sencilla, sin comandos)

1. Entra a **https://github.com/diegocabuya/Ciberpoder-y-Poder-Maritimo**
2. Haz clic en **Add file → Upload files**.
3. **Arrastra todo el contenido de este paquete** (las carpetas `docs`, `simulador`,
   `presentacion`, `infografia`, `figuras` y los archivos `index.html`, `README.md`,
   `LICENSE`, `.nojekyll`). GitHub conserva la estructura de carpetas al arrastrarlas.
4. Escribe un mensaje de commit, por ejemplo: *"Portada del proyecto + materiales"*.
5. Haz clic en **Commit changes**.

> El archivo `.nojekyll` es importante: asegura que GitHub Pages sirva todos los
> archivos tal cual. Si al arrastrar no aparece (algunos navegadores ocultan los
> archivos que empiezan por punto), créalo con **Add file → Create new file**,
> nómbralo `.nojekyll` y deja el contenido vacío.

---

## Opción B — Por línea de comandos (Git)

```bash
# 1. Clona el repositorio (si aún no lo tienes en tu equipo)
git clone https://github.com/diegocabuya/Ciberpoder-y-Poder-Maritimo.git
cd Ciberpoder-y-Poder-Maritimo

# 2. Copia aquí TODO el contenido de este paquete
#    (index.html, README.md, LICENSE, .nojekyll y las carpetas)

# 3. Sube los cambios
git add .
git commit -m "Portada del proyecto + materiales completos"
git push origin main
```

---

## Activar GitHub Pages (si no está activo)

1. En el repositorio: **Settings → Pages**.
2. En *Source*, elige **Deploy from a branch**.
3. Rama **main**, carpeta **/ (root)**. Guarda.
4. En 1–2 minutos, tu sitio estará en vivo en:
   **https://diegocabuya.github.io/Ciberpoder-y-Poder-Maritimo/**

El simulador seguirá funcionando en su ruta actual, y ahora también desde la portada.

---

## Verificación rápida tras subir

- La portada abre en `https://diegocabuya.github.io/Ciberpoder-y-Poder-Maritimo/`
- El botón **"Abrir simulador"** carga el modelo interactivo.
- La galería de ecuaciones amplía cada lámina al hacer clic.
- Los enlaces de **Descargas** bajan cada archivo.

Si alguna imagen no carga, confirma que la carpeta `figuras/` se subió completa
(con sus subcarpetas `ecuaciones/` y `esquemas/`).
