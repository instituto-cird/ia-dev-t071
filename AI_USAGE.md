# AI_USAGE.md · Registro de uso de IA

> Este archivo documenta el **origen** del trabajo: qué hizo la IA, qué hizo la persona y cómo se verificó. Se completa en cada laboratorio. En las revisiones y en la defensa final se puede preguntar por cualquier entrada. El formato es un criterio del programa.

## Cuándo registrar

**Se registra cuando hubo una decisión, no cuando hubo un autocompletado.**

Se registra si:
- El pedido se reescribió tres veces o más hasta obtener el resultado
- La salida no funcionó al primer intento y hubo que depurarla
- Se aceptó un diseño que la persona no había pensado antes
- Se **rechazó** una sugerencia (por seguridad, rendimiento o corrección)
- La IA **inventó** algo (librería, función, dato) y se detectó
- Un agente modificó varios archivos o ejecutó comandos
- Se usó IA para diagnosticar un error

No hace falta registrar el autocompletado de un `import`, de un nombre de variable o de un bloque que la persona iba a escribir de todos modos.

> **Regla práctica:** si dentro de tres meses no se va a recordar por qué el código quedó así, se registra.

## Niveles de autonomía

Se usan los cinco niveles de Feng, McDonald y Zhang (2025), definidos por el rol de la persona frente al agente: **1 operador** (la persona planifica y ejecuta; la IA sugiere a pedido) · **2 colaborador** (trabajo compartido; la persona puede tomar el control) · **3 consultor** (el agente planifica y ejecuta; la persona orienta en momentos clave) · **4 aprobador** (el agente trabaja solo; la persona destraba bloqueos y aprueba acciones importantes) · **5 observador** (la persona solo revisa el registro o detiene al agente).

Fuente: Feng, K. J. K., McDonald, D. W. y Zhang, A. X. (2025). *Levels of Autonomy for AI Agents*. arXiv:2506.12469. Preprint sin revisión por pares.

---

## Entradas

### Entrada 000 · Lab 0 · Onboarding

| Campo | Detalle |
|---|---|
| Fecha | 2026-11-13 |
| Herramienta | Claude Code (en Visual Studio Code) |
| Nivel de autonomía | 1 operador |
| Para qué se usó | Diagnosticar errores |
| Qué hizo la IA | Sugirió a pedido cómo diagnosticar errores |
| Qué hubo que corregir o rehacer | Nada |
| Cómo se verificó | CI |
| Qué decisión fue propia | Revisé las sugerencias y decidí qué cambios aplicar |
| Commit o PR | #1 |

<!-- Copiar el bloque de la entrada para cada nueva (001, 002…) -->

### Entrada 001 · Lab 1 · Comparación de modelos

| Campo | Detalle |
|---|---|
| Fecha | 2026-11-23 a 2026-11-26 |
| Herramienta | Claude |
| Nivel de autonomía | 2 colaborador |
| Para qué se usó | Entender la consigna, verificar el estado del repositorio, guiar los comandos y redactar el borrador de DECISION.md |
| Qué hizo la IA | Guió la instalación del kit y las corridas, leyó la consigna en Moodle, revisó VS Code y GitHub, propuso verificaciones y redactó el borrador |
| Qué hubo que corregir o rehacer | La extracción del kit se rehízo porque no quedó en el repo; se repitieron comandos que fallaron al pegarlos en la terminal |
| Cómo se verificó | CI local (ruff, mypy, bandit, pip-audit, 42 pruebas) y cifras contrastadas con resumen.md y los CSV |
| Qué decisión fue propia | Revisé y acepté la regla de ruteo, incluida la decisión de no adoptar la cascada; ejecuté los comandos en mi equipo |
| Commit o PR | PR del Lab 1, rama lab1/comparar-modelos |

---

## Resumen por laboratorio

Al cerrar cada laboratorio se completa una fila. Al final del programa, cada participante tiene sus propios números de **autonomía** y **retrabajo**, dos métricas que aparecen en descripciones de puestos de equipos que trabajan con agentes (revisadas por el programa en 2026, uso interno).

| Lab | Entradas | Nivel más usado | Parte hecha por el agente (aprox. %) | Parte que hubo que rehacer (aprox. %) |
|---|---|---|---|---|
| Lab 0 | | | | |
| Lab 1 | | | | |
| Lab 2 | | | | |
| Lab 3 | | | | |
| Lab 4 | | | | |
