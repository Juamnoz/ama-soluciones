# AMA Soluciones — Manual de marca

Fuente: `docs/manual-de-marca.pdf` (V3 Propuesta AMA Marca). Este archivo es el resumen accionable para trabajar sin tener que abrir el PDF cada vez.

## Qué es AMA Soluciones

Agencia multimarca de seguros y créditos (Medellín, Colombia). Compara entre varias aseguradoras en vez de vender una sola marca, y además tramita crédito de vehículo (nuevo/usado + compra de cartera).

- **Misión:** Proteger el bienestar y el patrimonio de los clientes a través de un portafolio integral de seguros (vida, salud, empresas, ARL) y créditos de vehículo. Mejores tiempos de respuesta, acompañamiento transparente.
- **Visión:** Consolidarse como la agencia de seguros y créditos más confiable y moderna del mercado, integrando IA en los procesos sin perder la esencia humana y familiar.
- **Promesa de marca:** Brindar la tranquilidad de que tu familia, tu empresa y tu futuro están respaldados por una marca que funciona con la solidez de una gran empresa, pero que cuida con la confianza y cercanía de una familia.
- **Valores:** Familiaridad (trata a cada cliente como en casa), Confianza (transparencia total), Cercanía (comunicación directa y humana).
- **Atributos:** Ágil e Innovadora (procesos optimizados con tecnología), Integral/Multimarca (todo en un solo lugar), Facilitadora (hace que lo complejo parezca sencillo).
- **Público objetivo:** Hombres y mujeres 25–50 años (foco principal 35+). Valoran estabilidad, quieren asegurar su salud y la de los suyos, proteger su empresa o apalancar la compra de un vehículo. Buscan un aliado que hable claro, sin dolores de cabeza, con respaldo real.
- **Origen del nombre:** "AMA" integra las iniciales de los hijos de los fundadores — **A**itana, **M**aximiliano y **A**ntonella — además de significar literalmente "ama" (amor). Ver [[landing-copy]] sección "Sobre nosotros" para el texto exacto que usa esta historia.

## Tagline oficial

**"Protegemos lo que amas."** — es el H1 elegido en el copy final de la landing (ver `docs/landing-copy.md`) y el que aparece en el lockup oficial del isotipo (`assets/logos/isotipo-tagline-color.png`).

El manual de marca lista 5 opciones de slogan que se barajaron (no usar estas como definitivas, están ahí solo como contexto de tono):
- Donde hay amor, hay alguien a quien cuidar
- Protegemos lo que más amas
- Cuidar lo que amas, es nuestra solución
- Lo que amas, en manos seguras
- La tranquilidad de ver seguros a quienes amas

Nota: en los mockups de redes del manual también aparece "Protegemos lo que hace grande tu vida." y "Donde hay amor, hay algo que cuidar." — son copys de piezas de ejemplo del manual, **no** el tagline final. Para la landing y cualquier pieza nueva, usar siempre **"Protegemos lo que amas."**

## Logo

El logo nace de la unión entre amor, familia y protección. Curvas suaves y continuas = cercanía, cuidado, confianza. El azul turquesa comunica tranquilidad, bienestar, seguridad y respaldo. El corazón representa el amor que protege; "ama" también son las iniciales de los hijos de los fundadores.

Archivos en `assets/logos/` (exportados del manual, fondo transparente):

| Archivo | Qué es | Uso |
|---|---|---|
| `logo-completo-color.png` | Wordmark "ama" + "SOLUCIONES" debajo, en azul turquesa | Logo principal, sobre fondos claros |
| `logo-completo-blanco.png` | Mismo logo completo, en blanco | Sobre fondos oscuros/de color sólido |
| `isotipo-corazon-color.png` | Solo el corazón (sin texto), en azul turquesa | Favicon, avatar de redes, marca de agua, espacios chicos |
| `isotipo-corazon-blanco.png` | Solo el corazón, en blanco | Sobre fondos oscuros/de color |
| `isotipo-tagline-color.png` | Corazón + "Protegemos lo que amas." | Piezas donde el tagline debe ir pegado al isotipo (portada de piezas, cierre de posts) |

**Zona de protección:** dejar un margen libre alrededor del logo equivalente aprox. a la altura de una de las "a" del wordmark (ver diagrama en el manual, pág. 9) — no pegar texto ni otros elementos dentro de esa zona.

**Usos incorrectos** (no hacer): rotar el logo, cambiar las proporciones (estirar/achatar), apilar el isotipo sobre el wordmark en vertical fuera del lockup oficial, ni separar las letras del wordmark del ícono de corazón de forma distinta a los assets ya exportados.

**Variaciones de color:** el logo puede usarse en los distintos tonos de azul de la paleta (abajo), y en blanco o negro sobre fondos sólidos de color cuando haga falta por legibilidad. **Nunca** sobre fondos con textura o que compitan visualmente con el logo.

El isotipo (solo corazón) puede usarse solo cuando el logo completo no sea necesario o el formato sea muy chico/cuadrado (ej. ícono de app, avatar IG).

## Paleta de color

| Hex | Uso |
|---|---|
| `#105c68` | Azul más oscuro — texto sobre fondos claros, variante oscura del logo |
| `#198799` | Azul principal de marca — el que más se repite en el manual (fondos de sección, CTAs) |
| `#46b4ce` | Azul medio — el del logo/wordmark principal |
| `#88bbd8` | Azul claro — variante suave del logo, detalles, fondos secundarios |

Todos dentro de la misma familia turquesa — no introducir otros colores de acento (ej. naranjas, verdes) salvo que el cliente lo pida explícitamente.

## Tipografía

**Avenir Next** (Regular + Bold) — único archivo en `assets/fonts/Avenir Next.ttc` (contiene ambos pesos, formato TrueType Collection). Es una fuente comercial (no Google Fonts) — para web hay que decidir entre:
- Comprarla/licenciarla para `@font-face` (ideal si el presupuesto lo permite), o
- Usar un sustituto de código abierto con métricas muy similares como **"Mulish"**, **"Nunito Sans"** o **"Figtree"** de Google Fonts (geométrica, redondeada, visualmente cercana a Avenir Next) hasta que el cliente confirme licencia.

Sin confirmación explícita del cliente sobre licenciamiento, por defecto usar un sustituto de Google Fonts y dejarlo anotado en el código (comentario) para swap fácil si llega la fuente real licenciada.

## Tono de voz (derivado del copy aprobado)

Cercano, cálido, directo — tutea al lector ("tu familia", "lo que amas"), evita jerga de seguros, usa frases cortas. Nunca suena a call center ni a letra pequeña agresiva (la letra pequeña existe pero es mínima y honesta, ej. "Crédito sujeto a estudio y aprobación de la entidad financiera"). Humor sutil y calidez (ej. "Porque ellos también son de la casa" para seguro de mascotas).
