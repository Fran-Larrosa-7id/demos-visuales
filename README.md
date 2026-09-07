# NAMI — Diseño + Web

Landing estática independiente, basada en los assets y el brief originales. El sitio está en la carpeta extraída: no necesita instalar paquetes ni compilar.

## Abrir y editar

Abrí `index.html` directamente en tu navegador o serví la carpeta extraída desde cualquier servidor estático. La fuente Sora/Inter se solicita a Google Fonts; si estás sin conexión se usa la alternativa local sans-serif.

- `index.html`: contenido, secciones, enlaces y composiciones de los tres conceptos.
- `styles.css`: identidad, responsive y variantes de movimiento reducido.
- `app.js`: scrollytelling, proceso, navegación, ventanas de conceptos, cursor y símbolo + con proyección 3D en canvas.
- `assets/`: SVG originales sin modificar, wordmark convertido a trazos compatibles y fotografías originales de Francisco y Santiago.

## Movimiento

El scroll es nativo: no hay captura de rueda ni scroll forzado. El hero se mantiene brevemente en desktop; el manifiesto desarrolla tres ideas y el proceso acompaña sus cuatro pasos. En móvil el proceso es vertical y el hero es estático. La preferencia del sistema `prefers-reduced-motion` convierte el manifiesto en contenido continuo y elimina los desplazamientos.

El canvas solo dibuja cuando cambian el scroll, el tamaño o la posición del cursor, y cuando el objeto está cerca de la pantalla. No usa Three.js, video ni un bucle permanente.

## Proyectos

Los tres elementos son **conceptos visuales**, no trabajos de clientes. Sus vistas se editan en `index.html` y los textos del diálogo en el array `projects` de `app.js`. Hay campos preparados para imagen, tecnologías, URL y año; cuando se incorporen casos reales, conectar esos campos con la vista y reemplazar los avisos de concepto. Actualmente no se presentan métricas, clientes ni enlaces de proyecto ficticios.

## Contacto

- Email: visual.nami@gmail.com
- Instagram: @nami.tandil
- Número informado: 2494 001904

El número se puede copiar. El enlace directo a WhatsApp queda pendiente de confirmar el número internacional completo: completar `CONTACT.whatsappE164` en `app.js`, con dígitos sin `+` ni espacios. No se asumió ningún prefijo. La copia automática requiere un contexto seguro y permisos de portapapeles; si no están disponibles, el sitio muestra el número para copiarlo manualmente.

## Equipo

Se conservan las fotografías originales de Francisco y Santiago. La foto de Santiago usa sus dimensiones reales y encuadre superior. El footer incorpora el wordmark original convertido de glifos SVG a trazos, enlaces de contacto, hora de Tandil y una animación de entrada que respeta movimiento reducido.

## Validación

Se verifica sintaxis JavaScript, estructura HTML, destinos internos y archivos locales. Esta entrega no incluye una prueba automatizada en navegador ni una auditoría formal de accesibilidad.
