# Integración de Datos y Prospectiva de Riesgo Operacional

## Descripción

Proyecto final de la asignatura **Integración de Datos y Prospectiva**, desarrollado a partir de la integración y análisis de dos fuentes de información relacionadas con eventos de riesgo operacional.

El proyecto utiliza una base interna correspondiente a **fallas tecnológicas en canales electrónicos de una entidad FINTECH** y una base externa asociada a **eventos operacionales de una terminal portuaria**. A partir de estas fuentes se busca identificar patrones comunes, evaluar la consistencia de los datos y desarrollar un análisis prospectivo que apoye la toma de decisiones frente a la gestión del riesgo operacional.

## Objetivo

Integrar dos fuentes de datos de sectores diferentes mediante metodologías de integración que permitan analizar el comportamiento del riesgo operacional y generar información útil para la toma de decisiones.

De manera específica, el proyecto busca:

- Integrar las dos bases de datos utilizando diferentes modelos de integración.
- Analizar la credibilidad y consistencia de las fuentes de información.
- Identificar relaciones entre variables operacionales y financieras.
- Analizar frecuencia, severidad y pérdidas asociadas a eventos de riesgo operacional.
- Desarrollar un análisis prospectivo orientado a la gestión y mitigación del riesgo.
- Analizar el potencial de captura de Gases de Efecto Invernadero (GEI) asociado a la mitigación de pérdidas operacionales.
- Generar recomendaciones para fortalecer la gestión del riesgo operacional.

## Datos

El proyecto utiliza dos fuentes de información:

### 1. Riesgo operacional – Fallas tecnológicas FINTECH

Base interna con registros históricos de eventos asociados a fallas tecnológicas en canales electrónicos.

Incluye variables relacionadas con:

- Fecha
- Transacciones diarias
- Valor transado
- Transacciones fallidas
- Valor generado promedio
- Descripción del evento

La base contiene inicialmente **706 registros**, de los cuales 5 corresponden a registros con valores faltantes que son tratados durante la etapa de preparación de los datos.

### 2. Riesgo operacional – Terminal portuaria

Base externa con información sobre eventos operacionales asociados a una terminal portuaria.

Incluye variables relacionadas con:

- Fecha
- Operaciones diarias
- Valor transado
- Operaciones fallidas
- Severidad
- Descripción del evento

La base contiene **1.000 registros**.

## Integración de las fuentes

La integración se plantea a partir de variables numéricas equivalentes entre ambas fuentes, permitiendo comparar comportamientos operacionales de sectores diferentes.

| FINTECH | Terminal portuaria |
|---|---|
| Transacciones diarias | Operaciones diarias |
| Valor transado | Valor transado |
| Transacciones fallidas | Operaciones fallidas |
| Valor generado promedio | Severidad |

El proyecto emplea dos enfoques principales de integración:

- **Integración mediante credibilidad**, considerando las características y consistencia de las fuentes.
- **Integración mediante aceptación y rechazo**, utilizando criterios estadísticos para determinar los registros que pueden ser incorporados al análisis.

## Metodología

El análisis se desarrolla mediante diferentes etapas:

1. **Carga y exploración de los datos**
2. **Limpieza y preparación de las bases**
3. **Análisis descriptivo de las variables**
4. **Análisis de correlaciones**
5. **Evaluación de la credibilidad de las fuentes**
6. **Integración de las bases mediante los métodos seleccionados**
7. **Análisis de frecuencia y severidad del riesgo operacional**
8. **Construcción de matrices de riesgo**
9. **Análisis prospectivo**
10. **Evaluación del potencial de captura de GEI**
11. **Interpretación de resultados y formulación de recomendaciones**

## Tecnologías utilizadas

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy

## Estructura del repositorio

```text
data-integration-operational-risk/
│
├── README.md
├── Proyecto_Final_Integracion_Datos.ipynb
│
└── data/
    ├── 5. Riesgo Operacional FallasTecnológicas (1).xlsx
    └── 6__RiesgoOperacional_TerminalPortuaria (1).xlsx
