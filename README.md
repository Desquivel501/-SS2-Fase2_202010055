# [SS2]Fase2_202010055

## Solución de Business Intelligence - SG-Food

## Modelo

![modelo](/imagenes/modelo.png)

Para el modelo del datawarehouse se decidio utilizar un modelo constelacion, ya que son necesarias dos tablas de hechos: compras y ventas.

Estas tablas de hechos se conectan con las sigueines dimensiones:

- Fecha: Esta tabla contiene los datos relacionados al tiempo del hecho (año, semestre, mes, dia)
- Proveedor: Contiene los datos del proovedor al que se le compraron los productos.
- Cliente: Contiene los datos del cliente al cual se le hizo la venta.
- Producto: Contiene los datos del producto.
  - Marca: Marca del producto.
  - Categoria: Categoria a la que pertenece el producto.
- Vendedor: Informacion del vendedor que efectuo la venta.
- Sucursal: Sucursal donde se realizo la compra o venta.
  - Region: Region donde se encuentra ls sucursal
  - Depertamento: Departamento donde se encuentra el sucursal.

Asi mismo, el datawarehouse cuenta con 4 metricas

- Unidades (Compra): Cantidad de productos que se compraron
- CostoU: Costo unitario al que se compraron los productos
- Unidades (Ventas): Cantidad de productos que se vendieron
- PrecioUnitario: Precio unitario al que se vendio cada producto

### Cubo Compras

![modelo](/imagenes/cobo_compras.png)

### Cubo Ventas

![modelo](/imagenes/cobo_ventas.png)
