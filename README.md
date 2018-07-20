# PROYECTO-FINAL-VOT
# Seguimiento de Objetos usando Convolucionales(CNN) en Drones

> Este proyecto consiste en hacer un seguimiento de objetos usando MDNet(CNN) en videos grabados por Drones para el trabajo final del curso Tópicos en Inteligencia Artificial-UNSA


## Integrantes
* **Oliver Sumari Huayta**
* **Juan López Condori**
* **Eyner Pariguana Medina**


## Introducción

> Para este trabajo hemos probado distintos algoritmos puestos en el repositorio, seleccionando de esto uno basado en deep learning, en particular las redes neuronales convolucionales ya que en los ultimos tiempos las CNNs son las que mejores resultados esta obteniendo. El algoritmo MDNet(Multi-Domain Network) es el que mejores resultados ah obtenido haciendo seguimiento de objetos. Este algoritmo fue presentado en el VOT CHALLENGE 2015 y fue el ganador, siendo de los mejores aportes en la actualidad.

> Con el fin de obtener experiencia práctica con la implementación de redes neuronales, decidimos implementar este algoritmo pero con videos grabados por Drones, añadiendo a este un modelo de movimiento para optimzar su seguimiento . Para este proyecto hemos usado Matlab, OpenCV.

## Data

> La Data usada es una propuesta por un Benchmark, que son 70 videos grabados por drones con distintos escenarios y objetos como animales, personas y carros. Cada video esta dividido en frames y cada carpeta de video contiene un .txt donde se encuentra las coordenas del Bounding Box. Esto nos sirve para analisar la robustez del algoritmo, comparando la prediccion con el verdadero.

> La Data se encuentra en el siguiente [link](https://www.dropbox.com/s/s1fj99s2six4lrs/DTB70.tar.gz?dl=0)

## Arquitectura Utilizada


> La arquitectura utilizada es la que se encuentra en mdnet.png en este repositorio.

> MDNet brinda bounding box aleatorios en todo el frame para distintos dominios, se etiqueta a bounding box como negativos y positivos, eliminado los negativos y el dominio minorizando hasta ser el más sercano al objeto.

> El procedimiento visual del aprendizaje que hace esta en iteranciones.png.


## Implementado con
* [Matlab]
* [OpenCV](http://opencv.org/) 


## Aplicaciones 

  * En video vigilancia.
  * Para el control de trafico inteligente.
  * Reconocer accidentes de autos.
  * Seguimiento de infractores, delicuentes, etc.

## Referencia:
Paper: https://arxiv.org/abs/1510.07945

