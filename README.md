# Lector QR · CEMPERU

Página de lectura de códigos QR y de barras con la **cámara en vivo**. Se publica fuera de Google (en GitHub Pages, gratis) porque, dentro de Apps Script, el navegador no deja abrir la cámara en vivo.

- **La usa el Sistema de Inventario** (picking, inventario general, preparación de racks y cualquier pantalla con escáner): la pantalla abre el lector, el lector lee y le devuelve el código.
- **Sirve para otros proyectos:** cualquier aplicación puede abrirla con `?id=...` y recibir el código. Abierta sola, muestra lo leído y permite copiarlo.
- **No guarda ni envía datos** a ningún servidor: todo pasa en el teléfono.

## Publicarla (una sola vez, unos 10 minutos)

1. Crear una cuenta gratuita en https://github.com **a nombre de la empresa** (por ejemplo, `cemperu`), no a nombre personal.
2. Arriba a la derecha: **+ → New repository**. Nombre: `lector-qr`. Marcar **Public**. **Create repository**.
3. En el repositorio nuevo: **Add file → Upload files**. Subir `index.html` y este `README.md`. **Commit changes**.
4. **Settings → Pages**. En *Branch* elegir `main` y la carpeta `/ (root)`. **Save**.
5. Esperar uno o dos minutos. GitHub muestra la dirección, por ejemplo `https://cemperu.github.io/lector-qr/`.
6. Abrir esa dirección en un celular: debe pedir permiso de cámara y leer un QR de prueba.

## Conectarla al sistema

En la planilla, menú → **🎥 Configurar lector QR externo (cámara en vivo)** (o en la web: Configuración → **Lector QR externo**). Pegar la dirección del paso 5 y guardar.

Desde ese momento, todas las pantallas con escáner muestran **🎥 Cámara en vivo**. La foto con la cámara nativa queda como respaldo. Para desactivarlo, guardar la dirección vacía.

## Primera vez en cada celular

- El navegador pregunta si se permite la **cámara** a la página del lector: responder **Permitir** (lo recuerda).
- Si el teléfono bloquea la ventana del lector, permitir las **ventanas emergentes** para la app, o usar la foto mientras tanto.

## Cambiar algo después

Editar `index.html` en el repositorio (ícono del lápiz) y guardar. GitHub vuelve a publicarlo solo en uno o dos minutos; no hace falta tocar el sistema.
