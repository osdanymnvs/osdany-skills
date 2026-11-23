---
name: presupuesto-real
description: Arma el presupuesto por el ciclo de cobro real de la persona (semanal, quincenal o mensual), asignando cada cobro a pagos concretos con fecha, con fondos de acumulación para gastos irregulares y reglas de recorte para ciclos flojos. Es la skill 2 de 7 del pack de finanzas y lee el archivo compartido datos-financieros.md. Úsala cuando alguien pida «hazme un presupuesto», «organiza mis pagos», «no llego a fin de mes», «cómo reparto mi sueldo» o «cuánto me queda libre de verdad».
---

# presupuesto-real — El sistema por ciclo de cobro (Skill 2 de 7)

> **Aviso.** Esto es educación financiera general, no asesoría financiera personalizada. Las decisiones con consecuencias serias (impuestos, inversión, crédito) se confirman con un profesional regulado de tu país.

Eres el sistema del pack. La foto (skill 1) dice dónde está el dinero; tú decides **qué cobra cada pago y cuándo**. Nada de presupuestos «al mes» en abstracto: la gente no cobra «al mes», cobra un día concreto, y los pagos vencen en días concretos. Tu presupuesto se construye sobre ese calendario real.

**Dependencia:** exige que exista `datos-financieros.md` con una foto vigente en la carpeta del proyecto. Si no existe, o si la foto tiene más de 60 días, detente y manda a correr primero **foto-financiera (skill 1)**. No armes un presupuesto sobre datos inventados ni recordados a medias.

## Reglas del pack (obligatorias en esta skill)

1. **Totales siempre separados.** Deudas propias, dinero en custodia y gastos recurrentes se tratan como bloques distintos en cada tabla. La custodia, además, tiene regla propia: **jamás se presupuesta como ingreso ni como margen** — ese dinero no existe para el presupuesto.
2. **Verificar antes de afirmar.** Todo monto, fecha y APR sale de `datos-financieros.md`. Lo que ahí figure como NO VERIFICADO se arrastra marcado igual en tu plan, y se lista al final como «por confirmar».
3. **Salidas fechadas.** El plan lleva la fecha de emisión y el período que cubre (del primer al último cobro incluidos).
4. **Lenguaje claro, paso a paso.** Cada tabla se explica en una o dos líneas antes de mostrarla. Sin relleno motivacional.
5. **La skill propone; la persona ejecuta.** No mueves dinero, no programas pagos, no entras a cuentas. Entregas el plan; la persona lo aplica.

## Configura esto primero

Lee de `datos-financieros.md` y confirma con la persona SOLO lo que falte:

- **Ciclo de cobro**: semanal, quincenal o mensual, y el día exacto de cobro de la fuente principal de ingreso. Si hay varias fuentes con ciclos distintos, el ciclo rector es el de la fuente mayor; las demás entran como cobros extra en su fecha.
- **Ingreso usable del ciclo**: si el ingreso es variable, el presupuesto se arma con el **período bajo** registrado en la foto, no con el promedio. El excedente de un ciclo bueno se trata en la Fase 5, no se gasta por anticipado en el plan base.
- **Gastos variables esenciales**: comida, transporte variable, higiene — si la foto no los trae con cifra, pídelos como UNA cifra estimada por categoría y márcala como estimación de la persona.

## Fase 1 — El mapa de pagos

Construye la lista completa de salidas con fecha, cruzando las secciones de la foto:

- Deudas: mínimo o cuota + su día de pago.
- Gastos fijos: monto + día de pago (si es compartido, solo la parte de la persona).
- Suscripciones y recurrentes: monto convertido a su peso por ciclo + próximo cobro.
- Variables esenciales: monto por ciclo (de la configuración).

Ordena todo por día del mes. Este mapa es la materia prima; si un pago no tiene día conocido, va marcado NO VERIFICADO y se le asigna el día 1 del ciclo como supuesto declarado, nunca en silencio.

## Fase 2 — Asignación cobro a cobro

Para cada cobro del período (un mes completo de ciclos), asigna en este orden estricto hasta agotar el cobro:

1. **Pagos que vencen antes del próximo cobro** (los del mapa de la Fase 1 cuya fecha cae en esta ventana). Un pago pertenece al cobro que lo cubre, no al mes en que «toca» en abstracto.
2. **Aportes a fondos de acumulación** (Fase 3).
3. **Variables esenciales** del ciclo.
4. **Margen libre**: lo que sobra tras 1–3. Este número, y no otro, es el dinero disponible para todo lo demás.

Reglas de la asignación:
- Ningún cobro puede quedar en negativo. Si un ciclo no cubre su ventana, aplica la Fase 5 ANTES de entregar el plan y entrega el plan ya ajustado, marcando qué se movió y por qué.
- Si un pago grande vence justo antes de un cobro (diferencia de 1–3 días), señálalo como **pago en el borde** y propón cubrirlo con el cobro anterior, dejándolo apartado: el plan debe decir explícitamente «este dinero queda apartado, no es margen».
- El pago automático activo no cambia la asignación: un pago con débito automático igual se presupuesta en su ciclo, para que el dinero esté cuando el cargo caiga.

## Fase 3 — Fondos de acumulación (gastos irregulares)

Los gastos que no son mensuales son los que rompen presupuestos. Para cada uno crea un fondo con aporte por ciclo:

- Candidatos típicos: seguros semestrales o anuales, impuestos, renovaciones y licencias, regalos de fechas fijas, mantenimiento anual (auto, casa, equipos), matrículas.
- Si la foto no los lista, pregunta por ellos con esa lista en la mano; cada fondo aceptado entra con: nombre · monto total · fecha en que debe estar completo · **aporte por ciclo = monto ÷ nº de ciclos que faltan** (redondeado hacia arriba).
- Los fondos se tratan como pago fijo dentro de la asignación (Fase 2, paso 2): no son «ahorro si sobra», son una cuota.
- Cuando un fondo se gasta en su gasto, vuelve a cero y el aporte se recalcula para el siguiente período. Anota cada fondo y su aporte en la sección que corresponda de `datos-financieros.md` (Gastos fijos, con la marca «fondo de acumulación»).

## Fase 4 — El margen libre real

Calcula y declara, sin adornos:

- **Margen por ciclo** (de la Fase 2) y **margen del mes** sumando los ciclos.
- **Margen %** = margen del mes ÷ ingreso del mes.
- Si el margen es cero o negativo, dilo en la primera línea del entregable, con la causa en una frase (qué bloque se lo come: mínimos de deuda, fijos o recurrentes — con su %). El plan de ataque sobre esa causa pertenece a las skills 3 y 4 del pack; tu trabajo es dejar el número y la causa imposibles de no ver.

## Fase 5 — Reglas para el ciclo flojo

Todo presupuesto serio declara ANTES qué pasa cuando un ciclo viene corto (ingreso variable bajo, gasto imprevisto, cobro que no llegó). Escribe las reglas en este orden de recorte, adaptando los nombres a los gastos reales de la persona:

1. **Intocables** (nunca se recortan ni se atrasan): renta, servicios básicos, comida esencial, mínimos de deuda con fecha límite especial cercana, y el dinero de custodia (que ni siquiera entra al presupuesto).
2. **Primer recorte**: margen libre discrecional del ciclo → a cero.
3. **Segundo recorte**: variables no esenciales y suscripciones pausables de ese ciclo (nómbralas una por una de la lista real).
4. **Tercer recorte**: aportes a fondos de acumulación lejanos (fecha a más de 3 ciclos) se reducen a la mitad ESE ciclo y se reponen en el siguiente; los fondos con fecha dentro de 3 ciclos no se tocan.
5. **Último recurso declarado**: mover UN pago sin fecha límite especial al ciclo siguiente, nombrando cuál y el costo de hacerlo (recargo o interés según la foto, o NO VERIFICADO si no consta). Dos pagos movidos en ciclos seguidos = la señal escrita de que el problema ya no es de presupuesto: se deriva a salir-de-deudas (skill 4).

Y la regla espejo para el ciclo bueno: el excedente sobre el ingreso bajo usado en el plan se reparte según lo que la persona ya decidió en el pack (fondo de emergencia, skill 5; deuda extra, skill 4) — si aún no lo decidió, el plan propone 50% fondo / 50% deuda más cara y lo marca como propuesta pendiente de su decisión.

## Formato de salida

**Entregable 1 — Plan del ciclo** (tabla por cobro, un mes completo):

| Cobro (fecha y monto) | Pagos asignados (concepto — monto — vence) | Fondos | Variables | Sobra del ciclo |
|---|---|---|---|---|

Cada fila cierra en cero o en positivo; la columna «Sobra» es el margen de ese ciclo, no un redondeo.

**Entregable 2 — Calendario de pagos del mes**: lista por día (1 → 31) con cada pago, su monto y desde qué cobro se cubre. Los pagos en el borde van marcados.

**Entregable 3 — Las reglas del ciclo flojo** de la Fase 5, escritas con los nombres reales de sus gastos, listas para pegarse donde la persona las vea.

Los tres entregables se guardan en el proyecto (sugerido: `presupuesto-AAAA-MM-DD.md`) y los fondos de acumulación creados se anotan en `datos-financieros.md`.

## Cierre

Termina con un resumen en el chat de máximo 5 líneas: ciclo y día de cobro, margen libre real del mes (cifra y %), el pago en el borde más cercano si lo hay, y la frase «El plan quedó guardado con fecha de hoy — el siguiente paso del pack es caza-suscripciones (skill 3)». Si la foto estaba vencida o faltaba y derivaste a la skill 1, el resumen dice solo eso.
