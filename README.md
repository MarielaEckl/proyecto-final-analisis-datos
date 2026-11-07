# 📊 Proyecto Final | Data Analytics

## ¿Dónde está el valor de nuestro negocio?
### Una investigación a través de los datos de Online Retail

Este proyecto busca transformar datos de transacciones comerciales en información útil para comprender el comportamiento de las ventas, los productos, los clientes y los mercados.

A través de un proceso de análisis exploratorio, preparación de datos y visualización, se investigan diferentes dimensiones del negocio para identificar patrones, detectar oportunidades y acompañar la toma de decisiones comerciales.

---

# 📁 1. Origen de los datos

Para desarrollar este proyecto se utilizó el conjunto de datos **Online Retail**, publicado en el [UCI Machine Learning Repository](https://doi.org/10.24432/C5BW33).

El dataset original contiene **541.909 registros de transacciones comerciales** de una empresa minorista británica dedicada a la venta online, correspondientes al período comprendido entre el 1 de diciembre de 2010 y el 9 de diciembre de 2011.

Cada registro representa una línea de factura e incluye información sobre:

- Número de factura.
- Código y descripción del producto.
- Cantidad vendida.
- Fecha de facturación.
- Precio unitario.
- Identificación del cliente.
- País.

**Referencia bibliográfica:**

Chen, D. (2015). *Online Retail* [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5BW33

**Licencia:** Creative Commons Attribution 4.0 International (CC BY 4.0).

---

# 🧹 2. Preparación y limpieza de los datos

Para este proyecto se trabajó con una **muestra de 400 registros** del conjunto original.

El proceso de preparación se realizó utilizando Python y Pandas, e incluyó la exploración de la estructura de los datos, la revisión de su calidad y la preparación de las variables necesarias para el análisis.

Como resultado se generó un archivo limpio y estructurado, exportado en formato CSV para su utilización en Power BI.

**Archivo utilizado para el análisis y el dashboard:**

`data/Online_Retail_limpio_para_PowerBI.csv`

El archivo contiene 400 registros y 9 columnas, incluyendo la variable adicional de ingresos estimados.

Se conservaron los 97 registros sin identificación de cliente, así como las cantidades negativas y los precios unitarios iguales a cero, de acuerdo con los criterios de preparación documentados en el notebook. Estas situaciones se consideran al interpretar los resultados.

**Importante:** todos los indicadores, gráficos y conclusiones del dashboard corresponden a esta muestra de 400 registros, no al conjunto completo de 541.909 transacciones.

---

# 🎯 3. Objetivo del proyecto

Comprender dónde se genera el valor del negocio a partir del análisis de las transacciones comerciales.

La investigación busca responder cinco preguntas principales:

1. ¿Cómo evolucionan los ingresos a lo largo del tiempo?
2. ¿Qué productos generan mayor contribución económica?
3. ¿Existe una relación directa entre unidades vendidas e ingresos?
4. ¿Qué mercados concentran la actividad comercial?
5. ¿Qué información tenemos disponible sobre nuestros clientes?

---

# 🔎 4. La investigación: ¿dónde está el valor de nuestro negocio?

## 4.1. Todo comienza con una pregunta

Imaginemos que somos responsables de un negocio. Tenemos productos, clientes, mercados, ventas e ingresos.

Pero ¿sabemos realmente dónde está el valor?

- ¿Los productos que más se venden son también los que más ingresos generan?
- ¿Todos los mercados tienen la misma importancia?
- ¿Conocemos realmente a nuestros clientes?

Decidí explorar estas preguntas porque detrás de cada transacción puede haber información que no resulta evidente a simple vista.

## 4.2. Comienza la investigación

A partir de la muestra de 400 registros, se realizó un proceso de preparación, exploración y análisis.

Utilicé **Python y Pandas** para procesar los datos y **Power BI y DAX** para construir un dashboard interactivo.

La investigación se organizó en cinco dimensiones:

- Evolución de los ingresos.
- Comportamiento de los productos.
- Relación entre unidades vendidas e ingresos.
- Distribución geográfica del negocio.
- Identificación de clientes.

## 4.3. Primera pista: ¿más ventas significan más ingresos?

Al analizar los productos, encontramos dos casos interesantes:

| Producto | Unidades vendidas | Ingresos estimados |
|---|---:|---:|
| SURTIDO COLORS SILK FAN | 600 | US$ 614,06 |
| LAUNDRY 15C METAL CARTEL | 288 | US$ 770,88 |

El segundo producto generó más ingresos con menos unidades vendidas.

**Primera conclusión:** vender más unidades no significa necesariamente generar más ingresos.

## 4.4. Segunda pista: ¿dónde se genera el negocio?

El análisis geográfico mostró una fuerte concentración:

- Reino Unido: 86,3 % de los ingresos.
- Otros mercados: 13,7 %.

Este resultado invita a analizar la dependencia comercial de un mercado y explorar oportunidades de diversificación.

## 4.5. Tercera pista: ¿conocemos realmente a nuestros clientes?

De los 400 registros analizados, 97 no tienen identificado el número de cliente.

Esto representa el **24,25 % de la muestra**.

La falta de identificación limita la posibilidad de analizar recurrencia, fidelización y comportamiento de compra de esos clientes.

## 4.6. El descubrimiento

La investigación permitió identificar tres aspectos relevantes:

- El volumen de unidades vendidas no siempre refleja la contribución económica de un producto.
- Los ingresos presentan una importante concentración geográfica.
- La calidad y disponibilidad de los datos de clientes condicionan el análisis comercial.

## 4.7. El desenlace: de los datos a las decisiones

Los hallazgos permiten plantear nuevas preguntas y posibles acciones:

- Analizar el surtido considerando su contribución económica, además del volumen de ventas.
- Explorar oportunidades para diversificar los mercados.
- Mejorar la identificación de clientes para fortalecer los análisis de comportamiento y fidelización.

Porque encontrar el valor de un negocio no consiste solamente en contar cuánto vendemos. Consiste en comprender qué hay detrás de esos números y qué decisiones podemos tomar a partir de ellos.

---

# 📊 5. Dashboard | Análisis Comercial

![Dashboard Online Retail](powerbi/results/Imagen%20Dashboard%20Mariela%20Eckl.JPG)

El dashboard fue desarrollado en Power BI con una estructura de una página principal, orientada a facilitar la lectura de los indicadores y la exploración de los resultados.

## Indicadores principales (KPIs)

| Indicador | Descripción |
|---|---|
| Ingresos Estimados USD | Ingresos estimados expresados en dólares |
| Cantidad Facturas | Cantidad de facturas diferentes |
| Unidades Vendidas | Suma de unidades registradas |
| Clientes Identificados | Cantidad de clientes con identificador disponible |
| Ticket Promedio USD | Ingresos estimados por factura |

## Visualizaciones

- Evolución mensual de ingresos.
- Distribución geográfica de ingresos.
- Productos destacados por ingresos estimados.
- Comparación entre unidades vendidas e ingresos.
- Hallazgos principales de la investigación.

## Interactividad

El dashboard permite explorar los resultados mediante filtros por:

- Mes.
- Año.
- País.

También incorpora navegación mediante botones para futuras secciones de análisis.

## Archivos del dashboard

- [Ver dashboard en PDF](powerbi/results/Ejercicio%20Final%20Mariela%20Eckl%20-%20Analisis%20de%20Datos.pdf)
- [Descargar archivo Power BI (.pbix)](powerbi/Ejercicio%20Final%20Mariela%20Eckl%20-%20Analisis%20de%20Datos.pbix)
- [Ver imagen del dashboard](powerbi/results/Imagen%20Dashboard%20Mariela%20Eckl.JPG)

---

# 🛠️ 6. Herramientas y metodología

| Herramienta | Aplicación |
|---|---|
| Python | Procesamiento y análisis de datos |
| Pandas | Exploración, limpieza y transformación |
| Power BI | Visualización y dashboard interactivo |
| DAX | Creación de medidas e indicadores |
| Google Colab | Desarrollo y documentación del análisis |
| GitHub | Publicación y organización del proyecto |

## Medidas principales en DAX

Se desarrollaron medidas para calcular los principales indicadores del dashboard:

- Ingresos estimados.
- Ingresos estimados en USD.
- Cantidad de facturas.
- Unidades vendidas.
- Clientes identificados.
- Ticket promedio.
- Ticket promedio en USD.

---

# 💱 7. Criterio de conversión monetaria

Los precios originales del dataset están expresados en libras esterlinas (GBP).

Para facilitar la lectura de los indicadores, se incorporó una conversión a dólares estadounidenses (USD) utilizando un factor fijo de **1,5745 USD/GBP**.

Este factor corresponde al promedio simple de los tipos de cambio anuales utilizados para 2010 y 2011.

Se trata de una conversión de referencia aplicada de manera uniforme, no de un tipo de cambio específico para cada transacción.

---

# 📌 8. Alcance y consideraciones sobre los resultados

Para interpretar correctamente los resultados, es importante tener en cuenta que:

- El análisis se realizó sobre una muestra de 400 registros.
- Los resultados no representan necesariamente el comportamiento del conjunto completo de transacciones.
- Se conservaron registros sin identificación de cliente.
- Las cantidades negativas y los precios unitarios iguales a cero se mantuvieron según los criterios documentados en el proceso de preparación.
- Los ingresos se expresan como estimaciones calculadas a partir de cantidad por precio unitario.
- Los importes en USD utilizan un factor de conversión fijo.

Por lo tanto, las conclusiones deben interpretarse dentro del alcance y las características de esta muestra.

---

# 📂 9. Estructura del repositorio

```text
proyecto-final-analisis-datos/
│
├── data/
│   ├── Online_Retail_limpio_para_PowerBI.csv
│   └── Online_Retail_muestra_400_filas.csv
│
├── notebooks/
│   ├── TP_FINAL_Procesamiento_de_Datos_Mariela_Eckl_con_exportacion_PowerBI.ipynb
│   └── TP_M1_Procesamiento_de_Datos_Mariela_Eckl.ipynb
│
├── powerbi/
│   ├── Ejercicio Final Mariela Eckl - Analisis de Datos.pbix
│   │
│   └── results/
│       ├── Ejercicio Final Mariela Eckl - Analisis de Datos.pdf
│       └── Imagen Dashboard Mariela Eckl.JPG
│
└── README.md
```

---

# 👩‍💻 10. Autora

**Mariela Eckl**
https://www.linkedin.com/in/mariela-eckl/ 
Proyecto desarrollado como trabajo final del curso de Herramientas de Análisis de Datos.

Intereses profesionales: análisis de datos, métricas, Business Intelligence y mejora de procesos.

[LinkedIn – Mariela Eckl](https://www.linkedin.com/in/mariela-eckl/)

---

*Un proyecto de análisis de datos no termina cuando construimos un dashboard. Termina cuando logramos transformar la información en preguntas, descubrimientos y decisiones.*
