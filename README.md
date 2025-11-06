[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=rafael-herrera-aguilar/Practica_4_MSF)

# Práctica 4: Regeneración de glóbulos rojos

## Información del estudiante

Rafael Herrera Aguilar \[22212258]; l22212258@tectijuana.edu.mx

Modelado de Sistemas Fisiológicos

Ingeniería Biomédica

## Docente

Dr. Paul Antonio Valle Trujillo; paul.valle@tectijuana.edu.mx

Departamento de Ingeniería Eléctrica y Electrónica, Tecnológico Nacional de México/IT Tijuana, Blvd. Alberto Limón Padilla s/n, Tijuana, C.P. 22454, B.C., México.

## Descripción de la asignatura

El modelizado de sistemas fisiológicos es una herramienta importante en Ingeniería Biomédica, permite comprender el funcionamiento del cuerpo humano, así como diseñar y evaluar terapias y dispositivos médicos; se define como el proceso de formular modelos matemáticos o computacionales que representan el comportamiento y la interacción de los sistemas biológicos y fisiológicos. Esta asignatura pretende aportar al perfil del Ingeniero Biomédico la capacidad de realizar investigación científica en el área de Biología de Sistemas con la finalidad de dirigir y participar en equipos de trabajo interdisciplinarios en contextos nacionales e internacionales, así como de proporcionar soluciones informáticas para resolver problemas en el campo de la Ingeniería Biomédica con ética profesional; lo anterior al proporcionar al estudiante bases sólidas para modelizar sistemas y diseñar controladores para la solución de problemas en las áreas de atención médica y del sector industrial médico. La construcción de analogías entre circuitos eléctricos y sistemas fisiológicos para la formulación de modelos matemáticos y el diseño de controladores mediante la experimentación in silico brindan herramientas de gran aplicación en el quehacer profesional del Ingeniero Biomédico.

La asignatura de Modelado de Sistemas Fisiológicos forma parte del plan de estudios de la carrera en Ingeniería Biomédica con la siguiente competencia general del curso: Utiliza las propiedades de los circuitos RLC para describir la dinámica de sistemas fisiológicos, obtener modelos matemáticos y aplicar el control clásico, esto con el objetivo de integrar los principios de la Ingeniería de Control, la Electrónica Analógica y las Ciencias de la Computación con la Anatomía y Fisiología del cuerpo humano para proporcionar descripciones cuantitativas y cualitativas de sistemas fisiológicos complejos con el objetivo de modelizar, analizar, controlar, ilustrar y predecir su dinámica tanto en el corto como en el largo plazo.

## Objetivos

1. Resolver el sistema de EDOs mediante el método de Euler (diferencias finitas).
2. Graficar sistema de EDOs en MATLAB.
3. Considerar el caso de transfusión sanguínea del individuo mediante la siguiente función:

## Descripción detallada del sistema

El siguiente modelo matemático de tres EDOs de primer orden es un modelo mecanicista de compartimento para la eritropoyesis después de la prdida de sangre en personas sanas, fenómeno que se puede modelizar como un proceso dinámico no lineal, donde x1(t) representa el compartimento de células precursoras eritroides altamente proliferantes con respecto a la eritropoyetina, x2(t) describe el compartimento no proliferante de células precursoras eritroides con respecto a la eritropoyetina, y x3(t) el compartimento para los eritrocitos maduros y reticulocitos sanguíneos.

Con respecto a los parámetros, X0 refleja la cantidad absoluta de células que se destinan al linaje eritroide y que maduran en el primer compartimento de células precursoras eritroides. Las tasas de transición y las tasas de mortalidad entre los compartimentos están dadas por k1, k2 y alpha, estas tasas son independientes de la hormona eritropoyetina. La compensación de la pérdida de sangre se describe mediante un término de retroalimentacién de los eritrocitos a las células en proliferación basado en la pérdida fraccional de eritrocitos. Con base en lo anterior, se introducen los parámetros beta y gamma, que se utilizan para la descripción de las características individuales de la eritropoyesis. Se asume que cada individuo tiene un recuento medio de eritrocitos indicado por el parámetro Base. 

Condiciones iniciales 
x1_0 = 
   58.2837   56.9020   56.3817   56.8495   57.1793   60.1951   58.3125   60.1429   57.8993   60.2531
x2_0 = 
   43.4658   42.4354   42.0474   42.3962   42.6422   44.8912   43.4873   44.8523   43.1791   44.9345
x3_0 = 
  874.2552  853.5304  845.7259  852.7427  857.6893  902.9258  874.6877  902.1438  868.4890  903.7969

Parámetros de beta y gamma
gamma = [0.769, 0.388, 0.510, 0.590, 0.262, 0.324, 0.356, 0.089, 0.243, 0.057]
beta = [1.650, 0.867, 1.617, 2.615, 1.518, 2.676, 0.891, 2.557, 0.925, 0.089]

Palabras clave: Regeneración de glóbulos rojos, Sistema de EDOs, Parámetros de estimación, Simulaciones numéricas.

## Lista de archivos incluidos en el repositorio

1. Cuaderno computacional de MATLAB \[.mlx].
2. Imagen de la simulación sin transfusión \[.pdf].
3. Imagen de la simulación con transfusión \[.pdf].

## Referencias

\[1] P. A. Valle, Syllabus para Modelado de Sistemas Fisiológicos, Tecnológico Nacional de México / Instituto Tecnológico de Tijuana, Tijuana, B.C., México, 2025. Permalink: https://biomath.xyz/course/

\[2] Tetschke, M., Lilienthal, P., Pottgiesser, T., Fischer, T., Schalk, E., & Sager, S. (2018). Mathematical modeling of RBC count dynamics after blood loss. Processes, 6(9), 157. https://doi.org/10.3390/pr6090157
