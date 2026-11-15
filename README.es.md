# sprint7-final-project 🌐 **Idioma Actual:** Español | Switch to: [English](README.md)

# 📊 ConnectaTel — Análisis del Uso de los Clientes

Proyecto de Análisis Exploratorio de Datos (EDA) enfocado en comprender el comportamiento de los clientes, identificar patrones de uso y desarrollar segmentos de clientes que permitan respaldar la toma de decisiones empresariales basadas en datos.

---

## 📌 Descripción del Proyecto

Este proyecto analiza la información de los clientes y los datos de uso de los servicios de telecomunicaciones de **ConnectaTel**, con el objetivo de comprender cómo interactúan los usuarios con los servicios de la empresa.

Mediante la limpieza de datos, el análisis exploratorio, los resúmenes estadísticos y la segmentación de clientes, se busca identificar patrones relevantes que ayuden a mejorar la oferta de servicios, fortalecer la retención de clientes y desarrollar estrategias comerciales más específicas.

## 🎯 Objetivos

- Evaluar la calidad y consistencia de los conjuntos de datos disponibles.
- Identificar y tratar valores ausentes y registros inválidos.
- Explorar las características demográficas de los clientes y sus patrones de uso de los servicios.
- Detectar y evaluar posibles valores atípicos.
- Segmentar a los clientes según su edad y nivel de uso.
- Transformar los hallazgos del análisis en recomendaciones empresariales aplicables.

## 🗂️ Conjuntos de Datos

El análisis utiliza tres conjuntos de datos:

| Conjunto de datos | Descripción |
| ------- | ------- |
| `users` | Información de los clientes, incluyendo edad, ciudad, fecha de registro y detalles de suscripción. |
| `plans` | Información sobre los planes de telecomunicaciones disponibles y sus características. |
| `usage` | Registros de actividad de los clientes, incluyendo llamadas y mensajes de texto. |

Los archivos CSV originales están incluidos en la carpeta [`datasets/`](datasets/):

- `plans.csv`
- `users_latam.csv`
- `usage.csv`

## 🛠️ Herramientas y Tecnologías

- **Python** — Análisis y manipulación de datos.
- **Pandas** — Limpieza, transformación y agregación de datos.
- **NumPy** — Operaciones numéricas.
- **Matplotlib** — Visualización de datos.
- **Seaborn** — Visualizaciones estadísticas.
- **Jupyter Notebook** — Análisis interactivo y documentación.
- **GitHub** — Control de versiones y documentación del proyecto.

## 🔎 Flujo de Trabajo del Análisis

El proyecto sigue un proceso estructurado de análisis de datos:

**1. Exploración de Datos**

- Se inspeccionaron las dimensiones de los conjuntos de datos, los tipos de columnas y su estructura general.
- Se revisaron las estadísticas descriptivas y se identificaron problemas iniciales relacionados con la calidad de los datos.

**2. Limpieza de Datos**

- Se identificaron valores ausentes e inconsistentes.
- Se corrigieron valores inválidos en la variable de edad.
- Se revisaron las fechas de registro que estaban fuera del período de análisis.
- Se evaluaron los valores ausentes en los registros de llamadas y mensajes.

**3. Preparación de Datos**

- Se convirtieron las columnas de fechas a los tipos de datos adecuados.
- Se crearon variables auxiliares para distinguir llamadas y mensajes de texto.
- Se agregaron los datos de uso por cliente.
- Se combinaron los datos de clientes y uso para construir un perfil consolidado.

**4. Análisis Exploratorio de Datos (EDA)**

- Se examinaron las distribuciones de edad y uso de los clientes.
- Se compararon los patrones de actividad entre los diferentes planes de suscripción.
- Se utilizaron histogramas y diagramas de caja (*boxplots*) para explorar las distribuciones y los posibles valores atípicos.

**5. Análisis de Valores Atípicos**

- Se identificaron observaciones extremas en las variables de edad, llamadas, mensajes y duración acumulada de llamadas.
- Se evaluó si estas observaciones representaban errores o comportamientos de consumo potencialmente relevantes de los clientes.

**6. Segmentación de Clientes**

- Se clasificaron los clientes en tres grupos de edad: Jóvenes, Adultos y Adultos Mayores.
- Se clasificaron los clientes en tres grupos según su nivel de uso: Bajo, Medio y Alto.

**7. Hallazgos y Recomendaciones de Negocio**

- Se interpretaron los segmentos de clientes identificados.
- Se identificaron posibles oportunidades para mejorar la retención de clientes y los servicios ofrecidos.
- Se propusieron recomendaciones para adaptar los planes de telecomunicaciones a los patrones de consumo de los clientes.

## 📈 Principales Hallazgos

### Segmentación por Edad

La base de clientes se dividió en tres grupos de edad:

| Segmento | Clientes | Porcentaje |
| ----------- | --------- | ---------- |
| Joven | 760 | 19,00 % |
| Adulto | 2.018 | 50,45 % |
| Adulto Mayor | 1.222 | 30,55 % |
| **Total** | **4.000** | **100 %** |

Los adultos representan el segmento más numeroso, con aproximadamente la mitad de la base total de clientes.

### Segmentación por Nivel de Uso

Los clientes se clasificaron según su actividad de llamadas y mensajes de texto:

| Segmento | Clientes | Porcentaje |
| ------------ | --------- | ---------- |
| Bajo uso | 778 | 19,45 % |
| Uso medio | 2.943 | 73,58 % |
| Alto uso | 279 | 6,98 % |
| **Total** | **4.000** | **100 %** |

Los clientes con un nivel de uso medio representan el segmento más numeroso, mientras que los usuarios de alto uso constituyen una proporción menor de la base de clientes.

### Análisis de Valores Atípicos

Se identificaron posibles valores atípicos en la cantidad de llamadas y mensajes, así como en la duración acumulada de llamadas.

Estas observaciones se conservaron porque no existía evidencia suficiente para clasificarlas como errores de registro. Podrían representar clientes con una actividad elevada legítima y proporcionar información útil para la toma de decisiones empresariales.

## 💡 Recomendaciones de Negocio

A partir del análisis, se identificaron las siguientes oportunidades:

- **Clientes de alto uso:** Evaluar planes con mayores capacidades de consumo y beneficios adicionales para mejorar la retención.
- **Clientes de bajo uso:** Considerar paquetes económicos e incentivos promocionales que fomenten un mayor aprovechamiento de los servicios.
- **Clientes de uso medio:** Mantener planes competitivos que respondan a las necesidades del segmento más numeroso.
- **Personalización de clientes:** Explorar estrategias basadas en las características demográficas y los patrones de consumo.
- **Monitoreo del uso:** Realizar seguimiento a los clientes con niveles de actividad inusualmente elevados para identificar oportunidades de fidelización y optimización de planes.

## 🚀 Cómo Ejecutar el Proyecto

Puedes reproducir el análisis utilizando Google Colab o Jupyter Notebook.

### Opción 1 — Google Colab

1. Descarga o clona este repositorio.
2. Ingresa a [Google Colab](https://colab.research.google.com/).
3. Sube el notebook `.ipynb`.
4. Sube los conjuntos de datos CSV necesarios.
5. Actualiza las rutas de los archivos si es necesario.
6. Ejecuta las celdas del notebook en orden secuencial.

### Opción 2 — Entorno Local

Clona el repositorio:

```bash
git clone <repository-url>
cd <repository-folder>
```

Instala las librerías necesarias:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

Inicia Jupyter Notebook:

```bash
jupyter notebook
```

Abre el notebook del proyecto y ejecuta las celdas en orden.

**Nota:** El notebook se incluye en su formato original. Las rutas de los archivos CSV apuntan al entorno local donde se desarrolló el proyecto, por lo que es posible que debas adaptarlas en tu propia copia de trabajo para utilizar los archivos de la carpeta `datasets/`. El notebook entregado no ha sido modificado.

## 📁 Estructura del Repositorio

```text
sprint7-final-project/
│
├── datasets/
│   ├── plans.csv
│   ├── users_latam.csv
│   ├── usage.csv
│   └── .gitkeep
│
├── JEOO-S7-Project-ConnectaTel.ipynb
├── README.md
└── README.es.md
```

## 👨‍💻 Autor

**Juan Esteban Ochoa Osorio**

Estudiante de Análisis de Datos | Bootcamp TripleTen

[Perfil de GitHub](https://github.com/Kathavx)

---

*Este proyecto fue desarrollado como parte del Bootcamp de Data Analyst de TripleTen.*
