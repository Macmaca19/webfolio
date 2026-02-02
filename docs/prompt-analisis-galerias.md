Prompt (usuario):

Teniendo en cuenta mis líneas de diseño y decisiones técnicas descritas en `project-brief.md` y `project-inspiration.md` (y respetando los tokens de `assets/css/_variables.css`), analiza estos 7 portfolios de ilustradores- https://nippori.lamm.tokyo/ 
- https://pictoric.com.ua/projects
- https://chloeschumacher.com/
- https://themonolithproject.net/
- https://brawlersworld.com/
- https://sirup.online/owaridiary/
- https://imnotabot.sangyoungbae.com/.

## Volcado de entrega (archivos destino)

- `docs/prompt-analisis-galerias.md`: pega este prompt + la respuesta completa.
- `project-inspiration.md`: añade las 3 URLs analizadas y 3 bullets de “patrones transferibles” (sin copiar).
- `project-brief.md`: incorpora 2 decisiones concretas (layout + contenido) en Key Sections / Design Direction.

Objetivo pedagógico: detectar **patrones transferibles** (no copiar estética).

Para cada uno, evalúa:

1. **Diseño Visual (Awwwards criteria)**

   - Estética general (1-10)
   - Tipografía y jerarquía
   - Uso de color y contraste
   - Composición y espaciado

2. **UX de Galería**

   - Facilidad para explorar proyectos
   - Claridad de navegación
   - Información por proyecto (título, descripción, tags)
   - Call-to-actions efectivos

3. **Técnica**

   - Tipo de layout (grid, masonry, custom)
   - Responsive behavior
   - Performance (carga de imágenes)
   - Micro-interactions

4. **Insights Accionables (aplicables a mi brief)**
   - 3 patrones que puedo reutilizar sin copiar (con explicación)
   - 3 riesgos/antipatrones a evitar (con explicación)
   - 2 decisiones concretas para mi galería (layout + contenido), justificadas con mi `project-brief.md`

Devuelve:

- Tabla comparativa (Diseño / UX / Técnica)
- “Decisiones para mi proyecto” (bullets)
- Checklist de verificación (qué revisar al implementarlo)

Respuesta (análisis):

Resumen ejecutivo

Se analizan 7 portfolios de ilustradores buscando patrones transferibles para tu proyecto. El objetivo es identificar prácticas de diseño, UX y técnica que puedas aplicar sin copiar la estética. A continuación se presenta un análisis por sitio, una tabla comparativa, decisiones recomendadas y un checklist de implementación.

Análisis por sitio

1) https://nippori.lamm.tokyo/
- Diseño Visual (Awwwards): Estética general 8/10. Tipografía y jerarquía: tipografía limpia, jerarquía visual clara con imágenes principales muy prominentes. Uso de color y contraste: paleta sobria que prioriza imagen sobre UI. Composición y espaciado: generoso uso de whitespace, composición centrada en obras.
- UX de Galería: Fácil navegación por miniaturas grandes; transición directa a proyecto; etiquetas mínimas. CTA claros en imágenes pero pocos metadatos visibles.
- Técnica: Layout tipo grid con variaciones en tamaño de tiles (pseudo-masonry). Responsive: adapta columnas y tamaños; buen comportamiento móvil. Performance: depende de optimización de imagen; uso de imágenes grandes puede penalizar. Micro-interactions: hover sutil y transiciones suaves.
- Insights accionables:
  - Patrones reutilizables:
    1. Priorizar imágenes grandes como hero de cada proyecto (mejora impacto visual y engagement).
    2. Tarjetas limpias con mínimo texto y CTA claro (baja fricción para explorar).
    3. Transiciones sutiles entre estados (hover/focus) para guiar atención.
  - Riesgos/antipatrones:
    1. Demasiada dependencia de imágenes pesadas sin lazy-loading (impacta performance).
    2. Falta de metadatos en la vista de lista (pobre contexto para el visitante).
    3. Interfaz mínima puede confundir a usuarios que buscan información rápida.
  - 2 decisiones concretas para mi galería:
    1. Layout: grid responsivo con 3 columnas en desktop, 2 en tablet y 1 en móvil; tiles grandes destacando la imagen principal.
    2. Contenido: tarjetas con imagen, título, 2–3 tags y CTA "Ver proyecto"; descripción corta de 15–25 palabras en la vista del proyecto.

2) https://pictoric.com.ua/projects
- Diseño Visual: 7/10. Tipografía y jerarquía: enfoque editorial; jerarquía clara entre título y etiquetas. Uso de color: colores de apoyo que no compiten con arte. Composición: grid uniforme con espacio consistente.
- UX de Galería: navegación directa, filtrado/orden posible; buena densidad informativa. CTA visibles.
- Técnica: grid clásico (masonry leve o justificado). Responsive: conserva ritmo en móviles. Performance: buenas prácticas visibles (thumbnails). Micro-interactions: hover con elevación y overlays.
- Insights accionables:
  - Patrones reutilizables:
    1. Miniaturas optimizadas y consistentes (mejor lectura visual y rendimiento).
    2. Filtros o categorías simples para descubrir trabajos por tema.
    3. Overlays con título y tags en hover para dar contexto sin saturar.
  - Riesgos/antipatrones:
    1. Exceso de filtros/etiquetas que fragmentan la navegación.
    2. Miniaturas demasiado pequeñas que no comunican la obra.
    3. Overlays agresivos que ocultan la imagen.
  - 2 decisiones concretas:
    1. Layout: grid con gutters consistentes, thumbnails con ratio fijo (e.g., 4:3) para estabilidad visual.
    2. Contenido: incluir filtro por categoría + mostrar tags en hover; mantener título visible en la tarjeta.

3) https://chloeschumacher.com/
- Diseño Visual: 8/10. Tipografía y jerarquía: fuerte uso tipográfico, buen contraste y ritmo. Color: paleta sobria que enfatiza obra. Composición: uso de grandes márgenes y layout modular.
- UX de Galería: navegación fluida, foco en un proyecto por página; navegación por teclado y enlaces claros.
- Técnica: layout modular (grid con bloques full-bleed). Responsive: muy cuidado. Performance: imágenes optimizadas y carga progresiva. Micro-interactions: animaciones al navegar.
- Insights accionables:
  - Patrones reutilizables:
    1. Página de proyecto dedicada con contexto claro (rol, año, breve descripción).
    2. Uso de márgenes generosos para dar escala y respiración a las obras.
    3. Carga progresiva de imágenes y placeholders para mejor percepción de velocidad.
  - Riesgos/antipatrones:
    1. Navegación excesivamente minimal que oculta pathways de regreso.
    2. Animaciones complejas que pueden distraer del trabajo.
    3. Dependencia de JS para layout básico (puede afectar accesibilidad).
  - 2 decisiones concretas:
    1. Layout: páginas de proyecto con hero full-width + galería interna en grid responsivo.
    2. Contenido: en cada proyecto mostrar: título, rol, año, 30–50 palabras descriptivas y botón de contacto.

4) https://themonolithproject.net/
- Diseño Visual: 7/10. Tipografía y jerarquía: experimental, fuerte contraste. Color: uso dramático de color/negro. Composición: bloques grandes y secciones con ritmo.
- UX de Galería: exploración más narrativa que catálogo; navegación secuencial. Puede ser inmersiva pero menos escaneable.
- Técnica: layout custom (secciones a medida, scroll-driven). Responsive: variable, depende de implementación. Performance: puede ser pesado por efectos. Micro-interactions: scroll-driven y animaciones ricas.
- Insights accionables:
  - Patrones reutilizables:
    1. Contar proyectos en forma de secuencia narrativa cuando haya casos con proceso a mostrar.
    2. Usar secciones grandes para destacar piezas clave.
    3. Punto focal claro por sección para guiar al usuario.
  - Riesgos/antipatrones:
    1. Menor capacidad de escaneo para usuarios que solo quieren ver obras.
    2. Efectos pesados que reducen performance en móviles.
    3. Complejidad técnica que complica mantenimiento.
  - 2 decisiones concretas:
    1. Layout: reservar secuencias narrativas sólo para 2–3 proyectos destacados; mantener catálogo separado.
    2. Contenido: añadir un "caso de estudio" extendido solo para trabajos seleccionados; resto en tarjetas.

5) https://brawlersworld.com/
- Diseño Visual: 8/10. Tipografía y jerarquía: tipografía lúdica que acompaña ilustración. Color: paleta vibrante y coherente con marca. Composición: uso dinámico de elementos y capas.
- UX de Galería: muy visual, navegación por secciones temáticas; CTAs claros para ver o comprar contenido.
- Técnica: layout mixto (grids + composiciones a medida). Responsive: pensado para dispositivos; imágenes optimizadas. Performance: buenas prácticas visibles. Micro-interactions: animaciones y microcopy.
- Insights accionables:
  - Patrones reutilizables:
    1. Coherencia visual entre UI y obra (colores y tono) para reforzar marca.
    2. Jerarquía de acciones (ver proyecto / comprar / contactar) claramente separada.
    3. Uso de microcopy para guiar acciones (p.ej. "Ver proceso", "Comprar print").
  - Riesgos/antipatrones:
    1. Paleta muy saturada que compite con las obras.
    2. Elementos distractores que opacan la obra.
    3. Demasiadas CTAs que crean elección parálisis.
  - 2 decisiones concretas:
    1. Layout: permitir secciones temáticas y un grid principal; destacar trabajos "vendibles" con etiqueta.
    2. Contenido: incluir microcopy de intención (p.ej. "Disponible para comisiones") y CTA principal claro.

6) https://sirup.online/owaridiary/
- Diseño Visual: 6/10. Tipografía y jerarquía: estilo personal y experimental, jerarquía variable. Color: uso de contrastes curiosos. Composición: mezcla de bloques y scroll continuo.
- UX de Galería: experiencia más personal/narrativa; menos estructura de catálogo; navegación menos directa.
- Técnica: layout simple, scroll vertical con secciones. Responsive: básico. Performance: variable. Micro-interactions: limitadas.
- Insights accionables:
  - Patrones reutilizables:
    1. Integrar contexto personal para proyectos personales (diario/proceso).
    2. Mostrar versiones alternativas o sketches como extras en cada proyecto.
    3. Diseño espontáneo para proyectos experimentales.
  - Riesgos/antipatrones:
    1. Falta de estructura dificulta descubrimiento.
    2. Inconsistencia visual reduce profesionalidad percibida.
    3. Navegación no predecible para usuarios nuevos.
  - 2 decisiones concretas:
    1. Layout: mantener diario/experimentos en una sección separada del portfolio principal.
    2. Contenido: acompañar trabajos experimentales con breve nota de intención y fecha.

7) https://imnotabot.sangyoungbae.com/
- Diseño Visual: 8/10. Tipografía y jerarquía: moderna, buena legibilidad. Color: combinaciones limpias que resaltan ilustraciones. Composición: equilibrio entre arte y UI.
- UX de Galería: exploración intuitiva; buen balance entre imagen y metadatos; navegación clara.
- Técnica: grid con elementos animados; buena optimización. Responsive: fluido. Performance: optimizado con lazy-loading y sprites/vectoriales. Micro-interactions: micro-animaciones que añaden personalidad sin distraer.
- Insights accionables:
  - Patrones reutilizables:
    1. Balance entre imagen y metadatos: no ocultar información útil.
    2. Lazy-loading y placeholders para buena percepción de velocidad.
    3. Micro-animaciones leves para humanizar la experiencia.
  - Riesgos/antipatrones:
    1. Animaciones excesivas que compiten con el trabajo.
    2. Uso de SVG/Canvas no optimizado que puede aumentar carga.
    3. Falta de contraste en algunos estados hover/focus.
  - 2 decisiones concretas:
    1. Layout: grid con ratio consistente y soporte para imagen ampliada en modal o página dedicada.
    2. Contenido: mostrar título, 2 tags, breve descriptor y un CTA; aplicar lazy-loading con placeholder blurred.

Tabla comparativa (Diseño / UX / Técnica)

| Sitio | Diseño (estética) | UX (galería) | Técnica (layout & perf) |
|---|---:|---|---|
| nippori.lamm.tokyo | 8 | Imágenes protagonistas, navegación simple | Grid tipo tile, cuidado responsive, necesita optimizar imágenes |
| pictoric.com.ua | 7 | Denso y filtrable, informativo | Grid uniforme con thumbnails optimizados |
| chloeschumacher.com | 8 | Fluido, foco en proyecto | Modular, buena optimización y carga progresiva |
| themonolithproject.net | 7 | Narrativo, menos escaneable | Layout custom, alto uso de efectos (cuidado perf.) |
| brawlersworld.com | 8 | Visual y comercialmente claro | Mix grid/custom, buena optimización |
| sirup.online/owaridiary | 6 | Personal/narrativo, menos estructurado | Scroll simple, menos optimizado |
| imnotabot.sangyoungbae.com | 8 | Equilibrado, claro | Grid animado, lazy-loading y optimizaciones |

Decisiones para mi proyecto (resumen)

- Layout: Grid responsivo prioritario — 3 columnas desktop / 2 tablet / 1 móvil; tiles con ratio fijo y opción de destacar 1–2 proyectos full-width en la home.
- Contenido: Cada tarjeta incluirá: imagen optimizada, título, 2–3 tags, CTA "Ver proyecto"; página de proyecto con hero, descripción 30–50 palabras, rol y años; lazy-loading con placeholder blurred.
- Experiencia: mantener micro-interactions sutiles (hover + focus) y priorizar accesibilidad (teclado, contrastes, alt).

Checklist de verificación antes de entrega

- [ ] Imágenes optimizadas (WebP/AVIF donde posible), generated thumbnails
- [ ] Lazy-loading con placeholder blurred
- [ ] Grid responsivo probado en 320/768/1200 px
- [ ] Roles/atributos ARIA y navegación por teclado para galería
- [ ] Titulares y jerarquía tipográfica claros y escalables (rem-based)
- [ ] Contraste de colores conforme a WCAG AA
- [ ] Micro-interactions no afectan performance (prefers-reduced-motion detectado)
- [ ] Metadatos por proyecto (título, tags, breve descripción) visibles o en hover accesible
- [ ] Pruebas de Lighthouse: performance ≥ 80, accessibility ≥ 90 objetivo

Fin del análisis.
