<div style="width: 100%; display: flex; align-items: flex-start; justify-content: space-between;">
  <div style="width: 50%;">
    <img src="https://static.wikia.nocookie.net/logopedia/images/2/2d/UPC-Logo-Actual.png/revision/latest?cb=20230305155749&path-prefix=es" style="width: 300px; height: auto;">
  </div>
  <div style="width: 50%; text-align: left;">
    <p style="margin: 0; padding-top: 22px;">1ACC0216-2510-256 - Fundamentos de Data Science · TB2</p>
    <p style="margin: 0;">2025 · Ciencia de la Computación</p>
    <p style="margin: 0;">Profesora: <b>Nérida Isabel Manrique Tunque</b></p>
    <p style="margin: 0;"><b>Alumnos:</b></p>
    <p style="margin: 0;"><b>Carlin Mendoza, Selinne Sandra</b> - <a href="mailto:U20251d325@upc.edu.pe">U20251d325@upc.edu.pe</a></p>
    <p style="margin: 0;"><b>Pacherres Muñoz, Peter Smith</b> - <a href="mailto:U202423854@upc.edu.pe">U202423854@upc.edu.pe</a></p>
    <p style="margin: 0;"><b>Timana Mendoza, Sebastian</b> - <a href="mailto:U202218729@upc.edu.pe">U202218729@upc.edu.pe</a></p>
  </div>
</div>

---
# CREACION DE CONOCIMIENTO APLICANDO LA METODOLOGÍA CRISP-DM: *Trending YouTube Video Statistics*

## Índice

1. [Objetivo del proyecto](#objetivo-del-proyecto)  
2. [Descripción del dataset](#descripción-del-dataset)  
   - 2.1 [Variables categóricas](#variables-categóricas)  
   - 2.2 [Variables numéricas](#variables-numéricas)  
   - 2.3 [Variables de fecha y tiempo](#variables-de-fecha)
   - 2.4 [Variable geoespacial](#variables-geoespacial)
3. [Conclusiones](#conclusiones-clave)  
4. [Licencia](#licencia)

---

## 1. Objetivo del proyecto <a name="objetivo-del-proyecto"></a>

Este proyecto de Ciencia de Datos tiene como objetivo analizar las tendencias de videos de YouTube en **India**, con el fin de responder preguntas clave del negocio relacionadas con el rendimiento de contenido en la plataforma. Utilizando la metodología **CRISP-DM**, se busca desarrollar una propuesta analítica que permita:

- Generar conocimiento y valor a partir de los datos disponibles.
- Tomar decisiones fundamentadas mediante el análisis de métricas clave como vistas, likes y dislikes.
- Identificar patrones de comportamiento por categorías, canales y ubicación geográfica.
- Evaluar la posibilidad de construir modelos predictivos que anticipen el desempeño de los videos.

La metodología CRISP-DM facilita la comunicación constante entre los miembros del equipo durante todas las fases del proyecto, lo cual permite adaptarse a los cambios en los requisitos del negocio y en el diseño analítico. El análisis está alineado con una necesidad real de una empresa de marketing digital interesada en entender cómo varían las tendencias de YouTube en distintos países, en este caso **India**, con el objetivo de tomar decisiones estratégicas basadas en datos.

---

## 2. Descripción del dataset <a name="descripción-del-dataset"></a>

Este conjunto de datos contiene información detallada sobre videos en tendencia de YouTube en India. Las variables se pueden clasificar en tres grandes grupos: categóricas, numéricas y geoespaciales.

### 2.1 Variables categóricas <a name="variables-categóricas"></a>

Estas variables representan atributos descriptivos de los videos y el canal que los publica:

- **video_id**: Identificador único del video en YouTube.  
- **title**: Título del video.  
- **channel_title**: Nombre del canal que publicó el video.  
- **category_id**: Código numérico que representa la categoría del video (requiere referencia externa en formato JSON).  
- **tags**: Lista de etiquetas asociadas al video.  
- **comments_disabled**: Indica si los comentarios están deshabilitados (`TRUE` / `FALSE`).  
- **ratings_disabled**: Indica si las calificaciones están deshabilitadas (`TRUE` / `FALSE`).  
- **video_error_or_removed**: Indica si el video presenta errores o fue eliminado.  
- **description**: Descripción textual del contenido del video.  
- **state**: Estado geográfico de India asignado al video (dato generado aleatoriamente).  

### 2.2 Variables numéricas <a name="variables-numéricas"></a>

Estas variables cuantifican la popularidad y la interacción de los usuarios con el contenido:

- **views**: Número de visualizaciones del video.  
- **likes**: Número de "me gusta" recibidos.  
- **dislikes**: Número de "no me gusta" recibidos.  
- **comment_count**: Número de comentarios publicados.  
- **lat**: Latitud del estado geográfico.  
- **lon**: Longitud del estado geográfico.  

### 2.3 Variables de fecha y tiempo <a name="variables-de-fecha"></a>

Estas variables permiten realizar análisis temporales y de tendencias:

- **trending_date**: Fecha en que el video fue registrado como tendencia (formato `YY.DD.MM`).  
- **publish_time**: Fecha y hora de publicación original del video (formato ISO 8601).  

### 2.4 Variable geoespacial  <a name="variables-geoespacial"></a>

Esta variable permite representar y visualizar los datos sobre un mapa:

- **geometry**: Representación geométrica del estado

---

## 3. Conclusiones <a name="conclusiones-clave"></a>

Este proyecto de Ciencia de Datos logró analizar de manera efectiva los factores que determinan las tendencias de videos de YouTube en India, cumpliendo con todos los requerimientos establecidos por la consultora internacional para su cliente de marketing digital. Los principales hallazgos incluyen:

- **Categorías más frecuentes y visibles:** *Entertainment*, *News & Politics* y *Music* dominan las listas de tendencias, lo que indica una alta demanda de estos géneros en la región.
- **Preferencias del público:** Categorías como *Pets & Animals* y *Gaming* generan mayor proporción de "me gusta", mientras que *Nonprofits & Activism* y *News & Politics* presentan menor aceptación.
- **Aceptación del contenido:** *Pets & Animals* y *Education* tienen la mejor proporción de "me gusta" vs. "no me gusta", mientras que *News & Politics* evidencia un contenido polarizante.
- **Participación de la audiencia:** Categorías como *Sports* y *Travel & Events* muestran un consumo pasivo (muchas vistas pero pocos comentarios), lo que puede guiar decisiones entre alcance y engagement.
- **Variación temporal:** Las tendencias fluctúan mensualmente, sugiriendo que factores estacionales o eventos virales influyen en la visibilidad del contenido.
- **Concentración de canales:** Pocos canales, como *etvteluguindia*, concentran la mayoría de las apariciones en tendencia, recomendando enfocar colaboraciones en creadores ya consolidados.
- **Engagement geográfico:** La interacción varía significativamente por estado; por ejemplo, *Nagaland* destaca por su alto nivel de engagement, abriendo oportunidades para campañas localizadas.
- **Relación entre valoraciones y conversación:** Se encontró una fuerte correlación entre "me gusta" y comentarios, indicando que videos bien valorados también generan más participación.
- **Predicción del rendimiento:** Se construyó un modelo de regresión con Random Forest que predice con alta precisión vistas, likes y dislikes (R² > 0.99 en escala logarítmica), demostrando el potencial de aplicar analítica predictiva para anticipar el impacto de nuevos contenidos.

En resumen, el proyecto no solo respondió satisfactoriamente a los objetivos planteados, sino que también entregó herramientas analíticas y predictivas aplicables a decisiones estratégicas en el ámbito del marketing digital.

---

## 4. Licencia <a name="licencia"></a>

Este proyecto se encuentra bajo la Licencia MIT. Para más información, consulta el archivo [LICENSE](LICENSE).
