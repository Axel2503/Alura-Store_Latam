# 🏬 Análisis Estratégico de Tiendas AluraStore

## 📌 Objetivo del Proyecto
Este proyecto realiza un **análisis comparativo del rendimiento de cuatro sucursales (Tienda 1, Tienda 2, Tienda 3 y Tienda 4)** de **AluraStore**.  
El objetivo final es **identificar la sucursal con el rendimiento más bajo** y proporcionar una **recomendación estratégica fundamentada al Sr. Juan** sobre cuál tienda debería considerar vender.

---

## 📊 Los Datos
El análisis se basa en **cuatro conjuntos de datos independientes**, cada uno correspondiente a las transacciones de una sucursal:
base-de-datos-challenge1-latam/
- tienda_1.csv
- tienda_2.csv
- tienda_3.csv
- tienda_4.csv


Cada archivo fue cargado y consolidado en un único **DataFrame de pandas**, agregando una columna `tienda` para segmentar correctamente los registros.

---

## ⚙️ Metodología y Análisis Realizado
El análisis se estructuró en **5 pasos principales**, los cuales se desarrollan dentro del notebook [`AluraStoreLatam.ipynb`](AluraStoreLatam.ipynb):

### 1️⃣ Ingresos Totales (Facturación)
Se calculó la facturación total de cada tienda sumando los valores de la columna **`Precio`**.  
Este indicador refleja la **salud financiera y volumen de negocio** de cada sucursal.

### 2️⃣ Ventas por Categoría
Las ventas se agruparon por **`Tienda`** y **`Categoría del Producto`**, permitiendo identificar los productos más populares y el **mix de venta predominante**.

### 3️⃣ Satisfacción del Cliente (Calificaciones)
Se calculó la **calificación promedio** de las compras (`Calificación`) para evaluar la **experiencia del cliente y percepción de marca**.

### 4️⃣ Análisis de Productos (Más y Menos Vendidos)
Se identificaron los **5 productos más vendidos y los 5 menos vendidos** por tienda.  
También se generaron gráficos con los **10 productos más populares**, almacenados en la carpeta:
/graficos_top_productos/
*├── top_10_productos_Tienda_1.png
*├── top_10_productos_Tienda_2.png
*├── top_10_productos_Tienda_3.png
*└── top_10_productos_Tienda_4.png


### 5️⃣ Costo de Envío Promedio
Se calculó el **costo de envío promedio (`Costo de envío`)** por tienda.  
Un costo elevado puede **afectar negativamente la conversión de ventas y la satisfacción del cliente**.

---

## 🧱 Estructura del Proyecto
.
*├── 📄 AluraStoreLatam.ipynb # Notebook principal con el código de análisis
*├── 📄 Informe_Final_AluraStore.md # Informe ejecutivo con la recomendación
*├── 📄 README.md # Este archivo
│
*├── 📁 base-de-datos-challenge1-latam/
*│ ├── tienda_1.csv
*│ ├── tienda_2.csv
*│ ├── tienda_3.csv
*│ └── tienda_4.csv
│
*└── 📁 graficos_top_productos/
*├── top_10_productos_Tienda_1.png
*├── top_10_productos_Tienda_2.png
*├── top_10_productos_Tienda_3.png
*└── top_10_productos_Tienda_4.png


---

## 🧭 Conclusión y Recomendación
El análisis de las cinco métricas principales permitió **detectar la tienda con el desempeño más bajo** en:
- Ingresos totales  
- Calificación promedio  
- Costos de envío  
- Mix de productos vendidos  

La **recomendación final** y su **justificación detallada** se encuentran documentadas en el archivo [`Informe_Final_AluraStore.md`](Informe_Final_AluraStore.md).

---

## 💻 Tecnologías Utilizadas
- **Python 3**
- **Pandas** → carga, limpieza y análisis de datos  
- **Matplotlib** → generación de visualizaciones  
- **Jupyter Notebook** → entorno interactivo para el desarrollo

---

## ✨ Autor
**Proyecto desarrollado por:**  
*Equipo de Análisis de Datos - AluraStore LATAM*  
📅 *Noviembre de 2025*
