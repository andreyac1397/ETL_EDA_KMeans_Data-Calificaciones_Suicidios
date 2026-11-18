# Proyecto Final – Minería de Datos 1

**Colegio Universitario de Cartago (CUC)**  
**Carrera:** Tecnologías de la Información – Big Data  
**Curso:** MD1-152 – Minería de Datos 1  
**Profesor:** Ronald Córdoba Vega  
**Grupo:** #2  
**Periodo:** III Cuatrimestre, 2026

## 1. Descripción del proyecto

El proyecto tiene como objetivo aplicar técnicas de minería de datos mediante procesos de extracción, transformación y carga (ETL), análisis exploratorio de datos (EDA) y algoritmos de agrupamiento (clustering).

Se desarrollarán dos análisis independientes utilizando datasets previamente aprobados por el profesor, con el propósito de identificar patrones, relaciones y agrupaciones relevantes mediante el algoritmo K-Means.


## 2. Datasets aprobados

El proyecto desarrolla dos análisis independientes mediante técnicas de limpieza, exploración, preprocesamiento y agrupamiento con K-Means.

| Dataset | Archivo original | Objetivo |
|---|---|---|
| **1. Calificaciones** | `student_grade_ses_dataset.csv` | Identificar perfiles de estudiantes según características académicas, familiares y socioeconómicas. |
| **2. Suicidios** | `global_suicide_rates_real_who_worldbank.csv` | Identificar agrupaciones y patrones entre países o registros según las tasas de suicidio y los indicadores disponibles. |

**Descarga de datasets:**

[Google Drive – Datasets del proyecto](https://drive.google.com/drive/folders/1sp9HoxjDZN1L6J8TAcZGyOnc-MIelEms?usp=sharing)

Los archivos originales se conservan en `data/raw/` sin modificar su contenido. Los datasets procesados se almacenan en `data/processed/`.



## 3. Integrantes del Grupo #2

| Integrante | Responsabilidad |
|---|---|
| **Byron Pérez Aguilar** | Carga y limpieza de ambos datasets. |
| **Andrei Calderón Vega** | EDA estadístico y EDA visual de Calificaciones. |
| **Mauricio Ortiz Coronado** | EDA estadístico y EDA visual de Suicidios. |
| **Brandon Acuña Gamboa** | Preprocesamiento, selección de K, K-Means y evaluación de Calificaciones. |
| **Desmond Bermúdez Rodríguez** | Preprocesamiento, selección de K, K-Means y evaluación de Suicidios. |

## 4. Distribución del trabajo por dataset

### 4.1 Dataset 1: Calificaciones

| Parte | Actividad | Responsable |
|---|---|---|
| **01** | Carga, diagnóstico, limpieza y transformación (ETL) | Byron Pérez Aguilar |
| **02** | Análisis exploratorio estadístico (EDA) | Andrei Calderón Vega |
| **03** | Análisis exploratorio visual (EDA) | Andrei Calderón Vega |
| **04** | Preprocesamiento, selección de variables y selección de K | Brandon Acuña Gamboa |
| **05** | K-Means, evaluación e interpretación de clústeres | Brandon Acuña Gamboa |

### 4.2 Dataset 2: Suicidios

| Parte | Actividad | Responsable |
|---|---|---|
| **01** | Carga, diagnóstico, limpieza y transformación (ETL) | Byron Pérez Aguilar |
| **02** | Análisis exploratorio estadístico (EDA) | Mauricio Ortiz Coronado |
| **03** | Análisis exploratorio visual (EDA) | Mauricio Ortiz Coronado |
| **04** | Preprocesamiento, selección de variables y selección de K | Desmond Bermúdez Rodríguez |
| **05** | K-Means, evaluación e interpretación de clústeres | Desmond Bermúdez Rodríguez |

### 4.3 Actividades principales por etapa

| Parte | Actividades |
|---|---|
| **01. ETL** | Carga de datos, diagnóstico de calidad, tratamiento de nulos, duplicados, inconsistencias, valores atípicos y exportación del dataset procesado. |
| **02. EDA estadístico** | Estadísticas descriptivas, frecuencias, medidas de tendencia central y dispersión, análisis de variables y comparaciones entre grupos. |
| **03. EDA visual** | Histogramas, boxplots, gráficos de barras y dispersión, matrices de correlación, distribuciones y análisis visual de valores atípicos. |
| **04. Preprocesamiento** | Selección de variables, codificación de categorías, escalado, evaluación de valores atípicos, método del codo (WCSS) y selección de K. |
| **05. K-Means y evaluación** | Entrenamiento, asignación de clústeres, análisis de centroides, distribución de registros, coeficiente de silueta, visualización mediante PCA e interpretación de grupos. |

### 4.4 Criterios generales

- Cada responsable debe incluir código, resultados, interpretaciones y conclusiones en los apartados asignados.
- Los integrantes deben utilizar los archivos procesados generados durante el ETL.
- Los encargados del preprocesamiento deben considerar los hallazgos de los análisis estadísticos y visuales.
- Los responsables de K-Means deben justificar la selección de variables, el número de clústeres y las métricas de evaluación.
- Se deben coordinar los cambios que puedan afectar el trabajo de otros integrantes.
- Todos los integrantes deben conocer ambos datasets y comprender los resultados finales para la defensa del proyecto.

**Documento de distribución:** `docs/Distribucion_Proyecto_Mineria_Datos_Grupo_2.docx`


## 5. Estructura del repositorio

```text
Mineria_Datos_1/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── data/
│   ├── raw/
│   │   ├── student_grade_ses_dataset.csv
│   │   └── global_suicide_rates_real_who_worldbank.csv
│   └── processed/
│       ├── calificaciones_limpio.csv
│       └── suicidio_limpio.csv
│
├── notebooks/
│   ├── 01_Calificaciones/
│   │   ├── 01_Carga_Limpieza.ipynb
│   │   ├── 02_EDA_Estadistico.ipynb
│   │   ├── 03_EDA_Visual.ipynb
│   │   ├── 04_Preprocesamiento.ipynb
│   │   └── 05_KMeans_Evaluacion.ipynb
│   │
│   ├── 02_Suicidio/
│   │   ├── 01_Carga_Limpieza.ipynb
│   │   ├── 02_EDA_Estadistico.ipynb
│   │   ├── 03_EDA_Visual.ipynb
│   │   ├── 04_Preprocesamiento.ipynb
│   │   └── 05_KMeans_Evaluacion.ipynb
│   │
│   └── Finales/
│       ├── Calificaciones_Final.ipynb
│       └── Suicidio_Final.ipynb
│
├── entregables/
│   ├── HTML/
│   │   ├── Calificaciones.html
│   │   └── Suicidio.html
│   └── PowerPoint/
│       ├── Calificaciones.pptx
│       └── Suicidio.pptx
│
└── docs/
    └── Distribucion_Proyecto_Mineria_Datos_Grupo_2.docx
```

*Los nombres de los CSV son nombres de referencia y pueden ajustarse a los archivos originales.*

## 6. Herramientas y tecnologías

- Python
- Jupyter Notebook
- Pandas y NumPy
- Matplotlib y Seaborn
- Scikit-learn
- Git y GitHub
- PowerPoint

Las librerías necesarias se registrarán en `requirements.txt`.

## 7. Indicaciones para el desarrollo

1. Utilizar los datasets aprobados por el profesor.
2. Mantener los datos originales en `data/raw/`.
3. Guardar los datos limpios en `data/processed/`.
4. Desarrollar cada apartado en el notebook correspondiente.
5. Utilizar rutas relativas para acceder a los archivos.
6. No modificar el trabajo de otros integrantes sin coordinación.
7. Incluir títulos, explicaciones, resultados y conclusiones en cada apartado.
8. Mantener una secuencia lógica entre limpieza, EDA, preprocesamiento y clustering.
9. Coordinar previamente las variables utilizadas para K-Means.
10. Verificar que los notebooks finales se ejecuten correctamente de principio a fin.

## 8. Trabajo colaborativo con GitHub

**Repositorio oficial:**

https://github.com/andreyac1397/ETL_EDA_KMeans_Data-Calificaciones_Suicidios

### Ramas de trabajo

```text
main
├── feature/persona-1
├── feature/persona-2
├── feature/persona-3
├── feature/persona-4
└── feature/persona-5
```

### Procedimiento de trabajo

1. Clonar el repositorio.
2. Crear o utilizar la rama asignada.
3. Desarrollar los notebooks correspondientes.
4. Guardar y verificar los cambios.
5. Realizar commits con mensajes descriptivos.
6. Subir los cambios a GitHub.
7. Crear un Pull Request hacia `main`.
8. Revisar los cambios antes de integrarlos.

La rama `main` contendrá las versiones revisadas e integradas del proyecto.

## 9. Entregables

Se deben presentar los siguientes archivos:

| Entregable | Cantidad | Formato |
|---|---|---|
| Análisis completo de Calificaciones | 1 | HTML |
| Análisis completo de Suicidios | 1 | HTML |
| Presentación de Calificaciones | 1 | PowerPoint |
| Presentación de Suicidios | 1 | PowerPoint |

Los notebooks desarrollados en Jupyter se integrarán en un notebook final por dataset y posteriormente se exportarán a HTML.

**No se aceptarán archivos PDF como sustituto de los entregables solicitados.**

## 10. Fechas importantes

| Actividad | Fecha |
|---|---|
| **Entrega interna para revisión** | Martes 17 de noviembre de 2026, 2:00 p. m. |
| **Entrega oficial en CUCVirtual** | Jueves 19 de noviembre de 2026, antes de las 6:00 p. m. |
| **Defensa del proyecto** | Miércoles 25 de noviembre de 2026 |
| **Foro y actividades de defensa** | Miércoles 2 de diciembre de 2026 |

La entrega interna permitirá verificar el funcionamiento de los análisis, revisar las interpretaciones y corregir posibles errores antes de la fecha oficial.

## 11. Evaluación

| Criterio | Porcentaje |
|---|---:|
| Documento Jupyter exportado a HTML | 10 % |
| Defensa del proyecto | 5 % |
| Foro individual | 5 % |
| **Total** | **20 %** |

**Importante:** El profesor seleccionará el dataset que se defenderá y al integrante encargado de presentarlo. Podrá cambiar de participante durante la defensa. La calificación de la defensa será grupal.

Todos los integrantes deben conocer el funcionamiento de ambos análisis, independientemente de las partes que hayan desarrollado.

La participación en el foro es individual y es necesaria para obtener el porcentaje correspondiente. Se debe asistir con vestimenta adecuada a las actividades indicadas.

---

**Colegio Universitario de Cartago – Tecnologías de la Información, Big Data**  
Proyecto Final de Minería de Datos 1 – Grupo #2 – 2026
