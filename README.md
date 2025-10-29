# Predicción del Rendimiento Académico de Estudiantes
## Descripción General

Este proyecto tiene como objetivo predecir el rendimiento académico de los estudiantes en función de variables relacionadas con hábitos de estudio, asistencia, descanso y estilo de aprendizaje.
El análisis se ha abordado desde dos perspectivas complementarias:

### Clasificación: determinar si el alumno aprobará o no.

### Regresión: estimar la nota final obtenida por el estudiante.

El dataset utilizado contiene información de 1.000 estudiantes y combina variables numéricas y categóricas representativas del comportamiento académico.

##Objetivos del Proyecto

Identificar los factores que más influyen en el rendimiento de los estudiantes.

Desarrollar modelos predictivos robustos y comparables (clasificación y regresión).

Evaluar el desempeño mediante métricas estándar y validar la estabilidad de los resultados.

Proporcionar insights interpretables que sirvan para diseñar estrategias de mejora educativa.

## Estructura del Dataset
Tipo de variable	Columnas
Numéricas	horas_estudio_semanal, nota_anterior, tasa_asistencia, horas_sueno, edad, nota_final
Categóricas	nivel_dificultad, tiene_tutor, horario_estudio_preferido, estilo_aprendizaje
Variables objetivo	aprobado (binaria), nota_final (continua)
Metodología

## Análisis exploratorio (EDA):

Distribuciones, correlaciones y detección de outliers.

Evaluación de la relación entre hábitos y rendimiento.

## Preprocesamiento:

Imputación de valores nulos (mediana/moda).

Codificación de variables categóricas con OneHotEncoder.

Estandarización de variables numéricas.

### Modelado predictivo:

Clasificación: Logistic Regression y Random Forest Classifier.

Regresión: Linear Regression y Random Forest Regressor.

División de datos 80/20 y validación con métricas de rendimiento.

Evaluación y validación:

Clasificación → Accuracy, F1, ROC-AUC.

Regresión → MAE, RMSE, R².

Análisis de residuos y comparación entre modelos.

### Resultados Principales
Modelo de Clasificación (Aprobado/No Aprobado)

Accuracy: 0.85 – 0.90

F1-score: 0.84

ROC-AUC: 0.90

Variables más influyentes: nota_anterior, tasa_asistencia, horas_estudio_semanal, tiene_tutor.

Modelo de Regresión (Nota Final)

R²: 0.82 – 0.88

MAE: 0.35 – 0.45

RMSE: 0.50

Variables más influyentes: nota_anterior, tasa_asistencia, horas_sueno.

## Conclusiones

El rendimiento académico se explica principalmente por el esfuerzo previo, la asistencia y los hábitos de estudio.

La variable nota_anterior es el predictor más consistente en ambos modelos.

Los modelos de tipo Random Forest ofrecieron un mejor equilibrio entre precisión y estabilidad.

El sistema puede emplearse para identificar alumnos en riesgo y anticipar medidas de refuerzo.


Antonio Romero
Continuous Improvement & VoC Senior Lead
Responsible for data analysis, model development, and documentation.
