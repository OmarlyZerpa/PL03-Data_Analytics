<h1 align='center'>
 <b>PROYECTO INDIVIDUAL Nº3</b>
</h1>

<p align='center'>
<img src = 'https://thumbs.dreamstime.com/b/mooc-massive-open-online-course-learning-vector-219370657.jpg' height = 200>
<p>

Los MOOCs (cursos masivos abiertos y online, por sus siglas en inglés) han revolucionado el mundo de la educación . El aumento de la popularidad de los MOOCs, no solo han aparecido nuevas plataformas privadas , sino que también muchas universidades y organizaciones sin fines de lucro han sumado a la oferta haciendo el mercado mucho más competitivo. En este contexto, resulta imperante para cada plataforma, ajustar sus modelos de negocio, los cursos y el contenido que se ofrece en los mismos para lograr captar y retener a la mayor cantidad de clientes.

### Desarrollo del proyecto

Una startup de tecnología está interesada en sumarse al mercado de cursos online, pero de una manera eficiente, por lo que compró datasets de las plataformas EDX, UDEMY Y COURSERA (los cuales se encuentran en el siguiente link https://drive.google.com/drive/folders/1TS76ok6giW7D_l5vc-zu5-cBU_dH3P5H), para analizar y sacar conclusiones de los datos recolectados.

Para ello se procedio con el **Analisis Exploratorio de datos** en un notebook (.ipynb), se importaron la librerias necesarias para la lectura de los dataset. Entre la transformaciones realizadas se tienen la eliminacion de valores duplicados, remplazo de valores nulos o vacios,  se realizaro graficas con el fin de visualizar los valores unicos de los dataset, ademas, se cambio de tipo de formato de algumas columnas como tambien se renombraron algunas de ellas.

Ahora teniendo en cuenta estos datos y analisis exploratorio se tomaron alguna decisiones:

* En el caso del dataset de coursera no se tomaron en cuenta los reviews dado a que existen, ademas de valores nulos, los comentarion son caracteres especiales o en el string ademas de texto tambien hay caracteres especiales, y algunos reseñas presentan emojis.
* Los url no seran relevantes para el analisis los extraigo, como muchas otras columnas.
* Para el analisis se solicita segmentar los niveles de ventas según precio, idioma, nivel y rating de cada curso para analizar qué tanto influyen dichas variables en la demanda del producto vendido. En algunos dataset no cuentan con esta informacion, por ejemplo el dataset de plataforma Coursera, a pesar que no tiene los datos requeridos, se decidio trabajarla solo con el rating, para Udemy como no tenemos rating, ni idioma, se trabajo con miembros y conferencias. En el caso de la plataforma edx, se observo que los cursos son FREE pero el certificado tiene un costo, se tomara este como precio de los cursos online.

Para mayor compresion revisar el archivo notebook jupyter "eda.ipynb".

Por otra parte se utilizo la libreria de **WordCloud** para extraer las palabras clave se repiten dentro del título del curso, de esta manera observar que rama tiene mayor demada.

Por último, se presenta en un archivo de POWER BI ''Dashboard.pbix''  las funcionalidades del **dashboard**, ademas de algunas implementaciones de **KPI's**, de esta manera y con el analisis previo exponer las **conclusiones y recomendaciones**.
