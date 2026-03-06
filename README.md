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
