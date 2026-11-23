# Pack de finanzas — 7 skills para Claude Code y Codex

> **Aviso.** Esto es educación financiera general, no asesoría financiera personalizada. Las skills no mueven dinero ni entran a tus cuentas: proponen, y tú decides y ejecutas. Las decisiones con consecuencias serias (impuestos, inversión, crédito) confírmalas con un profesional regulado de tu país.

Un sistema, no siete piezas sueltas: **el recorrido completo del dinero de una persona, en orden**. Cada skill hace una fase y le pasa el trabajo a la siguiente. Todas leen y escriben el mismo archivo de datos, `datos-financieros.md`, así que los datos se capturan una sola vez.

**El recorrido: Ver → Ordenar → Cortar → Atacar → Respirar → Crecer → Revisar**

| # | Skill | Qué hace | Necesita antes |
|---|-------|----------|----------------|
| 1 | `foto-financiera` | El diagnóstico: construye la foto completa (ingresos, cuentas, deudas con APR y fechas, dinero en custodia, suscripciones) y crea `datos-financieros.md`. Patrimonio neto fechado. | Nada. Es la entrada. |
| 2 | `presupuesto-real` | Presupuesto por ciclo de cobro real: cada cobro asignado a pagos con fecha, fondos para gastos irregulares y margen libre verdadero. | La foto (1) |
| 3 | `caza-suscripciones` | Audita suscripciones y recurrentes: duplicadas, zombies, pruebas que ya cobran. Cada una QUEDA / DUDA / CORTA, con ahorro anual y pasos de cancelación. | La foto (1) |
| 4 | `salir-de-deudas` | La estrategia de ataque: fechas límite que ahorran y avalancha por costo, calendario cobro a cobro y fecha de salida de cada deuda. | La foto (1) |
| 5 | `fondo-de-emergencia` | El colchón por niveles (1 semana → 1 mes → 3 meses de gastos), aporte automático por ciclo y reglas de uso y reposición. | Presupuesto (2) |
| 6 | `invertir-sin-humo` | Primera inversión con puerta dura: solo se activa con el fondo en Nivel 1 y sin deudas de APR alto. Cuenta de retiro, un fondo índice, aporte automático, reglas anti-humo. | Fondo Nivel 1 (5) |
| 7 | `revision-financiera` | El ritual mensual o trimestral: foto nueva contra la anterior, semáforo por área y las 3 movidas del próximo período. Cierra el círculo y vuelve a la 1. | Haber corrido el pack |

## Reglas que comparten las 7

- **Un solo archivo de datos** (`datos-financieros.md`) con secciones fijas: Ingresos · Cuentas y saldos · Deudas · Dinero en custodia · Suscripciones y recurrentes · Gastos fijos · Fondo de emergencia · Inversión · Historial de fotos.
- **Totales siempre separados**: deudas propias / dinero ajeno en custodia (dinero que guardas para otra persona: no es tuyo ni es deuda) / recurrentes. Nunca sumados juntos.
- **Verificar antes de afirmar**: lo no confirmado se marca NO VERIFICADO y no se usa para decidir.
- **Ninguna mueve dinero**: proponen con fechas y montos exactos; tú ejecutas cada pago, cancelación o aporte.
- **Salidas fechadas** y lenguaje claro, paso a paso.

## Instalación

1. Copia las 7 carpetas a `~/.claude/skills/` (Claude Code) o `~/.agents/skills/` (Codex).
2. Crea una carpeta de proyecto para tus finanzas y ábrela en Claude Code.
3. Corre primero `/foto-financiera` (o pide «hazme la foto financiera»): ella crea el archivo de datos y de ahí sigue el recorrido.

Hay un archivo de ejemplo con datos ficticios en `../../finance-pack/examples/` (en inglés) para que veas cómo queda.
