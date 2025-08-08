# 📊 Análisis de Ventas de Videojuegos (Kaggle Dataset)

Este proyecto consiste en un **Análisis Exploratorio de Datos (EDA)** sobre tres datasets extraídos de Kaggle, enfocados en las ventas globales de videojuegos para diferentes consolas, incluyendo **PS4**, **Xbox One** y un dataset principal con múltiples plataformas.

El objetivo principal fue **limpiar, explorar y visualizar** los datos para identificar tendencias, plataformas y publishers más exitosos, así como analizar relaciones entre ventas y puntuaciones de críticos y usuarios.

---

## 📂 Estructura del Proyecto

El proyecto está dividido en tres notebooks / scripts principales:

1. **`ps4.ipynb`** → Análisis y visualizaciones exclusivas de PS4.  
2. **`xbox.ipynb`** → Análisis y visualizaciones exclusivas de Xbox One.  
3. **`main.py`** → Análisis y visualizaciones sobre el dataset general con todas las plataformas.

---

## 🛠️ Metodología

### A. Limpieza de Datos

**PS4 y Xbox One**
- Normalización de géneros (ej. `Action` → `Action-Adventure`).
- Homologación de nombres de publishers.
- Imputación de valores faltantes (`Unknown`, medianas, modas).
- Eliminación de registros de 2019 y 2020.
- Conversión de ventas de “decenas de millones” a “millones”.

**Dataset principal**
- Renombrado de columnas para consistencia.
- Eliminación de valores nulos en `Year`.
- Relleno de valores faltantes con mediana, moda o `Unknown`.
- Conversión de `Staff_Score` a escala de 0 a 10.

---

## 📈 Principales Visualizaciones

### 1. Distribuciones Generales
- **Distribución de juegos por año**
- **Distribución de juegos por género**
- **Distribución de juegos por plataforma**
- **Distribución de juegos por clasificación (rating)**

![Distribución de juegos](images\main_dist.png)

---

### 2. Rankings por Ventas

- **Top 10 juegos más vendidos por consola**
- **Top 10 juegos más vendidos por año**
- **Top 10 juegos más vendidos por género**
- **Top 10 juegos más vendidos por publisher**

![Top 10 por consola](images\main_top10g_top12c.png)  
![Top 10 por año](images\main_top10g_top12y.png)  
![Top 10 por género](images\main_top10g_top12gen.png)  
![Top 10 por publisher](images\main_top10g_top12pub.png)

---

### 3. Ventas por Región
- Comparativa de plataformas más exitosas en **Norteamérica**, **Europa**, **Japón** y **Otros**.
  
![Ventas por región](images\main_top10_plat_x_reg.png)

---

### 4. Relaciones entre Variables
- **Critic Score vs. Critic Count**
- **User Score vs. User Count**
- Comparativas por género, rating y plataforma.
- Pairplots de puntuaciones y ventas por región.

![Pairplot puntuaciones](images\main_users_x_staff.png)  
![Stripplot género-score](images\main_g_r_p_x_staff_user.png)
![Pairplot puntuaciones](images\main_y_x_user_staff_sales.png)  

### 4. PS4 y XBOX

![PS4 Publisher vs Años](images\ps4_pub_vs_ans.png)
![PS4 Publisher vs Años](images\ps4_top10.png)
![PS4 Publisher vs Años](images\xbox_pub_vs_ans.png)
![PS4 Publisher vs Años](images\xbox_pub_vs_ans.png)

---

## 📌 Hallazgos Clave

- Las plataformas con mayor venta global tienden a tener un catálogo amplio de títulos, no solo pocos éxitos masivos.
- El género **Action-Adventure** domina en ventas globales tanto en PS4 como en Xbox One.
- Algunos publishers, como **Sony Interactive** y **Activision**, mantienen posiciones destacadas a lo largo de los años.
- Existe una correlación positiva moderada entre la puntuación de Staff y las ventas globales, aunque no es determinante.

---

## 🚀 Tecnologías Utilizadas
- **Python**  
- **Pandas** → Manipulación y limpieza de datos.  
- **Matplotlib** y **Seaborn** → Visualizaciones estáticas.  

---

## 📂 Datasets
- [`Video_Games_Sales_as_at_22_Dec_2016.csv`](https://www.kaggle.com/datasets)  
- [`PS4_GamesSales.csv`](https://www.kaggle.com/datasets)  
- [`XboxOne_GameSales.csv`](https://www.kaggle.com/datasets)  

---

## ✨ Autor
[Christian Vizcardo]
[www.linkedin.com/in/christian-vizcardo]
---
