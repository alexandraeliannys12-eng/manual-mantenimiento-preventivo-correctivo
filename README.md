# Manual de mantenimiento preventivo y correctivo

Sitio web estático con un manual de usuario sobre el mantenimiento preventivo y correctivo de laptops y computadoras de escritorio, con guías de diagnóstico desde el sistema operativo.

- **Autora:** Eliannys López (C.I: 31.781.126)
- **Asignatura:** Sistemas Operativos
- **Tecnologías:** HTML5 y CSS3 (sin dependencias ni paso de compilación)

## Estructura

```text
manual-mantenimiento/
├── public/                 Sitio publicable
│   ├── index.html          Inicio
│   ├── preventivo.html     Mantenimiento preventivo
│   ├── correctivo.html     Mantenimiento correctivo
│   ├── laptop.html         Laptop (incluye diagnóstico)
│   ├── escritorio.html     PC de escritorio (incluye diagnóstico)
│   ├── referencias.html    Bibliografía (APA 7)
│   ├── 404.html            Página de error
│   ├── css/styles.css      Estilos
│   └── img/                Fotografías e íconos
├── vercel.json             Configuración de despliegue
├── .editorconfig           Reglas de estilo del editor
└── .prettierrc             Reglas de formato
```

## Ejecutar en local

1. Abre la carpeta en VS Code e instala las extensiones recomendadas.
2. Clic derecho en `public/index.html` → **Open with Live Server**.

## Desplegar en Vercel

1. Sube el repositorio a GitHub (pasos abajo).
2. En [vercel.com/new](https://vercel.com/new) importa el repositorio.
3. Deja **Framework Preset** en `Other`; `vercel.json` ya define `public` como directorio de salida.
4. Pulsa **Deploy**.

También puedes usar la CLI: `npx vercel` (vista previa) y `npx vercel --prod` (producción).

## Subir a GitHub

```bash
git init
git add .
git commit -m "feat: manual de mantenimiento de equipos de cómputo"
git branch -M main
git remote add origin https://github.com/<usuario>/<repositorio>.git
git push -u origin main
```

## Formato del código

El proyecto usa [Prettier](https://prettier.io/) con la extensión de VS Code (formato al guardar). Para formatear manualmente: `npx prettier --write "public/**/*.{html,css}"`.

## Licencia

Código bajo licencia MIT (ver `LICENSE`). Las fotografías pertenecen a sus respectivos autores.
