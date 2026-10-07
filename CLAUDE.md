# CLAUDE.md

Guía de trabajo para este repo. Léeme antes de tocar nada.

## Qué es este proyecto

Landing page para **AMA Soluciones**, agencia multimarca de seguros y créditos de vehículo en Medellín, Colombia — cliente de **AIC Studio**. Es un proyecto de marca/landing nuevo (venía de una carpeta suelta en el Desktop del usuario con el manual de marca y el copy ya aprobado por el cliente; este repo lo organiza para trabajar).

El copy de la landing lo escribió la agencia externa **"El combo del tinto"** y ya está aprobado por el cliente — no es un borrador. El manual de marca lo hizo un diseñador aparte. Mi trabajo aquí es **implementar**, no redefinir marca ni reescribir copy salvo que el usuario lo pida explícitamente.

## Dónde está todo

```
.
├── CLAUDE.md                      ← este archivo
├── docs/
│   ├── brand-manual.md            ← resumen accionable del manual de marca (colores, logo, tipografía, tono)
│   ├── landing-copy.md            ← copy completo y final de la landing, sección por sección
│   ├── manual-de-marca.pdf        ← PDF original del manual de marca (15 páginas) — fuente de brand-manual.md
│   └── landing-copy-original.docx ← docx original del copy — fuente de landing-copy.md
└── assets/
    ├── logos/                     ← PNG exportados, fondo transparente, nombres descriptivos
    └── fonts/Avenir Next.ttc      ← fuente oficial de marca (Regular + Bold en un solo .ttc)
```

**Siempre leer `docs/brand-manual.md` y `docs/landing-copy.md` antes de generar cualquier pieza o código** — ahí está todo lo decidido (colores exactos, tagline oficial, textos aprobados, mensajes de WhatsApp por sección). No inventar copy nuevo ni paleta nueva.

## Lo que falta decidir (preguntar al usuario, no asumir)

- **Stack técnico:** todavía no se eligió framework. Mirando el resto de proyectos de AIC Studio, el patrón por defecto para landings de cliente es HTML/CSS/JS estático (como `scenius-web`) o Next.js simple desplegado en Vercel (como `grata-ropainfantil`, `zoomwithtara`, `paisa-soluciones`) — preguntar antes de hacer scaffold.
- **Dominio y hosting:** sin definir. Los demás proyectos de AIC Studio usan subdominio `*.aicstudio.tech` (vía Hostinger DNS) o dominio propio del cliente + Vercel. Confirmar con el usuario.
- **Fuente Avenir Next:** es comercial, no está en Google Fonts. Sin confirmación de licencia para web, usar un sustituto de Google Fonts visualmente cercano (Mulish, Nunito Sans o Figtree) — ver nota en `docs/brand-manual.md`.
- **Datos pendientes del cliente** (no inventar): correo de contacto, fotos del equipo (Diana Carolina y Andrés), logos en alta resolución de los aliados (Sura, Allianz, Seguros Bolívar, Axa Colpatria, SBS), IDs de Meta Pixel y Google Analytics. Lista completa al final de `docs/landing-copy.md`.

## Convenciones heredadas de AIC Studio (aplican aquí también)

- **Git:** nunca hacer `push` sin que el usuario lo pida explícitamente en ese momento — una aprobación anterior no cubre pushes futuros.
- **Deploy:** si el sitio termina en Vercel (patrón estándar de AIC Studio), el deploy es automático al hacer push a `main` vía integración de Git — nunca `vercel --prod` manual.
- **Sin pruebas en navegador** salvo que el usuario lo pida explícitamente — implementar y reportar.
- **Footer "Powered by LISA":** agregar un badge pequeño "Powered by" + isologo de LISA en blanco con link a `https://aicstudio.tech`, sutil (opacidad ~0.75, sube a 1 en hover), junto al copyright. Logo correcto: `/Users/Juamnoz/Desktop/proyectos/lisa/Isologotipo lisa nuevo blanco transparente.png` — **ojo**, existe un archivo homónimo con "incompleto" en el nombre que está roto, no usar ese. Recortar el bounding box real antes de insertarlo (el canvas trae mucho margen transparente).
- **WhatsApp:** cada CTA de la landing lleva su propio mensaje predefinido (no uno genérico para todos) — así el equipo de AMA identifica qué producto pidió cada lead. Los mensajes exactos están en `docs/landing-copy.md`.
- **Analítica:** el cliente pidió explícitamente Meta Pixel + Google Analytics — no son "nice to have", van en el alcance base.
- **Mobile-first:** pedido explícito del cliente en las notas de implementación del copy.

## Flujo de trabajo

1. Antes de escribir código: confirmar stack con el usuario si no se ha hecho.
2. Usar el copy de `docs/landing-copy.md` tal cual — si algo no calza con el diseño, preguntar antes de parafrasear.
3. Usar los colores/logos/tipografía de `docs/brand-manual.md` tal cual — no improvisar paleta.
4. Commit solo cuando el usuario lo pida (salvo que diga lo contrario explícitamente para este proyecto).
