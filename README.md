# Chance 2 Change — SIM, Simulador de Carga

Sitio estático bilingüe (ES/EN). Sin build: se publica tal cual en Vercel.

## 1. Rutas a crear en GitHub (raíz del repo)

```
/ (raíz del repo)
├── index.html
├── README.md
└── assets/
    ├── logo-icon.jpg              ✅ favicon + logo del nav
    ├── banner.jpg                 ✅
    ├── video/
    │   ├── hero.mp4               ✅ video del hero (optimizado)
    │   ├── hero-poster.jpg        ✅
    │   ├── hueso-1.mp4            ⬜ videos del hueso rotando 3D
    │   ├── hueso-2.mp4            ⬜ (si no están, la sección se oculta sola)
    │   └── hueso-3.mp4            ⬜
    ├── img/
    │   ├── sim-tomografo.jpg      ✅
    │   ├── sim-ensamble.jpg       ⬜ final1.jpg
    │   ├── sim-piezas.jpg         ⬜ final2.jpg
    │   ├── sim-base.jpg           ⬜ base con medidas
    │   └── sim-figuras.jpg        ⬜ Figura 1 y Figura 2.jpg
    ├── logos/                     ⬜ PNG con fondo transparente
    │   ├── centro-rossi.png
    │   ├── swiss-medical.png
    │   ├── dupuytren.png
    │   ├── osde.png
    │   └── deragopyan.png         (si falta un logo, se muestra el nombre)
    └── docs/  (opcional: hoy los documentos abren desde Drive)
        ├── Despiece-SIM-B.pdf     ⬜
        ├── paper-clinico.pdf      ⬜
        ├── ficha-tecnica.pdf      ⬜
        ├── manual-patologias.pdf  ⬜
        └── casos-clinicos.pdf     ⬜
```

Nombres en minúscula, sin espacios ni acentos. Cada archivo debe pesar menos de 25 MB
(límite de subida web de GitHub); los videos del hueso idealmente < 3 MB cada uno.

## 2. Videos de YouTube y nota

Al final de `index.html`: `VIDEOS` → ID de YouTube en `id: ""`; `NEWS_URL` → link a la nota.

## 3. Subir a GitHub

1. github.com → **New repository** → nombre `chance2change` → Public → **Create**.
2. **uploading an existing file** → arrastrá `index.html`, `README.md` y la carpeta `assets` completa
   (GitHub mantiene las subcarpetas al arrastrar la carpeta) → **Commit changes**.
3. Para agregar archivos después: entrá a la carpeta (ej. `assets/logos`) → **Add file → Upload files**.

## 4. Conectar con Vercel

1. vercel.com → **Sign up / Log in with GitHub**.
2. **Add New → Project** → elegí `chance2change` → **Import**.
3. Framework Preset: **Other** · Root Directory: `./` · sin Build Command → **Deploy**.
4. Queda en `chance2change.vercel.app`. Cada commit en GitHub se publica solo en ~30 segundos.
5. Dominio propio: Project → **Settings → Domains** → agregá el dominio y copiá los DNS que indica Vercel en tu proveedor.

## 5. Después

Actualizá la URL en LinkedIn e Instagram.
