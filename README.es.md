# sprint7-final-project 🌐 **Idioma Actual:** Español | Switch to: [English](README.md)

# 📊 ConnectaTel — Análisis de uso de los clientes

Proyecto de Análisis Exploratorio de Datos (EDA) centrado en comprender el comportamiento de los clientes, identificar patrones de uso y desarrollar segmentos de clientes para respaldar la toma de decisiones empresariales basadas en datos.

---

## 📌 Descripción general del proyecto

Este proyecto analiza información de los clientes y datos de uso de servicios de telecomunicaciones de **ConnectaTel**, con el objetivo de comprender cómo interactúan los usuarios con los servicios de la empresa.

Mediante la limpieza de datos, el análisis exploratorio, la elaboración de resúmenes estadísticos y la segmentación de clientes, el proyecto busca identificar patrones relevantes que ayuden a la empresa a mejorar su oferta de servicios, fortalecer la retención de clientes y desarrollar estrategias comerciales más específicas.

## 🎯 Objetivos

- Evaluar la calidad y consistencia de los conjuntos de datos disponibles.
- Identificar y gestionar valores faltantes y registros no válidos.
- Explorar los datos demográficos de los clientes y sus patrones de uso de los servicios.
- Detectar y evaluar posibles valores atípicos (*outliers*).
- Segmentar a los clientes según su edad e intensidad de uso.
- Traducir los hallazgos analíticos en recomendaciones empresariales accionables.

## 🗂️ Conjuntos de datos

El análisis utiliza tres conjuntos de datos:

| Conjunto de datos | Descripción |
|---|---|
| `users` | Información de los clientes, incluyendo edad, ciudad, fecha de registro y detalles de la suscripción. |
| `plans` | Información sobre los planes de telecomunicaciones disponibles y sus características. |
| `usage` | Registros de la actividad de los clientes, incluyendo llamadas y mensajes de texto. |

## 🛠️ Herramientas y tecnologías

- **Python** — Análisis y manipulación de datos.
- **Pandas** — Limpieza, transformación y agregación de datos.
- **NumPy** — Operaciones numéricas.
- **Matplotlib** — Visualización de datos.
- **Seaborn** — Visualizaciones estadísticas.
- **Jupyter Notebook** — Análisis interactivo y documentación.
- **GitHub** — Control de versiones y documentación del proyecto.

## 🔎 Flujo de trabajo del análisis

El proyecto sigue un proceso estructurado de análisis de datos:

**1. Exploración de datos**
- Inspección de las dimensiones de los conjuntos de datos, los tipos de columnas y la estructura general.
- Revisión de estadísticas descriptivas e identificación de problemas iniciales en la calidad de los datos.

**2. Limpieza de datos**
- Identificación de valores faltantes e inconsistentes.
- Corrección de valores de edad no válidos. - Se revisaron las fechas de registro fuera del periodo de análisis.
- Se evaluaron los valores faltantes en los registros de llamadas y mensajes.

**3. Preparación de datos**
- Se convirtieron las columnas de fecha a los tipos de datos adecuados.
- Se crearon variables auxiliares para distinguir entre llamadas y mensajes de texto.
- Se agregó la información de uso por cliente.
- Se combinó la información del cliente con la de uso para generar un perfil consolidado.

**4. Análisis exploratorio de datos**
- Se examinaron las distribuciones de la edad de los clientes y de su nivel de uso.
- Se compararon los patrones de actividad entre los distintos planes de suscripción.
- Se utilizaron histogramas y diagramas de caja (*boxplots*) para explorar las distribuciones y detectar posibles valores atípicos.

**5. Análisis de valores atípicos**
- Se identificaron observaciones extremas en cuanto a edad, llamadas, mensajes y duración acumulada de las llamadas.
- Se evaluó si dichas observaciones correspondían a errores o a comportamientos de los clientes potencialmente significativos.

**6. Segmentación de clientes**
- Se clasificó a los clientes en tres grupos de edad: Jóvenes, Adultos y Adultos mayores.
- Se clasificó a los clientes en tres grupos según su nivel de uso: Bajo, Medio y Alto.

**7. Perspectivas de negocio y recomendaciones**
- Se interpretaron los segmentos de clientes resultantes.
- Se identificaron posibles oportunidades para la retención de clientes y la mejora del servicio.
- Se formularon recomendaciones para adaptar los planes de telecomunicaciones a los patrones de uso de los clientes.

## 📈 Hallazgos clave

### Segmentación por edad

La base de clientes se dividió en tres grupos de edad:

| Segmento | Clientes | Porcentaje |
|---|---:|---:|
| Jóvenes | 760 | 19,00 % |
| Adultos | 2018 | 50,45 % |
| Adultos mayores | 1222 | 30,55 % |
| **Total** | **4000** | **100 %** |

Los adultos constituyen el segmento más numeroso, representando aproximadamente la mitad de la base de clientes.

### Segmentación por nivel de uso

Los clientes fueron clasificados según su actividad de llamadas y mensajes de texto:

| Segmento | Clientes | Porcentaje |
|---|---:|---:|
| Uso bajo | 778 | 19,45 % |
| Uso medio | 2943 | 73,58 % |
| Uso alto | 279 | 6,98 % |
| **Total** | **4000** | **100 %** |

Los clientes de uso medio constituyen el segmento más grande, mientras que los clientes de alto uso representan una proporción menor de la base de clientes.

## Análisis de valores atípicos

Se identificaron posibles valores atípicos en el número de llamadas y mensajes, así como en la duración acumulada de las llamadas.

Estas observaciones se mantuvieron, ya que no había pruebas suficientes para clasificarlas como errores de entrada de datos. Es posible que correspondan a clientes con un nivel de actividad realmente alto y que aporten información valiosa para la toma de decisiones empresariales.

## 💡 Recomendaciones para el negocio

A partir del análisis, se identificaron las siguientes oportunidades:

- **Clientes de alto uso:** Evaluar planes con mayores límites de consumo y beneficios adicionales para mejorar la retención.
- **Clientes de bajo uso:** Considerar paquetes asequibles e incentivos promocionales para fomentar el uso del servicio.
- **Clientes de uso medio:** Mantener planes competitivos que satisfagan sus necesidades.
