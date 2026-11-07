# 📊 Proyecto Final | Data Analytics

## ¿Dónde está el valor de nuestro negocio?
### Una investigación a través de los datos de Online Retail

Este proyecto explora una muestra de 400 registros de transacciones comerciales para comprender el comportamiento de las ventas, los productos, los clientes y los mercados.

El objetivo es transformar datos en información que permita identificar oportunidades y acompañar la toma de decisiones comerciales.

---

## 📸 Dashboard | Análisis Comercial

![Dashboard Online Retail](powerbi/results/Imagen%20Dashboard%20Mariela%20Eckl.JPG)

**Archivos del proyecto:**

- [Ver Dashboard en PDF](powerbi/results/Ejercicio%20Final%20Mariela%20Eckl%20-%20Analisis%20de%20Datos.pdf)
- [Descargar archivo Power BI (.pbix)](powerbi/Ejercicio%20Final%20Mariela%20Eckl%20-%20Analisis%20de%20Datos.pbix)
- [Consultar datos procesados (.csv)](data/Online_Retail_limpio_para_PowerBI.csv)

---

# 🔎 La investigación

## 1. Todo comienza con una pregunta

Imaginemos que somos responsables de un negocio. Tenemos productos, clientes, mercados, ventas e ingresos.

Pero ¿sabemos realmente dónde está el valor?

- ¿Los productos que más se venden son también los que más ingresos generan?
- ¿Todos los mercados tienen la misma importancia?
- ¿Conocemos realmente a nuestros clientes?

Decidí explorar estas preguntas porque detrás de cada transacción puede haber información que no resulta evidente a simple vista.

## 2. Comienza la investigación

Trabajé con una muestra de 400 registros del conjunto de datos Online Retail.

El proceso incluyó preparación, revisión de calidad y transformación de los datos para convertirlos en información útil para el análisis.

Utilicé **Python y Pandas** para el procesamiento y análisis de los datos, y **Power BI y DAX** para construir un dashboard interactivo.

La investigación se organizó en cinco dimensiones:

1. Evolución de los ingresos.
2. Comportamiento de los productos.
3. Relación entre unidades vendidas e ingresos.
4. Distribución geográfica del negocio.
5. Identificación de clientes.

## 3. Primera pista: ¿más ventas significan más ingresos?

Al analizar los productos, encontramos dos casos interesantes:

| Producto | Unidades vendidas | Ingresos estimados |
|---|---:|---:|
| SURTIDO COLORS SILK FAN | 600 | US$ 614,06 |
| LAUNDRY 15C METAL CARTEL | 288 | US$ 770,88 |

El segundo producto generó más ingresos con menos unidades vendidas.

**Primera conclusión:** vender más unidades no significa necesariamente generar más ingresos.

## 4. Segunda pista: ¿dónde se genera el negocio?

El análisis geográfico mostró una fuerte concentración:

- Reino Unido: 86,3 % de los ingresos.
- Otros mercados: 13,7 %.

Este resultado invita a analizar la dependencia comercial de un mercado y explorar oportunidades de diversificación.

## 5. Tercera pista: ¿conocemos realmente a nuestros clientes?

De los 400 registros analizados, 97 no tienen identificado el número de cliente.

Esto representa el **24,25 % de la muestra**.

La falta de identificación limita la posibilidad de analizar recurrencia, fidelización y comportamiento de compra de esos clientes.

## 6. El descubrimiento

La investigación permitió identificar tres aspectos relevantes:

- El volumen de unidades vendidas no siempre refleja la contribución económica de un producto.
- Los ingresos presentan una importante concentración geográfica.
- La calidad y disponibilidad de los datos de clientes condicionan el análisis comercial.

## 7. El desenlace: de los datos a las decisiones

Los hallazgos permiten plantear nuevas preguntas y posibles acciones:

- Analizar el surtido considerando su contribución económica, además del volumen de ventas.
- Explorar oportunidades para diversificar los mercados.
- Mejorar la identificación de clientes para fortalecer los análisis de comportamiento y fidelización.

Porque encontrar el valor de un negocio no consiste solamente en contar cuánto vendemos. Consiste en comprender qué hay detrás de esos números y qué decisiones podemos tomar a partir de ellos.

---

# 🛠️ Herramientas y metodología

| Herramienta | Aplicación |
|---|---|
| Python | Procesamiento y análisis de datos |
| Pandas | Limpieza y transformación |
| Power BI | Visualización y dashboard interactivo |
| DAX | Medidas e indicadores |
| GitHub | Documentación y versionado del proyecto |

## Indicadores del dashboard

- Ingresos estimados en USD.
- Cantidad de facturas.
- Unidades vendidas.
- Clientes identificados.
- Ticket promedio en USD.

El dashboard incorpora filtros por mes, año y país, permitiendo explorar los resultados desde distintas perspectivas.

---

# 📂 Estructura del repositorio

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

# 📌 Consideraciones sobre los datos

- El análisis presentado en el dashboard corresponde a una muestra de 400 registros, no al conjunto completo de Online Retail.
- Se conservaron los registros sin identificación de cliente para documentar la calidad de los datos.
- Se incorporó la variable de ingresos estimados, calculada a partir de cantidad por precio unitario.
- Los importes originales están expresados en libras esterlinas (GBP).
- Para presentar los importes en USD se utilizó un factor de conversión fijo de 1,5745 USD/GBP, calculado como el promedio simple de los tipos de cambio anuales utilizados para 2010 y 2011. No representa una conversión al tipo de cambio de cada transacción.

**Nota:** Los resultados y conclusiones deben interpretarse dentro del alcance de esta muestra.

---

## 👩‍💻 Autora

**Mariela Eckl**

Proyecto desarrollado como trabajo final de formación en Análisis de Datos.

Interés profesional: análisis de datos, métricas, Business Intelligence y mejora de procesos.

[LinkedIn](https://www.linkedin.com/in/mariela-eckl/)
