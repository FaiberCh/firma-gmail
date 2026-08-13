# Firma Gmail — Exámenes Médicos Especializados

Firma de correo personalizada para **JT(r) Jonny Barragán**, coordinador del servicio
de [Exámenes Médicos Especializados](https://www.examenesespecializados.com/)
(exámenes de ingreso y retiro a la Armada Nacional de Colombia).

Usa la identidad de marca del sitio del cliente (colores, tagline y logo) en lugar de
una foto personal.

## Contenido

```
firma-gmail/
├── index.html                          → la firma (HTML con estilos inline, lista para Gmail)
├── images/
│   ├── logo-completo-signature.png     → logo optimizado (320×320) usado en la firma
│   ├── logo-icono-signature.png        → variante circular optimizada (240×240), por si se prefiere
│   ├── logo-completo.png               → logo original (alta resolución, sin optimizar)
│   └── logo-icono.png                  → ícono original (alta resolución, sin optimizar)
└── README.md
```

## ⚠️ Importante antes de usarla: publicar el repo

`index.html` referencia el logo con esta URL:

```
https://raw.githubusercontent.com/FaiberCh/firma-gmail/main/images/logo-completo-signature.png
```

Esa URL **solo funciona después de subir este repo a GitHub** (público, rama `main`).
Mientras el repo sea solo local, el logo no se verá al abrir `index.html` ni al pegarlo en Gmail.

Pasos para publicarlo:

```bash
git remote add origin https://github.com/FaiberCh/firma-gmail.git
git branch -M main
git push -u origin main
```

El repositorio debe quedar **público** (o el logo no cargará, porque `raw.githubusercontent.com`
no sirve archivos de repos privados sin autenticación).

## Cómo instalar la firma en Gmail

1. Sube el repo a GitHub (paso anterior) y confirma que la imagen carga abriendo su URL
   directamente en el navegador.
2. Abre `index.html` en tu navegador (doble clic en el archivo).
3. Selecciona todo el bloque de la tarjeta de la firma (clic y arrastra desde la esquina
   superior izquierda hasta la esquina inferior derecha) y copia con `Ctrl+C`.
4. Ve a Gmail → ⚙️ **Configuración** → **Ver todos los ajustes** → pestaña **General** →
   sección **Firma**.
5. Crea o edita una firma, haz clic dentro del cuadro de edición y pega con `Ctrl+V`.
6. Guarda los cambios al final de la página.

## Datos incluidos en la firma

| Campo | Valor |
|---|---|
| Nombre | JT(r) Jonny Barragán |
| Cargo | Coordinador de Exámenes Médicos |
| Empresa | Exámenes Médicos Especializados |
| WhatsApp / Teléfono | +57 350 620 9179 |
| Email principal | examenespecializado@gmail.com |
| Email directo | jobaquira@gmail.com |
| Web | https://www.examenesespecializados.com/ |
| Tagline | "Tu proceso, en las mejores manos" |

## Identidad de marca usada

Colores y reglas tomados del `DESIGN.md` del proyecto del sitio web
(`examenes-medicos-especializados`):

- **Azul Armada** `#080D1A` — fondo de la tarjeta.
- **Azul Convocatoria** `#3A86FF` — cargo, enlaces y botón CTA.
- **Insignia Dorada** `#FFD700` — únicamente en la mención "Armada Nacional".
- Botón CTA con `border-radius: 9999px` (regla del sistema: todos los botones son circulares).

## Notas

- Los íconos de contacto (WhatsApp, teléfono, email, web) se cargan desde
  `img.icons8.com`, el mismo servicio usado en la firma de referencia — no requieren
  subirse a este repo.
- Si el logo se ve pixelado o muy grande/pequeño en Gmail, ajusta los atributos
  `width`/`height` del `<img>` en `index.html` (están en 130×130 px).
- Si más adelante el negocio define un dominio propio de email (por ejemplo
  `@examenesespecializados.com`), actualiza la fila de email principal en `index.html`.
