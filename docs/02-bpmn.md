# 02 - Modelado de Procesos de Negocio (BPMN 2.0)

## 1. Proceso As-Is (Operación Actual)
El proceso actual evidencia la ausencia de herramientas tecnológicas en el negocio
 Detección Inspección ocular directa de estantes. No existen parámetros cuantitativos para gatillar pedidos.
 Pedido Negociación presencial informal con el preventista de ruta cuando visita el local. Registro precario en un cuaderno de notas personales.
 Recepción Cotejo superficial de factura en papel contra bultos recibidos. Las mercaderías van directo a la estantería sin registrar ingresos en sistema.
 Venta Cobro en caja mediante terminal POS o efectivo. El inventario no se rebaja y no existe registro del producto comercializado.

![Diagrama As-Is](..assetsbpmn-as-is.png)

---

## 2. Proceso To-Be (Operación con SIG Propuesto)
El proceso propuesto integra la aplicación local en los puntos críticos de decisión
 Detección Automatizada El sistema compara el stock disponible en tiempo real con el punto de reposición configurado, emitiendo una lista de compras sugerida.
 Recepción y Carga El operario escanea los productos entrantes e ingresa costo y cantidad según la factura. El inventario se incrementa de forma trazable.
 Venta Ágil Escaneo de productos en caja, totalización y rebaja inmediata del stock en la base de datos local.
 Ajustes Registro formal de mermas por vencimiento o rotura.

![Diagrama To-Be](..assetsbpmn-to-be.png)

---

## 3. Tabla Comparativa de Mejoras
 Aspecto Operativo  Proceso Actual (As-Is)  Proceso Propuesto (To-Be) 
 ---  ---  --- 
 Detección de faltantes  Inspección visual en góndola.  Alerta automática por umbral de stock. 
 Criterio de pedido  Estimación intuitiva  empírica.  Cálculo por demanda histórica y plazo de entrega. 
 Entrada de mercadería  Sin registro de stock ni costo unitario.  Registro digital con costo, fecha y lote. 
 Registro de venta  Total global en POS (sin detalle de ítems).  Detalle unitario con rebaja automática de inventario. 
 Control de mermas  Desecho sin cuantificación.  Registro explícito como ajuste de inventario. 