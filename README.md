# ani-sic

Simulador visual e interactivo del **Ciclo de Instrucción (Direccionamiento Directo)** y el **Datapath** del procesador educacional **SIC 18-Bits** (AHPL RTL).

Desarrollado para la materia **ETN-821: Sistemas Digitales II** (Carrera de Ingeniería Electrónica - UMSA).

## Características

- **Diseño minimalista y oscuro:** Estética inspirada en 3Blue1Brown (3b1b).
- **Datapath fiel a la arquitectura:**
  - Registros: `PC[13]`, `MA[13]`, `MD[18]`, `IR[18]`, `AC[18]`, `IA[13]`, `IB[13]`, `Lf` (Link flag).
  - Memoria: `M (2¹³ × 18)` flanqueada físicamente por `MA` y `MD`.
  - Buses: `OBUS [19]`, `ABUS [18]`, `BBUS [18]`, `OBUS₀`.
  - Unidad Aritmético-Lógica (`ALU`).
- **Control por 3 sub-etapas:**
  1. Iluminación de cajas involucradas (origen en azul, destino en amarillo/verde).
  2. Ejecución física de la transferencia de datos en tiempo real (valores octales en los registros).
  3. Estado *Idle* de reposo/estabilización.
- **Rastreo didáctico de bifurcaciones AHPL:**
  - Muestra la fórmula RTL exacta del paso.
  - Siguiente paso al que bifurca la máquina de control y la condición lógica que lo activa.
  - Tracker de pasos interactivo.
- **Instrucciones soportadas:** `LAC`, `TAD`, `AND`, `DAC`, `ISZ (MD ≠ 0)`, `ISZ (MD = 0)`, `JMP`, `JMS`.

## Controles

- **Siguiente / Anterior:** Teclas `Flecha Derecha` y `Flecha Izquierda`.
- **Play / Pausa Automático:** Barra espaciadora (`Space`).
- **Selector de Instrucción:** Clic en los botones superiores.

---
Aux. Gabriel Sebastian Herrera Tola &bull; ETN-821
