# Sistema de Información para la Gestión (SIG) - Minimarket Alma Neira Muñoz

## 1. Identificación de la PYME y Problema Central
* **PYME:** Minimarket Alma Neira Muñoz (Microempresa, Persona Natural con Giro, SII Folio N° 21007629601).
* **Ubicación:** Pasaje Carlos Isamitt 785, Rengo, Región de O'Higgins.
* **Problema de Gestión:** El negocio opera con un 0% de trazabilidad digital e individual por producto; los registros de venta se limitan a montos globales en el terminal POS. El control de inventario es 100% manual y visual, provocando quiebres de stock recurrentes en ciclos rígidos de 15 días, pérdidas por merma no cuantificada y entre 1 a 2 horas diarias perdidas en revisión física de perchas.
* **Objetivo de la Solución:** Desarrollar un software de gestión local (localhost) para registrar productos (vía lector de código de barras), procesar ventas con descuento automático de inventario, calcular puntos de reposición y mantener respaldos locales sincronizables con la nube.

---

## 2. Integrantes y Roles (Grupo N° 5)
* **Bruno Vega Veloso** (Rol: 202360680-4) - Arquitectura y Gestión de Repositorio / Backend
* **Lorenzo Ruiz Flandez** (Rol: 202304619-1) - Modelado de Procesos BPMN y Requerimientos
* **Igor Ríos Rojas** (Rol: 202360586-7) - Modelado de Procesos BPMN y Diagramación Bizagi
* **Michelle Medina Barra** (Rol: 202360506-9) - Levantamiento de Caso PYME y Análisis de Riesgos / Ley 21.719
* **Charles Piket Silva** (Rol: 202360512-3) - Diseño de Base de Datos y Lógica de Indicadores (KPIs)

---

## 3. Estructura del Repositorio
* **`README.md`**: Resumen ejecutivo y guía rápida de comprensión del proyecto (≤ 10 minutos).
* **`docs/`**: Especificación detallada del proyecto en formato Markdown:
  * [`00-caso-pyme.md`](./docs/00-caso-pyme.md): Contexto del negocio, evidencias formales y transcripción de entrevista.
  * [`01-requerimientos.md`](./docs/01-requerimientos.md): Actores, alcance in/out, requisitos funcionales (RF) priorizados por MoSCoW y no funcionales (RNF).
  * [`02-bpmn.md`](./docs/02-bpmn.md): Explicación detallada de los procesos As-Is y To-Be con enlaces a los diagramas.
  * [`03-er-preliminar.md`](./docs/03-er-preliminar.md): Nota explicativa sobre el modelo de datos preliminar (eximido de evaluación por instrucción docente).
* **`assets/`**: Diagramas de procesos exportados en alta resolución (`bpmn-as-is.png`, `bpmn-to-be.png`) y el archivo fuente nativo de Bizagi (`modelo_procesos_minimarket.bpm`).
* **`informe/`**: Copia digital obligatoria del informe formal de la Entrega 1 en formato PDF y editable (.docx / .tex):
  * Acceso directo: [Carpeta de Informes](./informe/)

---

