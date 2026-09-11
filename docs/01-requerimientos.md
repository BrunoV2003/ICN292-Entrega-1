# 01 - Especificación de Requerimientos del Sistema

## 1. Actores y Roles
* **Encargada del Minimarket:** Usuaria principal. Opera la interfaz para registrar productos, ingresar compras, efectuar cobros/ventas y consultar reportes e inventario.
* **Proveedor (Actor Externo):** Abastece los productos y entrega la factura o guía de despacho física.
* **Lector de Código de Barras (Dispositivo Externo):** Dispositivo periférico HID/USB utilizado para capturar el identificador del producto en ventas e inventario.
* **Google Drive API (Servicio Externo):** Receptor de copias de seguridad de la base de datos cuando exista conectividad a Internet.

## 2. Alcance (In / Out)
* **Dentro del Alcance (In):**
  * Catálogo de productos con código de barras y generación de códigos internos.
  * Registro de entradas de inventario asociadas a costos unitarios históricos.
  * Módulo de ventas con rebaja automática de stock.
  * Notificación visual de productos bajo el punto de reposición.
  * Persistencia en base de datos local y módulo de respaldos programados.
* **Fuera del Alcance (Out):**
  * Facturación electrónica directa o sincronización automática con el SII.
  * Soporte multiusuario o sincronización concurrente en red (pensado para monousuario local).
  * Módulo contable integral (balances financieros completos, liquidación de sueldos o cálculo de impuestos).

## 3. Requisitos Funcionales (Priorizados vía MoSCoW)

### Must Have (Obligatorios)
* **RF01 - Catálogo de productos:** Registrar, editar y listar productos con nombre, código de barras y precio de venta actual.
* **RF02 - Generación de código interno:** Asignar identificadores numéricos únicos a productos que carecen de código de barras comercial.
* **RF03 - Ingreso de mercadería:** Registrar entradas de stock actualizando las unidades disponibles.
* **RF04 - Historial de costos:** Asociar cada lote de entrada al costo de compra unitario registrado en la factura.
* **RF05 - Módulo de ventas:** Registrar transacciones agregando múltiples ítems, calculando el total a pagar.
* **RF06 - Rebaja de inventario:** Descontar de forma transaccional e inmediata las unidades vendidas del stock.
* **RF07 - Inmutabilidad histórica:** Almacenar el detalle de venta con el precio y costo congelados al momento de la transacción.
* **RF08 - Alertas de reposición:** Identificar visualmente los artículos cuyo stock es menor o igual al stock mínimo de seguridad.

### Should Have (Importantes)
* **RF09 - Integración de lector de barras:** Procesar lecturas emitidas por el lector USB en venta e inventario sin requerir foco manual estricto.
* **RF10 - Indicadores operacionales (KPI):** Visualizar ventas diarias totales, unidades vendidas por ítem y lista de quiebres.
* **RF11 - Margen bruto operativo:** Desplegar margen comercial básico (Ingreso total - Costo de reposición).

### Could Have (Deseables)
* **RF12 - Respaldo en la nube:** Exportar copia de la base de datos hacia Google Drive vía API si hay conexión.
* **RF13 - Exportación de reportes:** Permitir exportar listados de reposición en formato CSV o plano.

## 4. Requisitos No Funcionales (RNF)
* **RNF01 - Autonomía y Funcionamiento Local:** La aplicación debe correr en `localhost` en el computador del local sin requerir Internet para su operación diaria.
* **RNF02 - Integridad y Persistencia:** Ningún corte eléctrico o cierre abrupto debe corromper la base de datos SQLite.
* **RNF03 - Tiempo de Respuesta:** La búsqueda por escaneo de código de barras y el registro de ventas deben responder en menos de 1 segundo.
* **RNF04 - Usabilidad:** Interfaz clara orientada a operarios con alfabetización digital básica, optimizada para teclado y lector.
* **RNF05 - Compatibilidad del Entorno:** Ejecución garantizada sobre sistema operativo Windows 10/11.