# Tarea de Programación 4

La tarea de programación consiste de varias diferentes funciones que resuelven partes independientes de la tarea. 
El resumen de los contenidos de este repositorio se encuentra a continuación. 

## Contenidos del Repositorio GIT

Esta tarea consiste de lo siguiente: 
	1) Un archivo .ipynb utilizado para programar en el entorno Jupyter. 
	2) Un archivo .py que contiene el código en formato de Python. 
	3) El archivo .csv que contiene los datos dados en el enunciado. 
	4) Las imagenes correspondientes a la solución de la tarea. 

### Punto 1

Primero se realiza una lectura del archivo .csv utilizando la herramienta de Numpy. 
Aplicando la función explicada en la discusión de clase para crear una señal sinusoidal normalizada (con amplitud unitaria), se logra obtener el conjunto de datos correspondiente a una señal sinusoidal para un dato particular. 
Utilizando un for loop la señal se logra modular para todos los datos correspondientes. 
Esto produce un arreglo de amplitudes que corresponden a las señales normalizadas y concatenadas, sin ruido. 

### Punto 2

En esta parte se utiliza la definición de "sum squared magnitude" para calcular la potencia promedio de la señal modulada. 
La potencia de una señal se define como la suma de todos las magnitudes discretas que componen la señal, al cuadrado. 
Por lo tanto, se aplica esta función para todo el arreglo de datos encontrado en el punto 1.

### Punto 3

La simulación de un canal de ruido blanco requiere limitar la función random de Numpy a la relación señal a ruido (SNR) correspondiente. 
Por lo tanto, se utiliza un for loop para realizar los cálculos correspondiente a todos los valores de SNR. 

### Punto 4

Las gráficas correspondiente a todos los puntos se realizaron por separado, para prevenir errores en donde se sobre-escriben todas las gráficas en el mismo archivo. 
Por lo tanto, cada gráfica empieza con un plt.figure(), el cual forma una nueva figura utilizando matplotlib, y aplica welch y semiogy de la biblioteca de scipy.signal. 
Mientras la densidad espectral de potencia del 

![Alt text](relative/path/to/DSPsinruido.png?raw=true "THIS IS AN IMAGE")


## Construido con

* [Jupyter](https://jupyter.org/) - GUI utilizado

## Autores

* **Laura Rojas** - [lrojasz](https://github.com/lrojasz)

## Reconocimientos

* Se utilizaron bibliotecas de numpy y scipy para manipulación de datos y archivos.
* Se utilizó la biblioteca de matplotlib para realizar las gráficas.
* Se utilizó código trabajado en la clase de discusión sobre la Tarea 4 para la resolución de la tarea. Además, se utilizó código encontrado en el archivo py8.ipynb del GIT para la resolucion del trabajo. El autor original de los códigos correspondientes es al profesor, Fabian Abarca Calderón. 

