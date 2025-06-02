# Maven-Toys
Análisis de ventas de Maven Toys, franquicia de jugueterías en México utilizando Power BI.

Se nos dan dados datos de ventas e inventario de una cadena ficticia de jugueterías en México llamada Maven Toys. Estos datos incluyen información sobre productos, tiendas, transacciones diarias de venta y niveles de inventario actuales en cada sucursal. Los datos abarcan del 1 de enero de 2017 al 30 de septiembre de 2018 y contienen más de 820,000 transacciones de todas las tiendas propiedad de Maven Toys.  
El objetivo es preparar los datos, analizarlos y visualizarlos, y posteriormente presentar los hallazgos que permitan a la cadena de jugueterías mejorar su capacidad de toma de decisiones e incrementar sus ganancias.  

# Recopilacion de Datos
Se nos proporcionan cuatro tablas en formato CSV que contienen los siguientes campos:

## Products (35 Productos Únicos)
Product_ID – ID único de cada producto ofrecido.  
Product_Name – Nombre único asignado a cada producto.  
Product_Category – Categoría asignada a cada producto según sus características o utilidad.  
Product_Cost – Costo para fabricar o adquirir el producto.  
Product_Price – Precio al que se vende el producto al cliente.  

## Stores (50 Diferentes Tiendas)
Store_ID – ID único de cada tienda.  
Store_Name – Nombre asignado a cada juguetería.  
Store_City – Ciudad de México donde está ubicada la tienda.  
Store_Location – Clasificación de la ubicación dentro de la ciudad (Centro, Comercial, Residencial, Aeropuerto).  
Store_Open_Date – Fecha en que la tienda fue inaugurada.  
Store_State – Estado de México donde está ubicada la tienda.  

## Sales
Sale_ID – ID único para cada transacción realizada en una tienda.   
Date – Fecha en la que ocurrió la transacción.  
Store_ID – ID único de la tienda donde se realizó la venta.  
Product_ID – ID único del producto vendido.  
Units – Número de unidades del producto vendidas.  
Revenue – Ingresos generados por la venta de productos, calculados como Units * Product_Price.  
Cost – Costo total de los productos vendidos, calculado como Units * Product_Cost.  
Profit – Ganancia obtenida por las ventas, calculada como Revenue - Cost.  

## Inventory:
Store_ID – ID único de la tienda.  
Product_ID – ID único del producto.  
Stock_On_Hand – Cantidad disponible del producto en inventario en la tienda.  

Además, se incorporaron una tabla de calendario para facilitar el análisis temporal por fechas y una tabla de estados de México para mejorar la visualización geográfica y reorganización del mapa interactivo según la ubicación de las tiendas.

## States
City - Ciudad de México donde está ubicada la tienda  
State - Estado de México donde está ubicada la tienda.  

## Calendar
Date – Fecha completa.  
Month – Nombre del mes (ej. Enero, Febrero, etc.).  
Month Order – Número del mes (1 para Enero, 2 para Febrero, etc.).  
Year – Año correspondiente a la fecha.  
Day Name – Nombre del día de la semana (ej. Lunes, Martes...).  
WeekDay – Número del día de la semana (1 = Lunes, 7 = Domingo, útil para ordenamiento).  
  
## Data Model
El modelo de datos está estructurado bajo un enfoque de esquema en estrella, donde las tablas de hechos (Ventas, Inventario) se conectan con diversas tablas dimensión como Productos, Tiendas, Calendario y Estados.
![Model](https://github.com/user-attachments/assets/55d87b6f-9514-432d-8efb-95c4b8055df4)

# Visualizacion de los Datos 





