# Machine Learning en Bioinformática

> Máster en Bioinformática Aplicada a Medicina Personalizada y Salud (Curso 2022-2023)

## Proyecto de Machine Learning

Objectivos principales y pasos a seguir:

1- Búsqueda de un conjunto de datos relacionados con la bioinformática/biomedicina/medicina.

- Buscador de conjuntos de datos [Google Dataset Search](https://datasetsearch.research.google.com/).
- Herramientas para buscar conjuntos de datos como [Kaagle](https://www.kaggle.com/datasets).
- Iniciativa de datos abiertos del [Gobierno de España](https://datos.gob.es/es).
- Repositorio [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets.php).

2- Identificación de la/s tarea/s de Machine Learning a abordar (regresión o clasificación) con el conjunto de datos seleccionado.

**HITO-1**: Envío de un correo a los profesores para especificar muy brevemente el dataset seleccionado (URL) y el tipo de problema que se pretende abordar. Debe enviarse como muy tarde el jueves **9 de marzo**. Los correos deben dirigirse a: alnogueira@uvigo.es, hlfernandez@uvigo.es y dgpena@uvigo.es.

3- Análisis exploratorio de los datos para observar si es necesario:

- Reducción del conjunto de datos, por ejemplo, eliminando columnas innecesarias.
- Identificación de datos adicionales.
- Transformación o descomposición de datos.
- Estudio de correlaciones entre variables.

**HITO-2**: Presentación en la clase del día **15 de marzo** explicando el conjunto de datos seleccionado con el problema a abordar, así como un pequeño estudio de los atributos de ese conjunto de datos. Cada grupo tendrá como **máximo 8 minutos**.

4- Preparación de los datos, por ejemplo, entre otras muchas técnicas:

- Limpieza de datos (*outliers* o *missing values*, etc).
- Integración de datos, en el caso de tener que unir diferentes base de datos para la creación del conjunto de datos.
- Balanceo de datos.
- Selección de características.
- Discretización de variables continuas.
  
5- Elección del(os) modelo(s) de aprendizaje. Investigar cuál es el modelo más apropiado para el problema planteado, teniendo en cuenta parámetros como *(i)* tiempos de procesamiento para su ejecución en tiempo real o no, *(ii)*  rendimiento predictivo del modelo, *(iii)* requisitos de memoria durante el entrenamiento, etc. También es posible seleccionar varios modelos o algoritmos para hacer comparativas tanto en métricas de rendimiento como en tiempos de ejecución, incluso, teniendo como referencia una publicación existente.

6- Entrenamiento y validación del(os) modelo(s). Consiste en dividir el conjunto de datos, asegurándose de que los datos de entrenamiento, validación y test no se mezclen entre las particiones, para llevar a cabo el entrenamiento del(os) modelo(s) y obtener las métricas de validación. Dependiendo del volumen de datos, quizás hay que emplear una validación cruzada de los datos.

7- Interpretación de los resultados y ajustar o modificar el modelo de aprendizaje. Hay que asegurarse de que el modelo ha aprendido algún patrón teniendo en cuenta los datos de entrada y que es capaz de generalizar, es decir, que no se produzca *overfitting*. Si esto sucediera, se debe analizar el problema y plantear una posible solución.

**HITO-3**: Presentación en la clase del día **17 de marzo** de los resultados obtenidos, explicando brevemente el trabajo realizado para la consecución de los mismos, incluyendo problemas detectados y estrategias empleadas. Cada grupo tendrá **máximo 15 minutos**.

### **Composición de grupos de trabajo**

Los grupos estarán formados por 3 o 4 personas.

### **Exposiciones de trabajo**

Los requisitos a tener en cuenta durante las exposiciones son:

- Ajustarse al tiempo disponible. En caso de exceder la duración, se podrá detener la presentación.
- Elaborar diapositivas que apoyen el discurso para facilitar la comprensión del problema planteado.
- No es necesario que expongan todos los miembros del grupo, pero no puede repetir la presentación la misma persona, es decir, si un miembro ya ha realizado la primera presentación, no podrá realizar la segunda.
- Pueden efectuarse preguntas a la finalización de cada exposición.

### **Rúbrica de evaluación**

| **Ítem**                                    | **Descripción**                                                                                                                                                                            | **Valoración** |
| ------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------- |
| Presentación del trabajo                    | Realización de las dos exposiciones. En la presentación final se deberá exponer el trabajo realizado y justificar la dedicación grupal al mismo (aproximadamente 5h).                      | 5 puntos       |
| Trabajo original                            | En caso de partir de código existente (de Kaggle, del notebook de prácticas, etc.) se debe aclarar cuáles han sido las contribuciones originales o adaptaciones realizadas por el grupo.   | 1 punto        |
| Justificación de las decisiones             | Explicación razonada de los motivos que llevaron a tomar ciertas decisiones (p. ej.: no tener en cuenta algunas columnas o *features*, la conversión de los valores de una columna, etc.). | 1 punto        |
| Interpretación de los resultados            | Ser capaces de transmitir e interpretar los resultados obtenidos (sean estos buenos o malos).                                                                                              | 1 punto        |
| Identificación de trabajo futuro            | Exposición de posibles vías de trabajo futuras (p. ej.: tareas interesantes que no dio tiempo a hacer, etc.).                                                                              | 1 punto        |
| Debate con los profesores y/o compañeros/as | Ser capaces de participar en un debate o de generar preguntas acerca del proyecto desarrollado.                                                                                            | 1 punto        |
