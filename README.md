# Análisis Interactivo de Ventas y Beneficios 📊

## 📖 Descripción del Proyecto
Este proyecto realiza un análisis exploratorio de la actividad de un supermercado. 
El análisis se centra tanto en las ventas como en los beneficios ya que al ser un supermercado, los márgenes son muy bajos y por lo tanto la diferencia entre los números de las ventas y los de los beneficios es muy grande. 
El objetivo también es proporcionar un dashboard para que el análisis de estos datos sea interactivo y se pueda actualizar automaticamente a medida que se carguen datos de ventas cada mes.

En cuanto al dataset, este tiene 20 columnas:
- Invoice ID: Esta es una columna con un valor único, que identifica cada pedido que se ha hecho.
- Branch: Esta columna contiene una letra que identifica al supermercado de cada ciudad ("A", "B" o "C").
- City: SI en la columna anterior había una "A" la ciudad es "Yangon", en cado de una "B" es "Mandalay" y en caso de una "C" es "Naypyitaw".
- Customer Type: Indica el tipo de cliente, hay dos tipos, "Normal" o "Member".
- Gender: Indica el género del cliente, hay dos géneros, "Male" o "Female".
- Product Line: Indica la categoría del producto que se ha comprado. En total hay 6 product lines ("Health and beauty", "Electronic accessories", "Home and lifestyle", "Sports and travel", "Food and beverages" y "Fashion accessories".
- Unit Price: Un número que indica el precio del producto que se ha comprado.
- Quantity Purchased: Un número que indica la cantidad de producto que se ha comprado.
- Tax 5%: Un número que indica la cantidad de impuesto a pagar por esa compra.
- Total Sale: Un número que indica el importe final de la compra.
- Date: Es una fecha que indica cuando se hizo la compra.
- Month: Indica el mes que se hizo la compra, en este dataset solo hay los tres primeros meses del año ("January", "February" y "March")
- Time: Un número que indica la hora del día que se hizo la compra incluyendo la hore, el minuto y los segundos (ejemplo: "10:11:00")
- Payment: Indica el método de pago que se usó para finalizar la compra, en este dataset hay tres opciones ("Ewallet", "Cash", "Credit card")
- COGS: Un número que indica los "Cost Of Goods Sold", que en Español sería el costo de los bienes vendidos.
- Gross Margin %: Es un porcentaje que indica el márgen que hay entre los costes del producto y el precio de venta, como más alto más beneficios para el vendedor.
- Gross Income: Es un número que indica el márgen pero en términos de importe y no de porcentaje.
- Rating: Es un número del 0 al 10 que pone el cliente en cada compra valorando la compra, como más alto más contento ha acabado el cliente (ejemplo: 9,1).
- Good Rating: Una tabla que he creado yo con la formula (=IF([@Rating]>8;1;), donde me contabiliza los ratings superiores a 8.
- BadRating: Igual que la anterior pero en esta contabiliza los ratings inferiores a 5 (=IF([@Rating]<5;1;)

## 📋 Estructura del Proyecto

- Data: [Descargar csv](https://kaggle.com/datasets/aungpyaeap/supermarket-sales?resource=download)
- Excel: (Un archivo excel donde se realiza el proyecto)
- README.md:  (Descripción del proyecto)

## 🛠 Instalación y Requisitos


Este proyecto usa:

- Un archivo csv con los datos de las ventas de 3 supermercados de una misma compañía.
- Un archivo excel para cargar los datos, analizarlos y crear un dashboard interactivo.

## 📊 Resultados y Conclusiones

- El margen de beneficios es del **4,76%**, lo cual es **muy alto** teniendo en cuenta que el margen de beneficios promedio de los supermercados en España es aproximadamente de entre el 2% y el 3% según distintas fuentes, entre ellas la más relevante La Razón (https://www.larazon.es/economia/supermercados-recortan-margen-beneficio-uno-niveles-mas-bajos-ultimos-diez-anos_2024090966daddbe9dc60f0001e589de.html).
- La categoría que tiene **peor rendimiento** es **Health and Beauty** lo cual es extraño teniendo en cuenta que el segmento principal de la categoría son las mujeres, las cuales son el grupo de clientes que gasta más dinero. Por lo tanto habría que centrarse en crear promociones atractivas para atraer al segmento.
- De media, los **martes y los jueves** son los días en los que se venden más productos por lo tanto se tendría que considerar poner descuentos los otros días para atraer más clientes y poner ofertas, como por ejeplo 3x2, los martes y los jueves que va más gente para que compren más productos.
- El average rating es solo del **6,97**, por lo tanto **indica una oportunidad para mejorar la satisfacción al cliente**. Un ejemplo sería ofrecer un training de "excelente atención al cliente" a los empleados que trabajan de cara al público. Otro sería hacer una encuesta a algunos clientes que dan ratings bajos para intentar entender la razón.
- El tipo de cliente que **genera más facturación** son las **mujeres que son miembros**, por lo tanto también sería una oportunidad dar ofertas personalizadas a este segmento.
- El tipo de cliente que **genera menos facturación** son los **hombres que son miembros**, por lo tanto también se tendrían que buscar oportunidades para atraer más a este segmento como lanzando mejores productos en la categoría de "Sports and travel".

## 🔄 Próximos Pasos

- Mejorar el análisis de los datos proporcionando más datos históricos ya que de momento solo hay los datos de los 3 primeros meses del año.
- Mejorar como afectan las macro a la visualización de los datos.

## 🤝 Contribuciones

Las contribuciones son bienvenidas :)

##  ✒ Autores

- Marcos Herrera
