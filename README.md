# Análisis de Videos en Tendencia en YouTube

## Objetivo del Proyecto
El objetivo de este proyecto es analizar los datos de videos en tendencia en YouTube para extraer información relevante y realizar predicciones sobre el comportamiento futuro de los videos en tendencia.

## Participantes
- Alumno 1: Salvador Díaz Aguirre
- Alumno 2: Diego Antonio Salinas Casaico
- Alumno 3: Ricardo Rafael Rivas Carrillo

## Descripción del Conjunto de Datos
El conjunto de datos utilizado en este proyecto incluye información sobre videos en tendencia en YouTube. Los datos incluyen variables como el número de vistas, me gusta, no me gusta, comentarios, la fecha en que el video se volvió tendencia, y la categoría del video, entre otros. 

Los datos han sido limpiados y se han eliminado los valores atípicos para asegurar la precisión del análisis. El conjunto de datos proviene de Kaggle y puede ser consultado en el archivo PDF adjunto y en el siguiente cuadro.

| Variable              | Descripción                                                                                                                                         |
|-----------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
| video_id              | El identificador único del video en YouTube. Es una cadena de caracteres que permite diferenciar cada video en la plataforma.                        |
| trending_date         | La fecha en la que el video comenzó a ser tendencia, almacenado en formato de fecha (YY.DD.MM).                                                      |
| title                 | El título del vídeo. Es un texto descriptivo que el creador del contenido asigna al video.                                                           |
| channel_title         | El nombre del canal que subió el video. Es el nombre del creador o de la entidad que posee el canal.                                                 |
| category_id           | Un identificador numérico que representa la categoría a la que pertenece el video. Cada categoría tiene un ID específico asignado por YouTube.      |
| publish_time          | La fecha y hora exacta en la que el video fue publicado en YouTube. Almacenado en formato de fecha y hora (YYYY-MM-DDTHH:MM).                        |
| tags                  | Las etiquetas asociadas al video. Son palabras clave o frases que describen el contenido del video y ayudan en la búsqueda y descubrimiento del mismo.|
| views                 | El número total de visualizaciones que ha tenido el video.                                                                                           |
| likes                 | El número total de "me gusta" que ha recibido el video.                                                                                              |
| dislikes              | El número total de "no me gusta" que ha recibido el video.                                                                                           |
| comment_count         | El número total de comentarios que se han dejado en el video.                                                                                        |
| thumbnail_link        | El enlace a la imagen en miniatura del video. Es la imagen que se muestra como previsualización del video en YouTube.                                |
| comments_disabled     | Un indicador booleano que señala si los comentarios están deshabilitados para el video. Puede ser True (verdadero) si los comentarios están deshabilitados, o False (falso) si están habilitados.|
| ratings_disabled      | Un indicador booleano que señala si las calificaciones (likes y dislikes) están deshabilitadas para el video. Puede ser True (verdadero) si las calificaciones están deshabilitadas, o False (falso) si están habilitadas.|
| video_error_or_removed| Un indicador booleano que señala si el video ha sido eliminado o si tiene algún error que impide su reproducción. Puede ser True (verdadero) si el video ha sido eliminado o tiene un error, o False (falso) si el video está disponible.|
| description           | La descripción del video. Es un texto proporcionado por el creador del contenido que ofrece información adicional sobre el video, enlaces, y otros detalles relevantes.|
| state                 | Nombre del Estado perteneciente al país (incorporado de forma aleatoria)                                                                             |
| lan                   | Latitud geográfica de ubicación del Estado.                                                                                                          |
| lon                   | Longitud geográfica de ubicación del Estado.                                                                                                         |
| geometry              | Registra las coordenadas de las geometrías donde se ubica el Estado dentro del planeta.                                                              |


## Conclusiones
 - El número de me gusta en un video está más relacionado a cuán corto es este.
 - Hay categorías que tienen más visitas y son más propensas a estar en tendencia.
 - En una empresa como lo sería YouTube, es crucial una correcta visualización de datos para identificar las relaciones entre datos y en qué enfocarse
 - Base a los datos encontrados la categoría con más proporción de aceptación y popularidad es la de Comedia
 - Se muestra además que la categoría de videos con más interacción de los usuarios es la de Música
 - Hay que recalcar cómo la categoría de comedia es la cual es la más equilibrada dentro de ser una fuente de visitas, likes y comentarios.
 - Podemos notar que hay estados que visualizan más los videos pero sin dejar tantos “me gusta” o “no me gusta”, mientras que hay estados que si dejan estas reacciones más seguido. Por lo que los estados que realizan más estás reacciones cambian mucho.
 - Tras experimentar con los datos, podemos concluir que en este caso un modelo de regresión lineal no es factible para predecir los “me gusta”, “no me gusta”, ni las “vistas”, puede que debido a que hay mucha variación entre estos datos por lo que no es muy preciso. 

## Licencia
Este proyecto se distribuye mediante la licencia [Atribución-NoComercial-CompartirIgual 4.0 Internacional (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.es)
