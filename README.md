# ICN-292: Sistemas de Información para la Gestión — Entrega 1 (2026-2)

## Ficha del Equipo
* **Paralelo:** 101
* **Integrantes:**
  * Bruno Alejandro Vega Veloso (21.281.706-6) - 202360680-4
  * Nombre Completo 2 (RUT) - Rol
  * Nombre Completo 3 (RUT) - Rol
  * Nombre Completo 4 (RUT) - Rol
  * Nombre Completo 5 (RUT) - Rol
---

## 1. Contexto de la PYME y Problema de Negocio
* **PYME:** Minimarket [Nombre o referencia], Rengo, Región de O'Higgins.
* **Problema:** Gestión manual/visual del inventario y ausencia de trazabilidad financiera inmediata (quiebres de stock, costos de adquisición desactualizados y márgenes no calculados).
* **Objetivo del SIG:** Implementar un sistema local offline-first para registrar entradas, ventas con lector de barras, control de stock mínimo y márgenes brutos.

---

## 2. Estructura del Repositorio
* `/docs/`: Documentación detallada del caso, requerimientos, procesos BPMN y modelo relacional.
  * `00-caso-pyme.md`: Contexto del negocio y evidencia de levantamiento.
  * `01-requerimientos.md`: Requisitos funcionales (RF) y no funcionales (RNF).
  * `02-bpmn.md`: Explicación de procesos As-Is y To-Be.
  * `03-er-preliminar.md`: Diagrama y justificación del modelo Entidad-Relación.
* `/assets/`: Diagramas exportados en alta resolución (BPMN y E-R).
* `/informe/`: Informe formal en formatos PDF y editable (.docx / .tex).

---

## 3. Relación con la Entrega 2
La arquitectura diseñada en esta entrega servirá de especificación funcional para la implementación del software en entorno local (`localhost:3000`), operando de forma desacoplada de la nube para transacciones críticas.

---

## 4. Enlaces y Accesos
* **Informe oficial:** [Carpeta informe/](./informe/)
