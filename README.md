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

| Dataset | Descripción |
|---|---|
| **1. Calificaciones** | Predicción de calificaciones basada en factores socioeconómicos. |
| **2. Suicidios** | Tasas globales de suicidio e indicadores socioeconómicos. |

**Descarga de datasets:**

[Google Drive – Datasets del proyecto](https://drive.google.com/drive/folders/1sp9HoxjDZN1L6J8TAcZGyOnc-MIelEms?usp=sharing)

Los archivos originales deben almacenarse en `data/raw/` sin modificar su contenido. Los datasets resultantes de la limpieza se guardarán en `data/processed/`.

## 3. Integrantes del Grupo #2

| Integrante | Responsabilidad |
|---|---|
| Brandon Acuña Gamboa | Por asignar |
| Desmond Bermúdez Rodríguez | Por asignar |
| Andrei Calderón Vega | Por asignar |
| Mauricio Ortiz Coronado | Por asignar |
| Byron Pérez Aguilar | Por asignar |

## 4. Distribución del trabajo

| Parte | Área | Actividades principales |
|---|---|---|
| **1** | Carga y limpieza | Carga de datasets, dimensiones, tipos de variables, valores nulos, duplicados, inconsistencias, limpieza, etc. **Conclusiones.** |
| **2** | EDA estadístico | Estadísticas descriptivas, media, mediana, moda, varianza, desviación estándar, cuartiles, frecuencias, comparaciones, etc. **Conclusiones.** |
| **3** | EDA visual | Histogramas, boxplots, gráficos de barras, dispersión, correlaciones, mapas de calor, valores atípicos, etc. **Conclusiones.** |
| **4** | Preprocesamiento y selección de K | Selección de variables, codificación, escalado, método del codo (WCSS), gráfico del codo, selección de K, etc. **Conclusiones.** |
| **5** | K-Means y evaluación | Entrenamiento, etiquetas, centroides, distribución de registros, coeficiente de silueta, PCA, comparación de clústeres, etc. **Conclusiones.** |

### Criterios de distribución

- **Partes 1, 2 y 5:** Cada responsable desarrolla su apartado en ambos datasets.
- **Partes 3 y 4:** Se distribuyen entre dos integrantes, considerando su carga de trabajo.
  - **Opción A:** Un integrante realiza las partes 3 y 4 de Calificaciones y otro las partes 3 y 4 de Suicidios.
  - **Opción B:** Un integrante realiza la parte 3 de Calificaciones y la parte 4 de Suicidios; el otro realiza la parte 4 de Calificaciones y la parte 3 de Suicidios.

Las actividades mencionadas son una guía y podrán ampliarse según las características de cada dataset.

**Cada apartado debe contener resultados, interpretaciones y una conclusión.**

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
│   │   ├── calificaciones.csv
│   │   └── suicidio.csv
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
    └── Distribucion_Trabajo.docx
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
