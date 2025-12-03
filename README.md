[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=Enkrique04/ProyectoMSF)
# Proyecto: Sistema optico

## Información de los estudiantes

German E. Avila [22212250]; L22212250@tectijuana.edu.mx

Josue Chizek Espinoza [22212382]; l22212382@tectijuana.edu.mx

Ian E. Estrada [22211753]; l22211753@tectijuana.edu.mx

Diego S. Lopez [22211759]; L22211759@tectijuana.edu.mx

Modelado de Sistemas Fisiológicos

Ingeniería Biomédica

## Docente

Dr. Paul Antonio Valle Trujillo; paul.valle@tectijuana.edu.mx

Departamento de Ingeniería Eléctrica y Electrónica, Tecnológico Nacional de México/IT Tijuana, Blvd. Alberto Limón Padilla s/n, Tijuana, C.P. 22454, B.C., México.

## Descripción de la asignatura

El modelizado de sistemas fisiológicos es una herramienta importante en Ingeniería Biomédica, permite comprender el funcionamiento del cuerpo humano, así como diseñar y evaluar terapias y dispositivos médicos; se define como el proceso de formular modelos matemáticos o computacionales que representan el comportamiento y la interacción de los sistemas biológicos y fisiológicos. Esta asignatura pretende aportar al perfil del Ingeniero Biomédico la capacidad de realizar investigación científica en el área de Biología de Sistemas con la finalidad de dirigir y participar en equipos de trabajo interdisciplinarios en contextos nacionales e internacionales, así como de proporcionar soluciones informáticas para resolver problemas en el campo de la Ingeniería Biomédica con ética profesional; lo anterior al proporcionar al estudiante bases sólidas para modelizar sistemas y diseñar controladores para la solución de problemas en las áreas de atención médica y del sector industrial médico. La construcción de analogías entre circuitos eléctricos y sistemas fisiológicos para la formulación de modelos matemáticos y el diseño de controladores mediante la experimentación in silico brindan herramientas de gran aplicación en el quehacer profesional del Ingeniero Biomédico.

La asignatura de Modelado de Sistemas Fisiológicos forma parte del plan de estudios de la carrera en Ingeniería Biomédica con la siguiente competencia general del curso: Utiliza las propiedades de los circuitos RLC para describir la dinámica de sistemas fisiológicos, obtener modelos matemáticos y aplicar el control clásico, esto con el objetivo de integrar los principios de la Ingeniería de Control, la Electrónica Analógica y las Ciencias de la Computación con la Anatomía y Fisiología del cuerpo humano para proporcionar descripciones cuantitativas y cualitativas de sistemas fisiológicos complejos con el objetivo de modelizar, analizar, controlar, ilustrar y predecir su dinámica tanto en el corto como en el largo plazo.

## Objetivos
1. Analizar la respuesta dinámica del sistema de fototransducción mediante un modelo de circuito RLC.
2. Graficar y comparar el comportamiento dinámico entre el caso de un ojo sano y uno con degeneración retinal (Retinitis Pigmentosa).
3. Interpretar las variaciones en la sensibilidad y temporalidad de la señal de salida ($V_{out}$) ante cambios paramétricos fisiológicos.
 

## Descripción detallada del sistema

El siguiente modelo matemático basado en un circuito eléctrico RLC serie-paralelo es una representación analógica de la transducción visual, el proceso mediante el cual un fotón de luz genera una respuesta nerviosa en los fotorreceptores de la retina.
Con respecto a las variables del sistema, la entrada $V_{in}$ modela el flujo de fotones absorbidos por el pigmento (fuente), mientras que la salida $V_{out}$ representa el potencial de membrana resultante. Los componentes del circuito no son físicos, sino que modelan dinámicas fisiológicas específicas: la inductancia $L$ representa la inercia fisiológica o el retardo en la cascada química (transducina/fosfodiesterasa); la capacitancia $C$ modela la capacidad de almacenamiento de carga en los discos membranosos del fotorreceptor; $R_1$ describe la resistividad del segmento celular y fugas iónicas; y $R_2$ representa la eficiencia sináptica hacia las células bipolares.
La degeneración retinal se simula alterando estos parámetros para reflejar la pérdida de estructura del tejido y la muerte celular, lo que resulta en una respuesta más lenta, sobreamortiguada y con menor ganancia.

El sistema se analizó con los siguientes parámetros de resistencia, inductancia y capacitancia:

Para el caso Sano, se propusieron los valores basales:
1. $R_1 = 1.0\ k\Omega$
2. $R_2 = 0.8\ k\Omega$
3. $C = 0.02\ F$
4. $L = 0.1\ H$ 

Para el caso con Degeneración Retinal, se utilizaron valores modificados que reflejan el daño fisiológico (menor conductancia y pérdida de discos):
1. $R_1 = 1.2\ k\Omega$ (Aumento por menor conductancia de membrana)
2. $R_2 = 2.0\ k\Omega$ (Aumento drástico por pérdida de conectividad sináptica)
3. $C = 0.008\ F$ (Disminución por reducción del área de membrana)
4. $L = 0.15\ H$ (Aumento por retardo en la cinética química)

Palabras clave: Fototransducción; Circuito RLC; Degeneración Retinal; Fotorreceptores; Modelado dinámico.

## Lista de archivos incluidos en el repositorio

1. Cuaderno computacional de MATLAB \[.mlx].
2. Imágenes de las simulaciones \[.pdf y .png].

## Referencias

[1] Lamb, T. D., & Pugh Jr, E. N. (1992). A quantitative account of the activation steps involved in phototransduction in amphibian photoreceptors. The Journal of Physiology, 449(1), 719-758.

[2] Hille, B. (2001). Ion Channels of Excitable Membranes (3rd ed.). Sinauer Associates.

[3] Hartong, D. T., Berson, E. L., & Dryja, T. P. (2006). Retinitis pigmentosa. The Lancet, 368(9549), 1795-1809.
