# Portafolio — Fernando Pur

Sitio estático (HTML/CSS/JS puro, sin build step). Listo para GitHub → Cloudflare Pages.

## Estructura

```
index.html
robots.txt
sitemap.xml
llms.txt
assets/img/
  sobre-mi/
  experiencia/
  portafolio/
    activaciones/
    branding/
    campanas/
    fotos/
```

## Subir a GitHub

```bash
git init
git add .
git commit -m "Portafolio inicial"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/TU-REPO.git
git push -u origin main
```

## Conectar a Cloudflare Pages

1. Cloudflare Dashboard → Workers & Pages → Create → Pages → Connect to Git.
2. Selecciona el repositorio.
3. Build settings: framework preset "None", build command vacío, output directory `/` (raíz).
4. Deploy.

## Pendiente antes o después de publicar

- **Dominio real**: el `index.html`, `robots.txt` y `sitemap.xml` usan el marcador `https://fernando-pur-portafolio.pages.dev` como placeholder. Cuando Cloudflare asigne el subdominio final (o conectes un dominio propio), reemplaza esa URL en los 3 archivos (busca "fernando-pur-portafolio.pages.dev").
- **Google Search Console**: una vez publicado, da de alta la propiedad y envía `sitemap.xml` para que Google indexe el sitio más rápido.
- **Favicon**: se generó automáticamente a partir de la foto de retrato (`favicon.png`, `apple-touch-icon.png`). Puedes reemplazarlo por un logo si prefieres.
