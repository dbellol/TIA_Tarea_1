# Tarea 1: Optimización, Histogramas, Sistemas Dinámicos Lineales y Generación de Datos

Este repositorio contiene la solución y análisis de los siguientes problemas divididos en cuatro partes principales:

---

## Parte I: Optimización

### Problema 1: Optimización de un Contenedor

**Maximizar** el volumen de un cilindro:

$$ V = \pi r^2 h $$

Sujeto a la restricción de área superficial:

$$ 2\pi rh + 2\pi r^2 = A_0 $$

### Problema 2: Diseño de Redes

**Minimizar** la pérdida de energía:

$$ P = I^2 R, \quad R = \frac{\rho L}{A} $$

Función objetivo:

$$ \min f(A) = \frac{I^2 \rho L}{A} $$

Sujeto a:

$$ A + \frac{L}{A} = 15 $$

---

## Parte II: Histogramas

### Problema 1: Datos Continuos

- Dividir los datos en bins  
- Dibujar histogramas  
- Estimar PMF  
- Evaluar normalidad o sesgo

### Problema 2: Comparación de Histogramas

- Crear histogramas para Bogotá y Cartagena  
- Estimar PMF  
- Comparar las distribuciones  
- Calcular correlación cruzada

---

## Parte III: Sistemas Dinámicos Lineales

Modelo masa-resorte-amortiguador:

$$ m\ddot{x}(t) + c\dot{x}(t) + kx(t) = f(t) $$

Parámetros:

- $$ \( m = 200 \text{g} \)  $$
- $$ \( f(t) \): señal real de entrada $$

### Simulación

- Señal sinusoidal como entrada  
- Añadir ruido  
- Calcular histograma y entropía de $$ \( x(t) \) y \( \dot{x}(t) \) $$

### Ajuste

- Minimizar entropía de salida  
- Relación: $$ \( k = 0.5c^2 \) $$

### Mitigación de Vibraciones

- Entrada: señal de aceleración  
- Comparar histogramas de entrada/salida  
- Analizar reducción de entropía

---

## Parte IV: Extracción de Características y Generación Sintética

### Análisis Exploratorio

- Cargar señales reales (posición de pie, movimiento, bache)  
- Graficar la aceleración z  
- Estimar PMF, PDF y métricas estadísticas:  
  $$ \mu, \quad \sigma, \quad \text{skewness}, \quad \text{kurtosis} $$

#### Entropía

$$ H = -\sum_i p(x_i) \log p(x_i) $$ 

- Cálculo de entropía con ventana móvil  
- Comparación de patrones de vibración

### Generación de Señales

1. Análisis de intervalos usando Hilbert + Cu-sum  
2. Generación de intervalos sintéticos  
3. Validación con métricas y entropía  
4. Evaluación de calidad comparando PDFs y entropía

---

**Autores:**  
### Nombre del estudiante: 
- Diana Marcela Bello López
- Cristián Tovar
### Universidad:
Universidad Nacional de Colombia
### Curso: 
Técnicas de inteligencia artificial
Fecha
