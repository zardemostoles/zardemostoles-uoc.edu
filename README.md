<div style="width: 100%; clear: both;">
<div style="float: left; width: 50%;">
<img src="http://www.uoc.edu/portal/_resources/common/imatges/marca_UOC/UOC_Masterbrand.jpg", align="left">
</div>
</div>
<div style="float: right; width: 50%;">
<p style="margin: 0; padding-top: 22px; text-align:right;">22.536 - Trabajo de Fin de Grado</p>
<p style="margin: 0; text-align:right;">Grado en Ciencia de Datos Aplicada</p>
<p style="margin: 0; text-align:right; padding-button: 100px;">Estudios Informática, Multimedia y Telecomunicación</p>
</div>
</div>
<div style="width: 100%; clear: both;">
<div style="width:100%;">&nbsp;</div>

### Trabajo de Fin de Grado de Antonio Carlos Rodríguez Bajo

### Diagnóstico automático de casos de riesgo de melanoma basado en imágenes dermatoscópicas
  
El melanoma es un cáncer de la piel que puede ser letal si no es tratado convenientemente. La supervivencia de los pacientes depende en gran medida de una atención temprana por parte de profesionales médicos. 
  
 El objetivo principal de este Trabajo es demostrar el uso aplicado de la Ciencia de Datos y de la Inteligencia Artificial para crear un sistema de apoyo capaz de emitir una predicción de riesgo de melanoma a partir de imágenes dermatoscópicas. Siguiendo una planificación del Trabajo por etapas, se ha realizado las siguientes fases: 
1. Estudio del arte sobre el tratamiento de imágenes mediante redes neuronales convolucionales, seleccionando EfficientNet. 
2. Análisis de los conjuntos de datos abiertos de imágenes ISIC, seleccionando los datos del desafío del año 2019. 
3. Experimentación y entrenamiento de modelos en Google Cloud para obtener el modelo óptimo. 
4. Evaluación de las métricas de rendimiento y equidad. 
5. Implementación del modelo en la nube de AWS, acompañado de una aplicación web para realizar diagnósticos sobre nuevas imágenes. 
  
Los resultados de la implementación se consideran satisfactorios, con la recomendación de su uso en pacientes adultos, tanto mujeres como hombres, mayores de 30 años, con tonos de piel clara o ligeramente morena. Mejoras en el sistema derivadas del incremento de la calidad de los datos, el aseguramiento de su interpretabilidad en un contexto clínico y la implementación de una práctica de MLOps para gestionar nuevas versiones podrían llevar a una implantación en un entorno real en producción al servicio de la comunidad médica.
  
El orden de ejecución y el propósito de cada elemento del respositorio es el siguiente:

| Orden | Elemento                             | Descripción                                                                     |
|-------|--------------------------------------|---------------------------------------------------------------------------------|  
|    1  | TFG_Comun.py                         | Variables comunes del proyecto.                                                 |
|    2  | TFG_Calculo_Tipo_Tono_Piel_ITA.ipynb | Cálculo aproximado del fototipo.                                                |
|    3  | TFG_EDA.ipynb                        | Análisis exploratorio de datos.                                                 |
|    4  | TFG_Modelo_Diagnostico.ipynb         | Experimentos y creación del modelo de diagnóstico óptimo.                       |
|    5  | TFG_Evaluacion.ipynb                 | Evaluación del rendimiento y equidad del modelo.                                |
|    6  | TFG_Crear_Modelo_AWS.ipynb           | Preparación del modelo en formato apropiado para AWS.                           |
|    7  | TFG_Despliegue_Modelo_AWS.ipynb      | Despliegue del modelo en AWS con su correspondiente punto de enlace.            |
|    8  | inference.py                         | Programa para convertir imágenes a tensores utilizado por el modelo desplegado. |
|    9  | requirements.txt                     | Módulos que necesita instalar el modelo desplegado en AWS.                      |
|   10  | TFG_Aplicacion_Web.tar.gz            | Aplicación web de diagnóstico.                                                  |
