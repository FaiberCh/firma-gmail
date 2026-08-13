<div align="center">

# ✉️ Firma Gmail — Exámenes Médicos Especializados

**Firma de correo HTML** con la identidad de marca de
[examenesespecializados.com](https://www.examenesespecializados.com/) — logo, colores y
tagline del sitio, en vez de una foto personal.

`HTML5` · `Inline CSS` · `Sin dependencias` · `Lista para copiar/pegar en Gmail`

</div>

---

## 📁 Contenido

```
firma-gmail/
├── index.html   ← la firma (tabla HTML con estilos inline, lista para Gmail)
└── README.md    ← esta guía
```

Un solo archivo, cero dependencias, cero build. Ábrelo, cópialo, pégalo.

## 🖼️ El logo no vive en este repo

`index.html` referencia el logo directo desde el sitio del cliente:

```
https://www.examenesespecializados.com/images/logo-completo.png
```

**A favor:** no hay que mantener una copia del logo aquí ni depender de que este repo esté
público.
**A tener en cuenta:** si el sitio del cliente cambia esa ruta de imagen, el logo dejará de
cargar en la firma — hay que actualizar el `src` en `index.html` con la nueva URL.

## 🚀 Cómo instalar la firma en Gmail

1. Abre `index.html` en tu navegador (doble clic en el archivo).
2. Selecciona todo el bloque de la tarjeta (clic y arrastra desde la esquina superior
   izquierda hasta la inferior derecha) y copia con `Ctrl+C`.
3. Ve a Gmail → ⚙️ **Configuración** → **Ver todos los ajustes** → pestaña **General** →
   sección **Firma**.
4. Crea o edita una firma, haz clic dentro del cuadro de edición y pega con `Ctrl+V`.
5. En los menús **"Para los correos nuevos usar"** y **"En la respuesta/reenvío usar"**,
   selecciona esa firma.
6. Baja hasta el final de **toda la página** de configuración y haz clic en
   **"Guardar cambios"**.
7. Manda un correo de prueba a ti mismo y revísalo también desde el celular — pegar en
   Gmail copia el resultado ya renderizado, así que esa es la única forma real de
   confirmar cómo se ve.

## 🎨 Identidad de marca usada

Colores y reglas tomados del `DESIGN.md` del proyecto del sitio web
(`examenes-medicos-especializados`):

| Token | Color | Uso en la firma |
|---|---|---|
| Azul Armada | `#080D1A` | Fondo de la tarjeta (degradado) |
| Azul Convocatoria | `#3A86FF` | Cargo, enlaces, botón CTA |
| Insignia Dorada | `#FFD700` | Únicamente en la mención "Armada Nacional" |

El botón de WhatsApp usa `border-radius: 9999px` — regla del sistema de diseño del sitio:
todos los botones CTA son circulares, sin excepción.

## 📝 Notas

- Los íconos de contacto (WhatsApp, teléfono, email, web) se cargan desde
  `img.icons8.com` — no requieren subirse a este repo.
- Los enlaces de WhatsApp y web abren en pestaña nueva (`target="_blank"`); teléfono y
  email abren la app nativa del dispositivo (`tel:` / `mailto:`).
- Si el logo se ve pixelado o muy grande/pequeño en Gmail, ajusta los atributos
  `width`/`height` del `<img>` en `index.html` (están en 190×190 px).
- Los datos de contacto (nombre, cargo, teléfono, email) están únicamente dentro de
  `index.html` — no se repiten en este README.
