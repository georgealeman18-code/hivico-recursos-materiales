# Configuración de ManyChat — “Comenta PLANTILLA” · @gestion_360mx

> La configuración la haces tú desde tu cuenta: Claude no puede iniciar sesión en ManyChat ni en Instagram. Los nombres de menús pueden variar ligeramente según la versión de ManyChat.

## 0. Requisitos previos (10 min)
| # | Requisito | Cómo verificar |
|---|---|---|
| 1 | Cuenta de Instagram **profesional** (Creador o Empresa) | Ya la tienes (aparece “Tu panel”) |
| 2 | Permitir acceso a mensajes | Instagram → Configuración → Mensajes y respuestas a historias → Controles de mensajes → **Herramientas conectadas: Permitir acceso a los mensajes** = activado |
| 3 | Recurso gratuito listo | `KIT_DIRECCION_360.md` convertido a PDF y subido a Drive con enlace público de solo lectura |
| 4 | Enlace corto (opcional) | Acortador o página de enlaces para medir clics |
| 5 | Una segunda cuenta de Instagram para pruebas | Cuenta personal o de alguien de confianza |

## 1. Crear la cuenta y conectar Instagram (5 min)
1. Entrar a manychat.com → **Get Started / Comenzar gratis**.
2. Elegir canal **Instagram** → iniciar sesión con la cuenta @gestion_360mx (inicio de sesión oficial; **no** compartir contraseña con nadie más).
3. Aceptar permisos de mensajes y comentarios.
4. Configurar zona horaria: **America/Mexico_City** e idioma español.

## 2. Evitar respuestas duplicadas
Si en Meta Business Suite activaste **respuesta instantánea**, desactívala o deja que solo ManyChat responda el primer mensaje. Si no, la persona recibe dos mensajes y se ve poco profesional.

## 3. Automatización principal: “Comenta PLANTILLA”
**Automatizaciones → Nueva automatización → Empezar desde cero** (o plantilla “Auto-DM links from comments”).

### Paso 3.1 · Disparador
- Tipo: **El usuario comenta en tu publicación o reel**.
- Publicación: **reel específico** (el del lunes 16/11) o **cualquier publicación** si usarás la misma palabra en varios reels de la semana (recomendado para semana 1).
- Palabras clave: `PLANTILLA`, `plantilla`, `Plantilla` (activar “contiene” para que funcione aunque escriban “plantilla por favor”).

### Paso 3.2 · Respuesta pública al comentario (rotar 3 variantes)
1. `¡Listo! Te la envié por mensaje directo 📩`
2. `Revisa tus mensajes, ya va en camino 🙌`
3. `¡Enviada! Si no la ves, revisa la carpeta de Solicitudes 📥`

### Paso 3.3 · Primer mensaje privado (con botón)
> ¡Hola! 👋 Gracias por comentar. Aquí tienes el **Kit de Dirección 360**: diagnóstico de 10 señales, matriz de delegación y plantilla RACI.
> Toca el botón para recibir el enlace 👇
> **[Botón: Quiero el kit]**

*Por qué con botón:* la persona responde, se abre la conversación y el enlace llega con mejor entregabilidad.

### Paso 3.4 · Mensaje con el enlace (al tocar el botón)
> Aquí está 👉 [ENLACE AL PDF]
> Empieza por la página 2: si marcas 4 o más señales, tu empresa depende demasiado de ti.

*(Opcional) Verificación de seguidor:* condición “¿Sigue la cuenta?” → si no, mensaje “Sígueme para recibir más herramientas como esta 🙌” + botón “Ya te sigo” → volver a verificar. Activarlo puede aumentar seguidores, pero algunas personas abandonan; probar una semana con y una sin.

### Paso 3.5 · Pregunta de calificación (5 min después)
> Una pregunta rápida para enviarte contenido útil: ¿diriges un equipo actualmente?
> **[Sí, dirijo un equipo]** **[Todavía no]**

- Sí → etiqueta `Dirige equipo` → ir a 3.6.
- Todavía no → etiqueta `Audiencia` → mensaje: “¡Perfecto! Te va a servir para cuando llegue el momento. Activa las notificaciones para no perderte los reels 🔔”. Fin.

### Paso 3.6 · Captura de contacto (solo `Dirige equipo`)
> ¿De cuántas personas es tu equipo?
> **[1–5]** **[6–20]** **[21–50]** **[Más de 50]** → guardar en campo personalizado `tamaño_equipo`.

> Si quieres, déjame tu correo y te envío una herramienta de dirección cada semana (sin spam).
> → Entrada de usuario tipo **Correo electrónico** → guardar en `correo`. Permitir “Omitir”.

> Gracias 🙌 Si marcaste 4 o más señales en el diagnóstico, escríbeme **DIAGNÓSTICO** y te digo por dónde empezar.

## 4. Automatización secundaria: palabra “DIAGNÓSTICO” por DM
- Disparador: **El usuario envía un mensaje directo** con palabra clave `DIAGNÓSTICO` / `diagnostico`.
- Acción: etiqueta `Prospecto asesoría` + mensaje:
> ¡Gracias por escribir! Para orientarte bien, cuéntame en 2–3 líneas: ¿a qué se dedica tu empresa, cuántas personas son y cuál es el reto que más te quita el sueño? Te respondo personalmente en menos de 24 h.
- Notificación: activar **aviso al administrador** (app de ManyChat) para responder tú mismo.

## 5. Etiquetas y campos a crear
| Tipo | Nombre | Uso |
|---|---|---|
| Etiqueta | `Kit enviado` | Quién recibió el recurso |
| Etiqueta | `Dirige equipo` / `Audiencia` | Segmentación |
| Etiqueta | `Prospecto asesoría` | Pidió diagnóstico → seguimiento personal |
| Campo | `tamaño_equipo` | Calificación |
| Campo | `correo` | Lista propia |

## 6. Prueba antes de publicar (obligatoria)
| # | Prueba | Resultado esperado |
|---|---|---|
| 1 | Desde la cuenta de prueba, comentar “plantilla” en un reel | Respuesta pública + DM en < 1 min |
| 2 | Tocar el botón | Llega el enlace y abre el PDF sin pedir permiso |
| 3 | Responder “Sí” y dar correo | Se guardan etiqueta y campos |
| 4 | Escribir DIAGNÓSTICO por DM | Llega mensaje + notificación al administrador |
| 5 | Revisar carpeta Solicitudes de la cuenta de prueba | Confirmar dónde llega si no sigue a la cuenta |

## 7. Límites y buenas prácticas
- Meta solo permite una respuesta privada por comentario y dentro de un periodo limitado tras el comentario; responde rápido y no reenvíes enlaces que no pidieron.
- Fuera de la ventana de 24 h desde el último mensaje de la persona, no se pueden enviar mensajes promocionales automáticos.
- Revisar semanalmente en ManyChat: **comentarios → DM enviados → clics en el enlace → correos captados → prospectos**.
- El plan gratuito tiene límite de contactos; cuando se acerque, evaluar el plan de pago (verificar precio vigente).

## 8. Indicadores del embudo (semana 1)
| Etapa | Meta semana 1 |
|---|---|
| Comentarios con PLANTILLA | 150 |
| DM entregados | 150 |
| Clics en el botón | ≥ 70% |
| `Dirige equipo` | ≥ 40% |
| Correos captados | 30 |
| Mensajes DIAGNÓSTICO | 5 |
