# Desafío técnico – segmentación pulmonar en imágenes de rayos X

## Descripción general

El objetivo de este desafío es implementar un algoritmo de **segmentación pulmonar** usando deep learning sobre imágenes de rayos X de tórax. Además, deberás elaborar una propuesta detallada sobre cómo abordarías el **fine-tuning de un modelo multimodal (vision-language model, VLM)** sobre este mismo dominio.

## Parte 1: segmentación pulmonar

### Objetivo

Entrenar un modelo de segmentación que identifique con precisión los pulmones en imágenes de rayos X de tórax.

### Dataset

Trabajarás con un dataset que incluye:

- Imágenes en formato `.jpg`.
- Una base de datos relacional con:
  - Identificadores de paciente y estudio.
  - Datos demográficos del paciente.
  - Información de modalidad según la nomenclatura **DICOM**.
  - Mediciones clínicas asociadas a cada imagen (índice cardiotorácico, distancias, ángulos).

### Tareas

#### 1. Segmentación pulmonar

- Implementa un modelo de segmentación pulmonar usando Deep Learning
- No se permite el uso de frameworks que funcionen como caja negra (por ejemplo, APIs que devuelven segmentaciones sin permitir entrenamiento manual).
- Deberás entrenar el modelo desde cero o realizar fine-tuning de un modelo segmentador abierto.

#### 3. Análisis demográfico y clínico

Explora y describe las características demográficas de los pacientes (edad, sexo, etc.) y cualquier otra variable clínica que consideres relevante y esté disponible en la base de datos.

## Parte 2: propuesta de fine-tuning de un VLM

Aunque no realizarás el fine-tuning real por limitaciones de tiempo y cómputo, deberás preparar una propuesta clara, razonada y técnica sobre cómo abordarías esta tarea.

### Objetivo

Describir un plan detallado para adaptar un vision-language model al dominio clínico utilizando el dataset **MIMIC-CXR**.

### Contenido esperado

Incluye en tu entrega una presentación (puede ser un PDF o cuaderno markdown) que contenga:

- ¿Qué tipo de modelo vision-language usarías y por qué?
- ¿Cómo prepararías los datos del MIMIC-CXR para entrenar dicho modelo?
- ¿Qué tarea elegirías (por ejemplo, generación de reporte, pregunta-respuesta, captioning, etc.)?
- ¿Qué secciones del reporte usarías como texto objetivo?
- ¿Qué estrategia de fine-tuning aplicarías (por ejemplo, full fine-tuning, LoRA, etc.)?
- ¿Qué métricas utilizarías para evaluar el modelo?
- ¿Cómo evaluarías si el modelo realmente aprende conceptos clínicos relevantes?

### Recurso

- MIMIC-CXR dataset – [https://physionet.org/content/mimic-cxr/2.0.0/](https://physionet.org/content/mimic-cxr/2.0.0/)

## Entregables

1. Código con el flujo completo de segmentación:

   - Carga y filtrado de imágenes.
   - Entrenamiento del modelo de segmentación.
   - Evaluación visual y cuantitativa de los resultados.
   - Análisis de datos demográficos y clínicos.
2. Una presentación con la propuesta de fine-tuning de un vision-language model para tareas clínicas con MIMIC-CXR.
