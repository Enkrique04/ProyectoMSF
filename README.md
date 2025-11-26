# Proyecto: Sistema optico

## Información del estudiante

Ian E. Estrada [22211753]; l22211753@tectijuana.edu.mx

Modelado de Sistemas Fisiológicos

Ingeniería Biomédica

## Docente

Dr. Paul Antonio Valle Trujillo; paul.valle@tectijuana.edu.mx

Departamento de Ingeniería Eléctrica y Electrónica, Tecnológico Nacional de México/IT Tijuana, Blvd. Alberto Limón Padilla s/n, Tijuana, C.P. 22454, B.C., México.

## Descripción de la asignatura

El modelizado de sistemas fisiológicos es una herramienta importante en Ingeniería Biomédica, permite comprender el funcionamiento del cuerpo humano, así como diseñar y evaluar terapias y dispositivos médicos; se define como el proceso de formular modelos matemáticos o computacionales que representan el comportamiento y la interacción de los sistemas biológicos y fisiológicos. Esta asignatura pretende aportar al perfil del Ingeniero Biomédico la capacidad de realizar investigación científica en el área de Biología de Sistemas con la finalidad de dirigir y participar en equipos de trabajo interdisciplinarios en contextos nacionales e internacionales, así como de proporcionar soluciones informáticas para resolver problemas en el campo de la Ingeniería Biomédica con ética profesional; lo anterior al proporcionar al estudiante bases sólidas para modelizar sistemas y diseñar controladores para la solución de problemas en las áreas de atención médica y del sector industrial médico. La construcción de analogías entre circuitos eléctricos y sistemas fisiológicos para la formulación de modelos matemáticos y el diseño de controladores mediante la experimentación in silico brindan herramientas de gran aplicación en el quehacer profesional del Ingeniero Biomédico.

La asignatura de Modelado de Sistemas Fisiológicos forma parte del plan de estudios de la carrera en Ingeniería Biomédica con la siguiente competencia general del curso: Utiliza las propiedades de los circuitos RLC para describir la dinámica de sistemas fisiológicos, obtener modelos matemáticos y aplicar el control clásico, esto con el objetivo de integrar los principios de la Ingeniería de Control, la Electrónica Analógica y las Ciencias de la Computación con la Anatomía y Fisiología del cuerpo humano para proporcionar descripciones cuantitativas y cualitativas de sistemas fisiológicos complejos con el objetivo de modelizar, analizar, controlar, ilustrar y predecir su dinámica tanto en el corto como en el largo plazo.

## Objetivos
1. Resolver el sistema de EDOs mediante el método de Euler.
2. Graficar el caso con transfusión sanguínea y sin transfusión sanguínea del individuo.
 

## Descripción detallada del sistema

El sistema óptico, en particular el comportamiento de un fotoreceptor de la retina (bastón o cono) ante un estímulo luminoso, puede representarse de forma simplificada mediante un modelo que simule la dinámica de la transducción de luz en señal eléctrica. Este proceso puede describirse mediante un circuito equivalente donde se representan el retardo bioquímico, la conductancia de la membrana y la variación del potencial eléctrico del fotoreceptor.El comportamiento de este sistema, modelado mediante un circuito eléctrico de segundo orden, se establece bajo las siguientes suposiciones:

1. El retardo bioquímico de la cascada de fototransducción, que incluye la activación de la rodopsina, transducina y PDE, se modela mediante una inductancia L, representando la inercia del sistema ante cambios rápidos de luz.

2. La resistencia interna del fotoreceptor, asociada al transporte iónico longitudinal y pérdidas internas antes de llegar a la membrana, se modela mediante un resistor en serie R1.

3. La capacitancia de la membrana del fotoreceptor, responsable de almacenar carga y regular la velocidad a la que cambia el potencial de membrana, se modela mediante un capacitor C.

4. La conductancia dependiente de cGMP, que regula la entrada de iones Na⁺ y Ca²⁺ a través de los canales sensibles a cGMP y determina la corriente en oscuridad, se modela con un resistor R2 en paralelo con el capacitor. Esta resistencia puede interpretarse como la vía por la cual se “descarga” o regula el potencial del fotoreceptor.

5. El potencial de salida del circuito, Vout(t), representa el potencial de membrana del fotoreceptor, el cual se hiperpolariza cuando disminuye la concentración de cGMP por acción de la luz.

6. El flujo fotoeléctrico, equivalente a la absorción de fotones y activación de la rodopsina, se interpreta como el flujo de señal que atraviesa la rama serie L–R1 hasta el nodo de la membrana (representado por la combinación R2–C).

La señal de entrada al sistema, Ve(t), se modela como un impulso unitario de luz, equivalente a un destello breve que activa de manera súbita la cascada de fototransducción. Esta señal permite estudiar la respuesta transitoria del fotoreceptor, incluyendo el retardo inicial, el pico de hiperpolarización y el retorno al estado de reposo, de forma análoga a cómo el fotoreceptor reacciona ante un estímulo visual abrupto.

Palabras clave: ?,?,?,?,?.

## Lista de archivos incluidos en el repositorio

1. Cuaderno computacional de MATLAB \[.mlx].
2. Imágenes de las simulaciones \[.pdf y .png].

## Referencias

[1] P. A. Valle, Syllabus para Modelado de Sistemas Fisiológicos, Tecnológico Nacional de México / Instituto Tecnológico de Tijuana, Tijuana, B.C., México, 2025. Permalink: https://biomath.xyz/course/

[2]  M. Tetschke, P. Lilienthal, T. Pottgiesser, T. Fischer, E. Schalk & S. Sager, Mathematical Modeling of RBC Count Dynamics after Blood Loss , Processes, vol. 6, issue 9, Sep 2018. https://doi.org/10.3390/pr6090157
