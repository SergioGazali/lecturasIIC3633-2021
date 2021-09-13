## Content-Based Recommendation Systems

El paper explica un panorama general de los sistemas de recomendación basados en contenido. Se hace un repaso sobre distintos métodos que, sin ser exclusivos al área estudiada, permiten modelar al usuario para, en base a las descripciones de los items, determinar recomendaciones.

En la sección sobre métodos "nearest neighbor", se comenta el ejemplo de un sitio de noticias, donde junto con el titular se indica la similaridad del artículo a elementos previamente leídos por el usuario, y el nivel de popularidad del artículo. Esto me hace darme cuenta de un fenómeno particular que puede darse en ciertas aplicaciones, por ejemplo sitios de noticias: la relevancia de un ítem podría estar definida por factores externos y totalmente independientes a la historia del usuario. Esto va un paso más allá de la noción básica de relevancia que podría tenerse, ya que por más que tengamos un modelo de lo que al usuario debiera gustarle, una noticia de alto impacto, incluso si no es de un tema usualmente preferido, puede ser una recomendación muy relevante.

Me parece muy interesante la observación que se hace hacia el final del paper, al aclarar que ningún sistema basado en contenido logrará buenos resultados si el contenido en cuestión no permite informar el modelo del usuario o las características de los ítems. Lo destaco porque al aprender estos sistemas se puede perder la perspectiva de que se deben cumplir condiciones que van más allá de las ecuaciones para que se generen recomendaciones valiosas. Es muy importante estar muy consciente de la aplicación y contexto en que se desarrolla, para determinar si el contenido disponible efectivamente permitirá modelar preferencias o no. 

En línea con lo anterior, destaco las posibilidades de combinar métodos basados en contenidos con otros sistemas, lo que puede ayudar a solucionar problemas como el mencionado en el párrafo previo. Por ejemplo, usar reglas basadas en contenido para depurar resultados obtenidos con métodos de filtrado colaborativo. Combinacione como esta pueden generar mejores resultados para ciertas aplicaciones.

Por último, relacionando lo leído con las clases de la semana pasada, el paper me permitió reflexionar sobre cómo generar efectivamente valor para las personas. En las clases, se comentó cómo existen métricas utilizadas en la academia, en la industria, y por último métricas que intentan capturar la utilidad real para el usuario; estas últimas son las más complejas. Se comenta en el paper cómo el feedback implícito viene acompañado con altos niveles de incertidumbre ya que no es fácil distinguir qué señales efectivamente revelan interés del usuario. Creo que las personas perciben esto, y en mi experiencia y en la de otros, a veces el usuario se ve a sí mismo haciendo acciones forzosas sólo para tratar de inducir al recomendador a que no recomiende algo o que sí lo haga. Con esto en cuenta, me interesaría saber si se puede aumentar la satisfacción de los usuarios y su comodidad de uso, al incluir interfaces en las aplicaciones, que permitan regular al sistema mediante parámetros controlables por el usuario (en una interfaz que simplifique los conceptos para el usuario común). Un ejemplo podría ser una barra en que se indique cuánto feedback implícito queremos que el sistema considere.