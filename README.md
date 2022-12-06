# Proyecto_de_Programacion_Equipo1
# **Secciones transversales y el uso de herramientas tecnológicas.**
**Prof: Sebastián Gonzalez**

**3•B**

**Programación II**
![](Aspose.Words.ef8416f3-5098-407f-9406-43c26dd12b9c.001.png)

Francisco Javier Aguilera Robles (1), Barbara García Carbajal (2) Jorge Ignacio García Gutiérrez (3)

(1) Facultad de Ingeniería Civil, Colima - Coquimatlán Kilómetro 9, Jardines del Llano, 28400 Coquimatlán, Col., [faguilera@ucol.mx (](mailto:faguilera@ucol.mx)2) [bgarcia42@ucol.mx (](mailto:bgarcia42@ucol.mx)3) <jgarcia73@ucol.mx>


**Resumen**
Se llevará acabo la digitalización de las secciones transversales de un lugar a definir haciendo uso del nivel fijo para conocer el comportamiento del terreno de manera longitudinal y transversal; además se apoyará el trabajo con Python para los cálculos previos a la realización del perfil y secciones. La visualización grafica del terreno tanto en CivilCAD como en Python. Además, la geolocalización más cercana al lugar del levantamiento usando QGIS. 

**Palabras clave**: nivel fijo, perfil, longitudinal, transversal, Python.

**Abstract**

The digitalization of the cross sections of a placeto be defined will be carried out using the fixed level to know the behavior of the terrain longitu- dinally and transversally; In addition, work with Python will be supported for calculations prior to making the profile and sections. The graphic visualization of the terrain both in CivilCAD and in Python. Also, the closest geolocation to the survey site using QGIS.

**Keywords:**

fixed	level,	profile,	longitudinal,	transverse, Python

**Introducción:**

Este proyecto se basa en obtener el nivel del canal que se localiza al costado derecho del laboratorio de topografía mediante método de secciones transversales y el uso del lenguaje de programación Python para llevar a cabo códigos que nos permita facilitar los cálculos al implementar librerías que nos ayuden a cumplir el propósito como lo son matplotlib, basemap entre otras, implementando así herramientas como el Qgis para hacer la representación en un shape de las coordenadas que imprime el código obteniendo así la ubicación del área de estudio mediante la geolocalización , con el fin de una futura expansión para mejorar la conducción de aguas pluviales y así conducirlas fuera de las instalaciones previniendo algún accidente o daño a la infraestructura de la facultad.

**Desarrollo y manejo de datos:**

El proyecto consistirá en determinar, el perfil y con ello las secciones transversales de un "canal" ubicado en las instalaciones de la Facultad de Ingeniería civil con la finalidad de realizar una ampliación; además de que permita recolectar la información necesaria para determinar y conocer el comportamiento del área de estudio, y así obtener la información necesaria para lograr los cálculos de los datos del terreno como lo son el desnivel, la tolerancia, y el error así obteniendo las cotas y la capacidad máxima de contención.

El levantamiento topográfico es el proceso de determinar la posición relativa de los elementos naturales y artificiales sobre o bajo la superficie de la tierra. El Congreso Americano de Topografía y Cartografía (ACSM) define la topografía como la ciencia y el arte de realizar todas las mediciones esenciales para determinar la posición relativa de puntos o detalles físicos y culturales arriba, sobre o debajo de la superficie de la Tierra, y para representarlos en forma utilizable, o para establecer la posición de los puntos o detalles. Hace cuatro mil años, los conceptos de matemáticas eran básicos, sin embargo, los egipcios fueron capaces de lograr maravillas. Utilizaron los predecesores de los instrumentos topográficos modernos para realizar muchas hazañas, desde canales hasta pirámides.

Para entrar un poco en tema, se deben conocer algunos conceptos claves para este proyecto. Secciones transversales: Las secciones transversales son líneas de niveles o perfiles cortos que se realizan de forma perpendicular al eje del proyecto. (A., 2021) proporcionan la información necesaria para la estimación de los volúmenes de movimientos de tierras. Existen dos tipos generales    de secciones transversales para proyectos de vías terrestres como carreteras y para bancos de materiales. Otro de los conceptos sería el de la n nivelación de perfil que es el proceso de determinación de una serie de elevaciones siguiendo una línea fija. El perfil es absolutamente necesario para el trazo de pendientes, carreteras, canales, drenajes, etc. Dicho   proceso es para fines de localización, diseño y construcción, donde es necesario determinar las elevaciones, a lo largo de las rutas propuestas de carreteras, canales, vías ferroviarias, líneas de conducción de agua, etc.

![Imagen3](https://user-images.githubusercontent.com/119510798/205818643-90c517aa-d9b3-4988-96e3-e74a6acd157d.jpg)

Ejemplo de secciones transversales.

Se estará utilizando el PyQgis para de alguna forma automatizar procesos, pero para comprender más, está lo siguiente. Se trata de una librería de Python que se utiliza para tratar datos geográficos. Esta librería es compatible con el conocido software QGIS. El saber escribir scripts nos da muchísima versatilidad a la hora de ejecutar los programas, ya que podemos automatizar todas esas tareas que tenemos que realizar varias veces de la misma forma.

Una vez que se tiene más soltura a la hora de generar estos scripts de automatización, podemos crear plugins más complejos (tal y como se conocen los complementos que tiene el programa).

Para empezar a crear scripts para QGIS, son necesarias dos cosas:

Tener conocimientos de GIS (saber qué es una capa, un ráster, un geo proceso…)

Tener conocimiento de algún lenguaje de programación. Preferiblemente Python, pero si estás acostumbrado a programar, conocer cualquier lenguaje hará que sea mucho más fácil entrar en el mundo de Python.

Abrir consola de Python:

![Imagen1](https://user-images.githubusercontent.com/119510798/205818077-7171d135-5703-4938-b006-4098c5cefdb1.png)

Con esto, en la parte inferior nos aparece la consola de Python:

![Imagen2](https://user-images.githubusercontent.com/119510798/205818502-d5268d72-f1c5-40fa-9b4f-4db27915935f.png)

En la barra inferior se pueden ir escribiendo comandos para realizar procesos.

La práctica se llevó a cabo en el canal que se sitúa un costado del laboratorio de topografía y se extiende por todo lo largo del andador que esta al costado derecho de donde era antiguamente el campo de fútbol, dentro de las instalaciones de la facultad de ingeniería civil campus Coquimatlán. ubicado en el kilómetro 9, colonia jardines del llano, cp. 28400, Coquimatlán, Colima.

Dicha área de estudio (canal) se encuentra en una condición no muy favorable puesto que con el paso del tiempo la vegetación que crece a su alrededor lo ha estado invadiendo, lo cual de cierta manera lo ha degradado considerablemente y dejando como consecuencia que en ocasión de que se llegue a necesitar no cumpla con el fin propuesto ya que no tendrá una buena conducción de agua debido a la obstrucción de los residuos de la vegetación ya mencionada anteriormente.

Las herramientas que se usaron fueron las siguientes:

Nivel fijo, cinta, cal, libreta de nivel, estadal y las herramientas tecnológicas como Colab y PyQgis.

Método utilizado:

Consiste, en términos generales, en ubicar primero un banco de nivel o un punto de referencia, y después mediante este levantamiento, se obtienen los perfiles o secciones del terreno, transversales a los lados del polígono, cubriendo el área requerida. Los pasos para seguir se describen a continuación:

• Definir las secciones transversales perpendiculares a la línea central en cada estación, espaciándolas según sea conveniente.

•	Tomar lecturas en el centro de las secciones, a la izquierda y a la derecha del eje.

•	Registrarlas debidamente

•	Si el estadal se mueve hasta un punto posterior en cual no se pueden observar más lecturas seleccionar un punto de cambio y efectuar una nivelación compuesta para la determinación de las elevaciones restantes.

•	Medir la distancia hacia los lados del trazo.

•	Repetir esto por todo el camino. (Tomar lecturas sobre el canal).

Ir a gabinete para la realización de los cálculos pertinentes para la representación el perfil y sus secciones. Calcular con ayuda de Excel las cotas que se sacaron en cada punto para después pasar todos esos puntos a un bloc de notas.

Realizar en colab el programa necesario para que los cálculos sean de manera distinta. Primero en Excel y después en Python y de la misma manera que arroje datos a parte de los que Excel pueda manejar.

Pasar a PyQgis para trabajar con las coordenadas arrojadas en el código de colab y poder agregar capas con un código que se pueda correr en el mando de Qgis y que se abran las capas y se puedan usar.

![Imagen4](https://user-images.githubusercontent.com/119510798/205818854-683be4af-d28e-49d9-9c6d-bfbae81834f2.png)


Ejemplo, de como se carga una capa con PyQgis.

**Resultados:**

!pip install basemap

#Calculos de la tolerancia, desnivel y pendiente de las nivelacion de perfil

a= float(input("Ingrese la distancia recorrida en km: ",))

L= a+a

print("La suma de las distancias es: ",L,"km")

#Obtencion de una raiz

from math import sqrt

T= 0.01\*sqrt(L)

print("La tolerancia de la medicion es de: ",T)

#Obtencion del desnivel entre dos puntos

ca= float(input("Ingrese la cota A: ",))

cb= float(input("Ingrese la cota B: ",))

des = (cb-ca)

print("El desnivel entre los 2 puntos` `es:",des,)

if des>0:
`  `print("La pendiente es positiva")

elif des<0:
`  `print("La pendiente es negativa")

else:
`  `print("La pendiente es cero")

Ingrese la distancia recorrida en km: **0.12167**

La suma de las distancias es:  **0.24334 km**

La tolerancia de la medicion es de:  **0.004932950435591259**

Ingrese la cota A: **300**

Ingrese la cota B: **299.086**

El desnivel entre los 2 puntos es: **-0.9139999999999873**

**La pendiente es negativa**

#Grafica de la pendiente

import matplotlib.pyplot as plt

x=[0,a]

y=[ca,cb]

plt.plot(x,y)

plt.title("Pendiente")

plt.xlabel("Distancia en km")

plt.ylabel("Elevacion en m")

plt.show()

![Imagen5](https://user-images.githubusercontent.com/119510798/205819639-71d6e99f-5ea5-4557-a562-804cc0fe3d7e.png)


#Perfil

from google.colab import drive

import matplotlib.pyplot as plt

import os 

from google.colab import files

x = []

y = []

drive.mount('/content/drive') #debemos confirmar acceso a nuestra cuenta para el colab

%cd "/content/drive/MyDrive/Colab Notebooks/PACO"

f=open('PerfilSecciones.txt','r')

for line in f:
`    `lines = [i for i in line.split()]

`    `x.append(lines[0])

`    `y.append(float(lines[1]))



plt.title("Perfil")

plt.xlabel('Distancia')

plt.ylabel('Elevacion')

plt.yticks(y)

plt.plot(x, y, marker = 'o', c = 'g')

plt.show()

![Imagen7](https://user-images.githubusercontent.com/119510798/205819856-e629118d-5a0d-466d-9c30-7c0717e7fbe3.png)

#Secciones

from google.colab import drive

import matplotlib.pyplot as plt

import os 

from google.colab import files

x = []

y = []

drive.mount('/content/drive') #debemos confirmar acceso a nuestra cuenta para el colab

%cd "/content/drive/MyDrive/Colab Notebooks/PACO"

f=open('secpro.txt','r')

for line in f:

`    `lines = [i for i in line.split()]

`    `x.append(lines[0])

`    `y.append(float(lines[1]))



plt.title("Seccion Transversal")

plt.xlabel('Distancia')

plt.ylabel('Elevacion')

plt.yticks(y)

plt.plot(x, y, marker = 'o', c = 'g')

plt.show()

![Imagen6](https://user-images.githubusercontent.com/119510798/205819918-2d4bf2cb-1dfb-43d9-82d9-5edf3d6a3f6a.png)

#Geolocalizar la zona

from geopy.geocoders import Nominatim

import time

import math

lugar = input("Mencione el lugar del levantamiento: ")

geo = Nominatim(user\_agent="MyApp")

loc = geo.geocode(lugar)

print(loc)

print(loc.latitude,loc.longitude)

Mencione el lugar del levantamiento: jardines del llano coquimatlan

**Parque Jardines del llano, Coquimatlán, Colima, México**

**19.2182467 -103.80650544094274**

#Mostrar mapa

from mpl\_toolkits.basemap.test import 

Basemap

import matplotlib.pyplot as plt

geo = geo = Nominatim(user\_agent=

"MyApp",timeout=2)

loc = geo.geocode(lugar)

plt.figure(figsize=(20,16))

my\_map= Basemap(projection="ortho",lon\_0=260,lat\_0=0)

my\_map.drawcoastlines()

my\_map.drawcountries()

my\_map.drawstates()

my\_map.fillcontinents(color="green")

my\_map.drawmapboundary(fill\_color="aqua")

x,y= my\_map(loc.longitude,loc.latitude)

my\_map.plot(x,y,color="red", marker="o",markersize="6")

![Imagen8](https://user-images.githubusercontent.com/119510798/205820252-dbb1c424-f69d-4947-825a-7c688baf67f3.png)

!pip install folium

import folium 

m = folium.Map( location=[19.212646978209623, -103.80425883150892], zoom\_start=12, tiles='Stamen Terrain' ) 

tooltip = 'FIC'

folium.Marker([19.212646978209623, -103.80425883150892], popup='FIC', tooltip=tooltip).add\_to(m) 

m

![Imagen9](https://user-images.githubusercontent.com/119510798/205820388-163f872d-08dc-41d7-88e5-f1665616e494.png)

Codigo en PyQgis

from qgis.gui import \*

import PyQt5.QtGui

import PyQt5.QtCore

from PyQt5.QtCore import \*

from PyQt5.QtGui import \*

from qgis.core import \*

#lienzo Raster y vectorial

Colima = r'''C:\Users\FRANCISCO\OneDrive\

Escritorio\Francisco- 5.10\PACO\B5.TIF'''

fileInfo = QFileInfo(Colima)

baseName = fileInfo.baseName()

rlayer = QgsRasterLayer(Colima, baseName)

QgsProject.instance().addMapLayer(rlayer)

#lienzo Raster y vectorial

Colima = r'''C:\Users\FRANCISCO\Downloads\

Municipios\_Colima\Municipios\_Colima\_UTM.shp'''

fileInfo = QFileInfo(Colima)

baseName = fileInfo.baseName()

vlayer = QgsVectorLayer(Colima, baseName)

QgsProject.instance().addMapLayer(vlayer)

#lienzo Raster y vectorial

Colima = r'''C:\Users\FRANCISCO\OneDrive\

Escritorio\Proyecto\_3\_Semestre\_EQ1\

Coordenadas\_UTM.shp'''

fileInfo = QFileInfo(Colima)

baseName = fileInfo.baseName()

vlayer = QgsVectorLayer(Colima, baseName)

QgsProject.instance().addMapLayer(vlayer)

![Imagen10](https://user-images.githubusercontent.com/119510798/205820472-76347ec6-5eaf-486f-af9d-3fcee2e4d1ad.png)


**Conclusiones:**

Se puede concluir con que fue un proyecto en el que se pusieron a prueba las habilidades del alumno como programador ya que para el curso en el que se va, se debe saber lo básico de Python que es el lenguaje con el que se ha venido trabajando y gracias a esto, la realización de los códigos para este proyecto se pudo llevar a acabo de buena manera. Se incorporó la parte geoespacial, utilizando librerías como Basemap o folium, que ayudan a la impresión y visualización de los mapas cargados con unas instrucciones previamente dadas por el usuario. Habilidades con el Pyqgis, que es una herramienta muy buena para de alguna forma automatizar procesos dentro de lo que es la cartografía de un lugar y poder llevar a a cabo los trabajos rápidos y eficaces.

**Referencias:**

1. (2021, 11 marzo). Que son y para que se usan las secciones transversales? – RESPUESTASRAPIDAS. respuestas rapidas. <https://respuestasrapidas.com.mx/que-son-ypara-que-se-usan-las-secciones-transversales/>

[https://www.comunidadism.es/como-empiezo-con-pyqgis-para-que-me-sirve/#](https://www.comunidadism.es/como-empiezo-con-pyqgis-para-que-me-sirve/)

Aguilera Francisco, García Barbara, García Jorge. *Título: Secciones transversales y el uso de herramientas tecnológicas. Subtítulo: Python en Topografía //* Ibersid. (2008) p1-pn. ISSN 1888-0967.

