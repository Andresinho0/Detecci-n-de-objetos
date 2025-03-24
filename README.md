   Detección de objetos
Programa que por medio de fotos detecta la cantidad de objetos

Librerías utilizadas:
  cv2
  matplotlib
  numpy

Este programa está dirigido a los almacenes que cuentan con cantidades grandes de cajas u objetos de formas similares.

Tiene como objetivo ahorrar tiempo al hacer el conteo de un inventario

Funcionamiento:

Este programa funciona aplicando tres filtros dados por la librería cv2. Como primer filtro se convierte la imagen a una escala de grises para reducir la complejidad visual de la imagen para los siguientes filtros. Para el segundo filtro se utiliza la función Sobel para calcular el gradiante de la imagen en los ejes X y Y, esto para encontrar los bordes resaltados de cada objeto de la imagen buscando transiciones de color o intensidad. Para finalizar, se utiliza el filtro Canny, el cual detecta los bordes obtenidos con la función Sobel y se usa un umbral para decidir cuales son los bordes significantes y cuales no. 
