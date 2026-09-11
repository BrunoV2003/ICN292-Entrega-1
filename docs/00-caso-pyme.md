# 00 - Caso PYME y Diagnóstico del Problema

## 1. Identificación de la PYME
* **Razón Social / Titular:** Alma Ninela del Carmen Neira Muñoz
* **Nombre de Fantasía:** Minimarket Alma Neira Muñoz
* **Rubro:** Minimarket, comercio minorista de abarrotes, bebidas, lácteos, frutas y verduras
* **Tamaño Oficial:** Microempresa (Clasificación oficial SII, Primera Categoría, afecta a IVA)
* **Ubicación:** Pasaje Carlos Isamitt 785, Rengo, Región de O'Higgins
* **Operación:** Atendido de manera unipersonal por su dueña en jornada continua

## 2. Evidencia de Existencia
La existencia formal y tributaria de la empresa se acredita mediante:
* **Declaración Jurada de Inicio de Actividades (SII):** Folio N° 21007629601 (Trámite registrado el 30-09-2021).
* **Comprobante en Repositorio:** El documento probatorio completo se encuentra adjunto en los anexos del informe oficial en la carpeta `/informe`.

## 3. Formulación Medible del Problema de Gestión
El negocio opera con un **0% de trazabilidad digital e individual por producto**, registrando los flujos de dinero exclusivamente mediante montos globales en el terminal POS diario sin desglose de artículos vendidos ni costos asociados.

Esta ausencia de registro genera los siguientes impactos operacionales:
* **Control 100% visual y empírico:** Las decisiones de reposición dependen exclusivamente de mirar las repisas al momento en que pasa el proveedor.
* **Ciclos rígidos y quiebres de stock:** Se trabaja en ciclos de reposición de 15 días, permitiendo que los productos se agoten por completo antes de reordenar.
* **Pérdida por merma no cuantificada:** Productos vencidos o deteriorados (lácteos, cecinas, frutas) son desechados sin registro contable.
* **Ineficiencia horaria:** Se pierden entre **1 y 2 horas diarias** en la revisión manual de perchas, cálculo mental de compras y verificación física de facturas.

## 4. Objetivo del Sistema de Información (SIG)
Desarrollar e implementar una solución de software local para:
1. Registrar el catálogo de productos identificados mediante código de barras (o código autogenerado).
2. Registrar entradas de mercadería conservando costos unitarios de adquisición y fechas.
3. Automatizar el descuento de inventario en el punto de venta.
4. Emitir alertas tempranas basadas en el cálculo automático del punto de reposición.
5. Proveer persistencia local en SQLite con respaldos rotativos programados hacia Google Drive.