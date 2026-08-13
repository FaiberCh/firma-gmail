# Firma Gmail — Exámenes Médicos Especializados

Firma de correo personalizada para **JT(r) Jonny Barragán**, coordinador del servicio
de [Exámenes Médicos Especializados](https://www.examenesespecializados.com/)
(exámenes de ingreso y retiro a la Armada Nacional de Colombia).

Usa la identidad de marca del sitio del cliente (colores, tagline y logo) en lugar de
una foto personal.

## Contenido

```
firma-gmail/
├── index.html   → la firma (HTML con estilos inline, lista para Gmail)
└── README.md
```

Este repo **no aloja el logo**: `index.html` lo referencia directo desde el propio sitio
del cliente:

```
https://www.examenesespecializados.com/images/logo-completo.png
```

Ventaja: no hay que mantener una copia del logo aquí ni depender de que este repo esté
público. Riesgo a tener en cuenta: si el cliente rediseña su sitio y cambia o elimina esa
ruta de imagen, el logo dejaría de cargar en la firma — en ese caso hay que actualizar el
`src` en `index.html` con la nueva URL.

## Cómo instalar la firma en Gmail

1. Abre `index.html` en tu navegador (doble clic en el archivo).
2. Selecciona todo el bloque de la tarjeta de la firma (clic y arrastra desde la esquina
   superior izquierda hasta la esquina inferior derecha) y copia con `Ctrl+C`.
3. Ve a Gmail → ⚙️ **Configuración** → **Ver todos los ajustes** → pestaña **General** →
   sección **Firma**.
4. Crea o edita una firma, haz clic dentro del cuadro de edición y pega con `Ctrl+V`.
5. Guarda los cambios al final de la página.

## Datos incluidos en la firma

| Campo | Valor |
|---|---|
| Nombre | JT(r) Jonny Barragán |
| Cargo | Coordinador de Exámenes Médicos |
| Empresa | Exámenes Médicos Especializados |
| WhatsApp / Teléfono | +57 350 620 9179 |
| Email | examenespecializado@gmail.com |
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
  `width`/`height` del `<img>` en `index.html` (están en 190×190 px).
- Si más adelante el negocio define un dominio propio de email (por ejemplo
  `@examenesespecializados.com`), actualiza la fila de email principal en `index.html`.
