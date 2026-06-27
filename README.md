# avafac.com.ar — Landing de avaFAC

Sitio estático (una sola página) de presentación del producto **avaFAC**
(facturación electrónica y punto de venta), servido por **GitHub Pages** con
dominio propio.

## Estructura

| Archivo | Propósito |
|---|---|
| `index.html` | Landing page completa (HTML + CSS inline, autocontenida) |
| `CNAME` | Dominio personalizado de GitHub Pages: `avafac.com.ar` |
| `404.html` | Redirige cualquier ruta desconocida a la home |
| `robots.txt` / `sitemap.xml` | SEO |

## Publicación

GitHub Pages publica la rama `main` (carpeta raíz). Cada push a `main`
actualiza el sitio en pocos minutos.

## DNS (configurar en NIC.ar)

Para que `avafac.com.ar` apunte a GitHub Pages, cargar en el DNS del dominio:

**Apex (`avafac.com.ar`) — registros A:**

```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**Apex — registros AAAA (IPv6, opcional):**

```
2606:50c0:8000::153
2606:50c0:8001::153
2606:50c0:8002::153
2606:50c0:8003::153
```

**Subdominio `www` — registro CNAME:**

```
www  ->  pabloandresparisi.github.io
```

Una vez que el DNS propague, activar **"Enforce HTTPS"** en
Settings → Pages del repositorio.
