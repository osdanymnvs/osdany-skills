---
name: revision-financiera
description: Skill 7 del pack de finanzas personales: el ritual de cierre que se corre cada mes o cada trimestre (configurable). Repite la foto financiera y la compara contra el Historial de fotos, revisa el presupuesto ciclo a ciclo, mide las deudas contra la revisión anterior y contra lo que el plan de salir-de-deudas predecía para esta fecha, caza las suscripciones nuevas que se colaron, comprueba el nivel del fondo de emergencia y lista los vencimientos de los próximos 90 días. Entrega un informe fechado en revisiones/AAAA-MM-DD.md con tabla comparativa, semáforo por área con criterio escrito y LAS 3 MOVIDAS del próximo período, cada una asignada a la skill del pack que la ejecuta. Úsala cuando el usuario diga «hagamos la revisión del mes», «revisión financiera», «¿cómo voy contra el mes pasado?», «cierre del trimestre», «revisemos mis finanzas» o al cumplirse el período configurado desde la última revisión.
---

# revision-financiera — Skill 7 del pack de finanzas

> **Aviso.** Esto es educación financiera general, no asesoría financiera personalizada. Las decisiones con consecuencias serias (impuestos, inversión, crédito) se confirman con un profesional regulado de tu país.

Eres el paso 7 y el cierre del círculo de un pack de 7 skills: 1 foto-financiera → 2 presupuesto-real → 3 caza-suscripciones → 4 salir-de-deudas → 5 fondo-de-emergencia → 6 invertir-sin-humo → **7 revision-financiera**. Las otras skills construyen el sistema; tú compruebas si el sistema está funcionando. No rehaces los planes: los mides contra la realidad, marcas cada área con un semáforo de criterio escrito y dejas exactamente **3 movidas** para el próximo período, cada una con la skill del pack que la ejecuta. Al terminar, el círculo vuelve a empezar: tu foto de hoy es la línea base de la próxima revisión.

## Reglas del pack (obligatorias en esta skill)

1. **Un solo archivo de datos.** Todo se lee y se escribe en `datos-financieros.md`, en la carpeta del proyecto, con sus secciones fijas: Ingresos · Cuentas y saldos · Deudas · Dinero en custodia · Suscripciones y recurrentes · Gastos fijos · Fondo de emergencia · Inversión · Historial de fotos. La comparación se hace contra ese archivo, no contra recuerdos ni contra informes sueltos.
2. **Totales siempre separados.** Deudas propias, dinero ajeno en custodia y gastos recurrentes se presentan siempre por separado, nunca sumados en una sola cifra. El dinero en custodia no cuenta como patrimonio de la persona en ninguna tabla.
3. **Verificar antes de afirmar.** Lo que no puedas confirmar se marca **NO VERIFICADO**. Si un saldo o una cifra de la foto anterior no se puede contrastar con la fuente actual, la variación de esa línea se reporta como NO VERIFICADO, no como un número inventado. Requisitos o productos que se mencionen se verifican en fuentes oficiales el día de la corrida, con la fecha anotada.
4. **Salidas fechadas.** El informe se guarda como `revisiones/AAAA-MM-DD.md` y la foto nueva se registra en el Historial de fotos con su fecha.
5. **Lenguaje claro, paso a paso.** Cada semáforo y cada movida se explican en lenguaje llano: qué se midió, qué salió y qué se hace.
6. **La skill propone; la persona ejecuta.** No mueves dinero, no cancelas suscripciones, no pagas deudas ni ejecutas inversiones: asignas cada movida a la skill correspondiente y la persona la corre y la ejecuta.

## Configura esto primero

Antes de medir nada, localiza y lee en la carpeta del proyecto:

1. `datos-financieros.md` completo, con atención al **Historial de fotos** (necesitas la foto de la revisión anterior: fecha y patrimonio neto) y a las fechas límite especiales de la sección Deudas.
2. El plan vigente de **salir-de-deudas**, si existe en el proyecto: necesitas su predicción de saldo total de deudas **para esta fecha**, no solo su meta final.
3. El informe de la revisión anterior en `revisiones/`, si existe: sus 3 movidas son lo primero que se audita (Fase 0).
4. **Período de la revisión**: mensual o trimestral, según lo configurado en el proyecto; si no está configurado, pregúntalo una vez, déjalo escrito en el encabezado del informe y úsalo en adelante. La comparación cubre desde la fecha de la foto anterior hasta hoy; si el período real difiere del configurado (revisión atrasada o adelantada), se declara en el informe.

Si no hay foto anterior en el Historial, esta corrida es la **línea base**: se hace la foto completa (Fase 1), se registran las áreas medibles y el informe lo dice explícitamente — sin comparaciones inventadas contra un pasado que no está registrado.

## Fase 0 — Audita las 3 movidas de la revisión anterior

Antes de mirar números nuevos: abre el informe anterior y verifica, una por una, si sus 3 movidas se hicieron.

- Movida hecha: se marca **HECHA**, con la evidencia (la cifra o el cambio en `datos-financieros.md` que lo prueba).
- Movida no hecha: se marca **PENDIENTE** y pasa automáticamente a candidata prioritaria de esta revisión; una movida que sobrevive a dos revisiones sin hacerse se señala como **BLOQUEO** en el informe, con la pregunta directa: ¿falta de dinero, falta de tiempo o la movida estaba mal planteada? La respuesta decide si se reformula con su skill o se sustituye.

## Fase 1 — Foto nueva y patrimonio neto

1. Corre el procedimiento de **foto-financiera** (skill 1) completo: saldos, deudas, custodia, recurrentes, fondo e inversión, todo con fecha de hoy.
2. **Patrimonio neto** = (cuentas y saldos + fondo de emergencia + inversión) − deudas propias. El dinero en custodia **no suma**: se reporta en su propia línea, fuera del cálculo.
3. Compara contra la foto anterior del Historial: patrimonio neto anterior, patrimonio neto hoy, **variación en cifra y en porcentaje**, y la explicación de la variación en una o dos frases con causa identificable (ahorro del período, pago de deuda, gasto extraordinario, caída de mercado). Si la causa no se puede identificar con los datos, se dice: causa NO VERIFICADA.
4. Registra la foto de hoy en el **Historial de fotos** de `datos-financieros.md`: fecha + patrimonio neto (+ las líneas de deudas totales y fondo, para que la próxima comparación no dependa de reconstruir).

## Fase 2 — Presupuesto: ciclos cumplidos y dónde se fue el extra

Con el calendario de **presupuesto-real** (skill 2) y los movimientos del período:

1. Cuenta los ciclos de cobro del período: **ciclos cumplidos** (el gasto se mantuvo dentro de lo asignado) contra **ciclos desbordados** (se pasó), en formato «3 de 4 ciclos cumplidos».
2. Por cada ciclo desbordado: de cuánto fue el exceso y **en qué categoría se fue el extra**, con la categoría nombrada (no «gastos varios»: si no se puede atribuir, se marca NO VERIFICADO).
3. Detecta el patrón: ¿el desborde es siempre la misma categoría? Entonces no es un accidente, es un presupuesto mal calibrado, y la movida candidata es recalibrarlo con presupuesto-real, no «tener más cuidado».

## Fase 3 — Deudas: contra ayer y contra el plan

Dos comparaciones obligatorias, no una:

1. **Contra la revisión anterior**: saldo total de deudas propias antes y hoy; variación del período. Deuda por deuda, señala cualquier saldo que **subió** (deuda que crece mientras hay plan es una alarma, no un detalle).
2. **Contra el plan**: saldo que salir-de-deudas predecía para esta fecha contra saldo real de hoy. Diferencia a favor o en contra, en cifra. Si el real está peor que el plan, identifica la causa con los datos de la Fase 2 (¿se fue en el desborde del presupuesto?) o márcala NO VERIFICADO.
3. Revisa las **fechas límite especiales** de la sección Deudas (compras anticipadas, vencimientos de promociones, cierres): cuáles se cumplieron en el período y cuáles caen en los próximos 90 días (se cruzan con la Fase 6).

## Fase 4 — Suscripciones: las que se colaron

1. Compara la sección Suscripciones y recurrentes de hoy contra la de la última corrida de **caza-suscripciones** (skill 3) o contra la foto anterior si no la hay.
2. Lista las **altas nuevas**: cada suscripción o cargo recurrente que no estaba, con su costo mensual y su **costo anual calculado**. Una prueba gratuita que empezó a cobrar cuenta como alta nueva.
3. Lista también las que caza-suscripciones mandó cancelar y **siguen activas**: son una movida incumplida, no un olvido neutro.
4. Total del período: cuánto suman al año las que se colaron. Esa cifra, sola, suele ser una de las 3 movidas.

## Fase 5 — Fondo de emergencia: nivel contra meta

1. Saldo actual del fondo y su equivalente en meses de gastos esenciales (saldo ÷ gastos esenciales mensuales de la sección Gastos fijos).
2. Nivel alcanzado según la escalera de **fondo-de-emergencia** (skill 5) y distancia a la meta vigente, en cifra.
3. Movimientos del período: ¿creció al ritmo que presupuesto-real asignó?, ¿se usó? Si se usó, ¿fue una emergencia real según las reglas de la skill 5 y ya hay plan de reposición fechado?

## Fase 6 — Vencimientos de los próximos 90 días

Lista cerrada y fechada de todo lo que vence o exige acción en los próximos 90 días, salido de `datos-financieros.md`:

- Fechas límite especiales de deudas (compras anticipadas, fin de promociones sin interés).
- Renovaciones de suscripciones anuales y subidas de precio anunciadas.
- Vencimientos de documentos o pólizas registrados en el archivo.
- La fecha de la **próxima revisión** según el período configurado.

Cada entrada: qué es, fecha exacta, monto si aplica y qué pasa si se deja pasar. Esta lista no opina: informa. Las urgencias de esta lista tienen prioridad al elegir las 3 movidas.

## Fase 7 — Semáforo por área (con criterio escrito)

Cada área recibe un color según estos criterios. No se promedia un «más o menos»: si un criterio de rojo se cumple, el área es roja aunque lo demás vaya bien.

| Área | 🟢 Verde | 🟡 Amarillo | 🔴 Rojo |
|---|---|---|---|
| Patrimonio neto | Subió en el período | Igual (±1%) | Bajó |
| Presupuesto | Todos los ciclos cumplidos | 1 ciclo desbordado | 2+ ciclos desbordados, o el mismo desborde repetido |
| Deudas | Saldo ≤ plan para esta fecha y ninguna deuda subió | Saldo sobre el plan por menos de un ciclo de pago | Alguna deuda subió, o saldo sobre el plan por un ciclo de pago o más |
| Suscripciones | Sin altas nuevas | Altas nuevas que suman menos que una suscripción típica al año | Altas nuevas con costo anual alto, o cancelaciones ordenadas que siguen activas |
| Fondo de emergencia | En meta o creciendo al ritmo asignado | Crece, pero por debajo del ritmo | Bajó sin emergencia real, o se usó sin plan de reposición |
| Inversión (si aplica) | Aporte automático activo y puerta de invertir-sin-humo vigente | Aporte reducido un ciclo con causa declarada | Aporte detenido sin causa, o puerta dejó de cumplirse (fondo bajo Nivel 1 o deuda cara nueva) |

Si un área no se puede medir por datos NO VERIFICADOS, su semáforo es **⚪ Sin datos**, con lo que falta para medirla. Nunca se rellena con una impresión.

## Fase 8 — LAS 3 MOVIDAS del próximo período

Exactamente tres. Ni dos, ni cinco: tres, en orden de impacto. Reglas para elegirlas:

1. Primero, lo que la Fase 6 pone en riesgo en 90 días (una fecha límite que se pierde cuesta dinero seguro).
2. Después, el área en rojo de mayor impacto en dinero; luego los amarillos que llevan dos revisiones repitiéndose.
3. Las movidas PENDIENTES o en BLOQUEO de la Fase 0 compiten con prioridad, reformuladas si estaban mal planteadas.

**Cada movida se escribe con este formato fijo:**
- **Movida** (qué se hace, en una frase con verbo).
- **Cifra** (el monto o la meta numérica que la define).
- **Skill que la ejecuta**: el nombre exacto de la skill del pack que la lleva a cabo (presupuesto-real, caza-suscripciones, salir-de-deudas, fondo-de-emergencia, invertir-sin-humo o foto-financiera). Si ninguna skill la cubre, se dice y se propone como tarea manual fechada.
- **Fecha** en que debe estar hecha (antes de la próxima revisión).

## Salida: el informe fechado

Guarda el informe en `revisiones/AAAA-MM-DD.md` con esta estructura:

1. **Encabezado**: fecha, período configurado, período real cubierto (desde–hasta) y si es línea base.
2. **Tabla comparativa**: una fila por magnitud (patrimonio neto, deudas totales, fondo en meses, recurrentes al año, inversión) con tres columnas: revisión anterior, hoy, variación.
3. **Las 3 movidas anteriores**: HECHA / PENDIENTE / BLOQUEO, con evidencia.
4. **Semáforo por área**: tabla con color y la frase del criterio que lo decidió.
5. **Hallazgos por fase** (presupuesto, deudas contra plan, suscripciones coladas, fondo, vencimientos 90 días), cada uno con sus cifras.
6. **LAS 3 MOVIDAS** del próximo período, en el formato fijo de la Fase 8.
7. **Actualización hecha**: confirma que la foto de hoy quedó registrada en el Historial de fotos de `datos-financieros.md`.

## Cierre

Termina con un resumen en el chat de máximo 5 líneas: patrimonio neto y su variación, el área en peor semáforo, las 3 movidas nombradas en una línea cada una (o en una sola frase si son claras), y dónde quedó el informe. El círculo queda cerrado: la próxima revisión se corre al cumplirse el período configurado, y empieza auditando estas 3 movidas.
