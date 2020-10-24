## Comentario: Deep Learning based Recommender System: A Survey and New Perspectives

Esta sección del paper habla sobre redes recurrentes, redes diseñadas para tratar con datos secuenciales. Por ejemplo, se puede utilizar RNNs para realizar predicciones basadas en los datos de la sesión de usuarios no registrados o para recomendaciones con usuarios identificados. Luego se describieron RBM, utilizadas para filtrado colaborativo. Después se comentó sobre modelos basados en atención, los que permiten filtrar inputs poco relevantes y enfocarse en los realmente importantes para la predicción. Se habló sobre distintos modelos basados en aprendizaje profundo, como _deep reinforcement learning_, _adversarial network_ y modelos híbridos. Finalmente se trataron problemas abiertos en el área y posibles investigaciones futuras.

Las redes recurrentes son un aporte muy significativo para el área de sistemas recomendadores, ya que las recomendaciones siempre siguen un orden temporal: se utiliza datos con los que el usuario interactuó en el pasado para recomendar ítems con los que podría interactuar en el futuro. Este orden secuencial también está presente en los datos, ya que los usuarios naturalmente interactúan con los ítems con un orden temporal. 

Las redes RNN también permiten aprender sobre cambios en los gustos de los usuarios, permitiendo mejores recomendaciones al adaptarse mejor a lo que el usuario le gusta recientemente. Relacionado a esto, y de manera anecdótica, es posible notar que YouTube tiene un fuerte _bias_ a favor de los videos consumidos recientemente. Tipos de videos o canales consumidos hace tiempo son rara vez recomendados. Cabe preguntar si esto es realmente lo más efectivo, o una mezcla entre reciente y antiguo podría generar mejores resultados.

El uso de los datos de una sesión de usuarios no registrados es interesante, y ayudaría al problema de la _sparsity_ en los datos.

Es muy interesante la idea de generar _reviews_ que acompañen la calificación predicha. Esto podría permitir recomendaciones aún más personalizadas y un mayor nivel de control para el usuario. Esto podría ser útil para el problema de que las recomendaciones de modelos de aprendizaje profundo son difíciles de explicar, especialmente cuando no se utilice atención.

Un problema de RBM es que la codificación binaria hace que se pierda información para mostrar al usuario y para comparar ítems. Es más fácil encontrar las mejores recomendaciones cuando los ratings predichos pueden ser decimales, que cuando deben tomar un valor entero.

En conclusión, en esta segunda parte del paper se describió modelos de RNN, de atención e híbridos. También se explicaron distintos problemas y desafíos en el área. Se postularon varias ideas interesantes, y es fácil ver que esta área es el camino para mejores recomendaciones.



