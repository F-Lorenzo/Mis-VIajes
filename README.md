# Mis Viajes

Web app (PWA) para conductores de apps (Uber, DiDi, Cabify, inDrive): registrá cada jornada y mirá cuánto ganaste en limpio.

- Ganancia neta por día, semana, mes o total, y por hora, por km y por día.
- **Nafta de trabajo vs. personal**: con el rendimiento del auto (km/l) y el precio del litro, calcula la nafta de cada jornada según los km de trabajo y la separa de lo que cargaste en el tanque.
- Desgaste por km opcional (service, cubiertas, aceite).
- Funciona sin internet y se instala como app.
- Los datos quedan en el celular. Desde Ajustes → *Hacer copia de seguridad* se exporta un `.json` que se puede mandar por WhatsApp y restaurar después.

## Instalar en el celu

1. Abrí el link publicado (por ejemplo, el de Vercel) desde el celu.
2. **Android (Chrome):** menú ⋮ → *Instalar app*. **iPhone (Safari):** Compartir → *Agregar a inicio*.

## Publicar

Es un sitio estático, sin build: `index.html`, `manifest.webmanifest`, `sw.js` e `icons/`.
Sirve en Vercel (importar el repo, framework "Other"), Netlify o GitHub Pages. Tiene que ir por HTTPS para que se pueda instalar.

Cuando cambies archivos, subí el número de `CACHE` en `sw.js` para que los celulares tomen la versión nueva.

## APK (opcional)

Con la app ya publicada, se puede generar un APK en [pwabuilder.com](https://www.pwabuilder.com) pegando la URL.
