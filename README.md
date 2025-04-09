# TIA_Tarea_1
# Tarea 1: Optimización, Histogramas, Sistemas Dinámicos Lineales y Generación de Datos

Este repositorio contiene la solución y análisis de los siguientes problemas divididos en cuatro partes principales:

---

## Parte I: Optimización

### Problema 1: Optimización de un Contenedor

**Maximizar** el volumen de un cilindro \( V = \pi r^2 h \) sujeto a la restricción de área superficial:

\[
2\pi rh + 2\pi r^2 = A_0
\]

### Problema 2: Diseño de Redes

**Minimizar** la pérdida de energía en un conductor eléctrico \( P = I^2R \) donde \( R = \frac{\rho L}{A} \):

\[
\text{Minimizar } f(A) = \frac{I^2 \rho L}{A}
\]
Sujeto a:
\[
A + \frac{L}{A} = 15
\]

---

## Parte II: Histogramas

### Problema 1: Datos Continuos

Datos de temperatura y velocidad del viento en Bogotá.

1. Dividir los datos en bins  
2. Dibujar histograma  
3. Estimar la Función de Masa de Probabilidad (PMF)  
4. Discutir si la distribución es normal o sesgada

### Problema 2: Comparación de Histogramas y PDFs

Comparación entre datos de Bogotá y Cartagena.

1. Crear histogramas con diferentes anchos de bin  
2. Estimar PMFs para ambos  
3. Comparar distribuciones y determinar cuál tiene mayor dispersión  
4. Calcular la correlación cruzada entre temperatura y velocidad del viento

---

## Parte III: Sistemas Dinámicos Lineales

Sistema masa-resorte-amortiguador:

\[
mẍ(t) + cẋ(t) + kx(t) = f(t)
\]

- **m**: masa (200 g)  
- **c**: coeficiente de amortiguamiento  
- **k**: constante del resorte  
- **f(t)**: señal de aceleración real

### 1. Simulación del sistema

- Señal sinusoidal como entrada  
- Simular con ruido  
- Histograma y entropía de entrada, \( x(t) \), \( ẋ(t) \)

### 2. Ajuste del sistema

- Minimizar la entropía de salida aumentando el amortiguamiento  
- \( k = 0.5c^2 \)  
- Simular y calcular PMF y entropía de las señales

### 3. Mitigación de vibraciones

- Usar aceleración real como entrada  
- Comparar histogramas de entrada y salida  
- Comentar sobre la capacidad del sistema para reducir la entropía

---

## Parte IV: Extracción de Características y Generación Sintética de Datos

### Análisis Exploratorio de Datos Reales

1. Cargar datos de eventos: posición de pie, movimiento estándar y bache  
2. Visualización temporal de la señal z (señal 5)  
3. Histogramas, PMF, PDF  
4. Métricas estadísticas:  
   - Media (\( \mu \)), desviación estándar (\( \sigma \)), varianza, asimetría, curtosis  
   - Entropía:

\[
H = - \sum_i p(x_i) \log p(x_i)
\]

5. Entropía con ventana móvil  
6. Comparación de PMF y entropía para diferenciar comportamientos de vibración

### Generación de Señales

#### 1. Análisis por Intervalos de Tiempo Gaussiano

- Preprocesar con Transformada de Hilbert y ventana móvil  
- Algoritmo Bootstrap / Cu-sum para segmentar  
- Comparar entropía entre señales reales y sintéticas

#### 2. Generar señales

- Crear intervalos de tiempo desde la distribución obtenida  
- Asignar media y desviación estándar a cada intervalo  
- Generar al menos dos señales por tipo de evento

#### 3. Validación

- Comparar estadísticas clave: media, varianza, asimetría, curtosis  
- Comparación de entropía

#### 4. Evaluación de Calidad

- Comparar PDFs  
- Validar similitud de entropía

---

**Autores:**  
Nombre del estudiante  
Universidad / Curso  
Fecha
