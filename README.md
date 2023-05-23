# Robot Trading en Python
#aluralatam #aluraChallengeRobotTrading
## El proyecto permite tomar decisiones de compra y venta de Bitcoin en tiempo real.

### Proyecto paso a paso:

- Configuración del ambiente: Se utilizó el entorno virtual de Google Colaboratory, como editor Python. Importó algunas librerías de Python que son esenciales para este proyecto, como Pandas, Numpy, Matplotlib, etc.

- Obtención de datos: Se accedió a una API que proporciono datos históricos de precios de Bitcoin en formato JSON. Realizar Web Scraping en un site de noticias para obtener el precio actual y algunos indicadores de tendencias del Bitcoin.

- Limpieza de datos: Los datos históricos se cargaron en un DataFrame de Pandas para poder manipularlos y analizarlos, se identificó y eliminó los outliers, además de tratar cualquier valor nulo o duplicados en la base. Finalmente, con la base limpia, calcula el precio promedio del Bitcoin.

- Tomar decisiones: Una vez obtenido el precio promedio, se comparó con el precio actual y tendencia del Bitcoin, que previamente se obtuvo con Web Scraping. Si el precio actual es mayor/igual que la media y la tendencia es de baja, entonces se debe vender, pero si el precio actual es menor que la media y la tendencia es de alta, entonces se debe comprar.

- Visualización: Utilizó la librería Matplotlib para crear un gráfico donde se muestre la evolución del precio del Bitcoin durante el periodo seleccionado, y una línea recta que pase sobre el precio medio. Por último, muestra un mensaje en el gráfico que indique “Vender”, “Comprar” o “” según sea la decisión del algoritmo.

- Automatización: Finalmente se automatizó el proceso. Utilizó la librería de Python "time" para ejecutar el algoritmo de decisión cada 5 minutos y actualizar el gráfico.

![Badge Challenge Robot Trading](https://github.com/siladev/robot-trading-python/blob/main/Badge-Challenge-Robot-Trading.png)
