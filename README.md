# Vantage, SIESA y WMS

Sitio estático que explica cómo se integran Vantage (el ERP del PAE y los comedores), SIESA y el WMS del CEDI de Yumbo.

| Página | Qué muestra |
|---|---|
| `index.html` | Informe: conexión con SIESA, flujo del menú a la factura, catálogos, interfaces SIESA ↔ WMS y qué cambia para Vantage |
| `circulacion-3d.html` | Mapa 3D interactivo: el mapa de conexiones, el interior de Vantage, el interior del WMS y la visión de futuro |

Las dos páginas se enlazan entre sí. No hay build ni dependencias: es HTML con el CSS y el JS adentro. Lo único externo son las fuentes de Google Fonts y three.js desde cdnjs.

## Verlo en local

```bash
python -m http.server 8000
```

Y abrir http://localhost:8000. También funciona abriendo `index.html` con doble clic.

## Publicar en GitHub Pages

Publicado en **https://erpplaneacion-eng.github.io/v_siesa_wms/** desde el repositorio `erpplaneacion-eng/v_siesa_wms`.

1. El repositorio debe ser público (en el plan gratis, Pages solo publica repositorios públicos).
2. En el repositorio: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, rama `master`, carpeta `/ (root)` → **Save**.
3. En uno o dos minutos queda publicado.

El archivo `.nojekyll` evita que GitHub procese el sitio con Jekyll.

## Actualizar

Editar los `.html` y volver a subir los cambios a `master`. GitHub Pages republica solo.

## Fuentes

- Estado de Vantage al 2 de octubre de 2026.
- Flujos del WMS según el acta de entrega de MUVUM del 28 de agosto de 2025 (no verifica qué está en producción hoy).
