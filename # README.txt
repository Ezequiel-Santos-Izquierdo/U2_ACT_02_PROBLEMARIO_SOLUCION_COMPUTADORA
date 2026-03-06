# README

## Calculadora Computacional para el Diseño de Ejes

### Asignatura: Diseño de Elementos Mecánicos – Ingeniería Mecatrónica

---

# Descripción del proyecto

Este proyecto consiste en el desarrollo de un algoritmo en Python para el análisis y diseño de ejes mecánicos, como parte de la actividad U2_ACT_02: Problemario solución por computadora de la asignatura Diseño de Elementos Mecánicos.

El objetivo del programa es automatizar los cálculos necesarios para el análisis de ejes sometidos a flexión y torsión combinadas, aplicando los criterios de diseño estudiados en la asignatura.

El algoritmo permite calcular los parámetros solicitados en la actividad académica, tales como:

* Sensibilidades a la muesca
* Factores de concentración de esfuerzo
* Factores de concentración por fatiga
* Esfuerzos alternantes y medios
* Esfuerzos equivalentes de Von Mises
* Esfuerzo máximo equivalente
* Factor de diseño de Von Mises
* Factor de diseño mediante criterios de fatiga

Este código fue desarrollado como herramienta computacional para resolver los casos del problemario, facilitando el proceso de cálculo requerido en el diseño de ejes en sistemas mecánicos y mecatrónicos.

---

# Funcionalidad del algoritmo

El código desarrollado sigue la estructura solicitada en el documento de la actividad y resuelve los siguientes incisos.

---

## a) Sensibilidades a la muesca

El programa permite ingresar los valores de:

* q → sensibilidad a la muesca en flexión
* qs → sensibilidad a la muesca en cortante

Estos parámetros se utilizan posteriormente para calcular los factores de concentración de esfuerzo por fatiga.

---

## b) Factores de concentración de esfuerzo

Se ingresan los parámetros geométricos del eje:

* D → diámetro mayor
* d → diámetro menor
* r → radio del entalle

Además de los factores:

* Kt → factor de concentración de esfuerzo en flexión
* Kts → factor de concentración de esfuerzo en torsión

El programa calcula también las relaciones geométricas:

D/d
r/d

Las cuales son utilizadas en las tablas de concentración de esfuerzos del diseño de ejes.

---

## c) Factores de concentración por fatiga

El algoritmo calcula:

Kf → factor de concentración por fatiga en flexión
Kfs → factor de concentración por fatiga en torsión

Utilizando la ecuación:

Kf = 1 + q(Kt − 1)

Kfs = 1 + qs(Kts − 1)

También se permite introducir estos valores directamente si ya se conocen.

---

## d) Esfuerzos en la sección crítica del eje

Se calculan los esfuerzos normal y cortante:

σa → esfuerzo normal alternante
σm → esfuerzo normal medio
τa → esfuerzo cortante alternante
τm → esfuerzo cortante medio

Las ecuaciones utilizadas corresponden al análisis de ejes circulares sometidos a flexión y torsión.

---

## e) Esfuerzos equivalentes de Von Mises

Para evaluar el estado combinado de esfuerzos se calculan los esfuerzos equivalentes:

σa' → esfuerzo equivalente alternante de Von Mises
σm' → esfuerzo equivalente medio de Von Mises

Estos valores permiten analizar el comportamiento del material bajo cargas variables.

---

## f) Esfuerzo máximo equivalente

El programa calcula el esfuerzo máximo equivalente de Von Mises:

σmax' = σm' + σa'

Este valor se utiliza para evaluar el riesgo de fluencia del material.

---

## g) Factor de diseño de Von Mises

El algoritmo calcula el factor de diseño contra fluencia:

n = Sy / σmax'

donde:

Sy = límite de fluencia del material.

---

## h) Factores de diseño por criterios de fatiga

El programa calcula factores de diseño mediante:

* Criterio de Goodman
* Criterio de Gerber

Estos criterios son utilizados en el diseño de elementos mecánicos sometidos a cargas fluctuantes.

---

# Librerías utilizadas

El programa utiliza la librería estándar de Python:

math

Esta librería permite realizar operaciones matemáticas necesarias como:

* raíces cuadradas
* potencias
* uso de π

La selección de esta librería se debe a su eficiencia y disponibilidad en Python sin necesidad de instalar paquetes adicionales.

---

# Gestión de entrada y salida de datos

El programa utiliza una función personalizada para manejar la entrada de datos:

* Permite introducir valores manualmente
* Permite dejar campos vacíos
* El sistema detecta automáticamente qué cálculos pueden realizarse

Esto permite que el programa funcione como una calculadora flexible para diferentes casos de diseño.

Los resultados se muestran directamente en la consola mediante mensajes que indican si cada inciso fue:

* Resuelto completamente
* Resuelto parcialmente
* No resuelto por falta de datos

---

# Aplicación académica

Este algoritmo fue desarrollado para apoyar la resolución de los casos del problemario de la Unidad 2, donde se solicita implementar una solución computacional para el análisis de ejes. 

El programa facilita el cálculo de todos los incisos solicitados en el documento de la actividad, permitiendo verificar rápidamente los resultados obtenidos en los ejercicios.

---

# Autores

CHABLÉ IZQUIERDO, MIGUEL ÁNGEL
DE LA CRUZ YEDRA, KEVIN RUBÉN
DOMÍNGUEZ HERNÁNDEZ, PERLA DEL CARMEN
GARCÍA MARTÍNEZ, ARTURO
MÉNDEZ MÉNDEZ, JOSÉ JUAN
PÉREZ TEOFANI, ALEXANDER
SANTOS IZQUIERDO, EZEQUIEL

---

# Asignatura

Diseño de Elementos Mecánicos
Carrera: Ingeniería Mecatrónica

---

# Licencia

Este proyecto se distribuye bajo la MIT License, una licencia de software libre que permite:

* Uso del código
* Modificación
* Distribución
* Uso académico y profesional

Siempre que se mantenga el reconocimiento a los autores originales.

---

# Ejecución del programa

Para ejecutar el programa:

1. Instalar Python 
2. Copiar el código en un archivo `.py`
3. Ejecutar el archivo desde un editor o terminal

Ejemplo:

```
python calculadora_ejes.py
```

El programa solicitará los datos necesarios y mostrará los resultados de cada inciso.

---

# Conclusión

El desarrollo de esta herramienta computacional permite aplicar de manera práctica los conceptos de diseño de ejes estudiados en la asignatura Diseño de Elementos Mecánicos.

El uso de programación para resolver problemas de ingeniería es una habilidad clave en Ingeniería Mecatrónica, ya que permite automatizar cálculos complejos, reducir errores y mejorar la eficiencia en el diseño de sistemas mecánicos.
