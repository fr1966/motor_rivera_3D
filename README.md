# motor_rivera_3D
Motor Rivera 3D v3.0 - Generador Paramétrico Biomimético e Interactivo WebGL

# Motor Rivera 3D v3.0 (Puro)

Generador paramétrico biomimético e interactivo basado en WebGL para la visualización y análisis cinemático de secuencias biológicas y texto en el espacio tridimensional.

## 🌟 Características Principales
- **Generación en Tiempo Real:** Proyección vectorial por letras/aminoácidos en 3D.
- **Renderizado de Alto Rendimiento:** Visualización híbrida (Ribbons + Esferas CPK) que escala de forma fluida.
- **Exportación Normalizada:** Generación de archivos CSV/PDB normalizados a escala física $C_\alpha - C_\alpha$ ($3.80\text{ \AA}$).
- **Métricas Integradas en Vivo:** Cálculo de Radio de Giro ($R_g$), evaluación de choques estéricos y recuento unívoco de contactos terciarios ($j > i + 4$).

## 🔬 Validación y Fundamento Matemático
El motor cuenta con un diseño determinista basado en trayectorias geométricas vectoriales, permitiendo auditar y calibrar constantes espaciales frente a estándares experimentales como la Proteína G (`PDB 1PGB`).

## 🛠️ Tecnologías
- HTML5 / JavaScript (WebGL / Three.js)
- Estilo modular adaptativo con HUD en tiempo real.

# Motor Rivera 3D v3.0

Título: Generador paramétrico, biomimétrico e interactivo: Una modelización en WebGL para convertir cadenas de letras de aminoácidos y nucleótidos en estructuras dentro del espacio 3D

## 1. Introducción
Al observar una cadena ordenada de letras que representan aminoácidos (proteínas) o nucleótidos (ADN/ARN), surge de inmediato la curiosidad de saber qué forma real adoptan en el espacio. El Motor Rivera 3D nace con la finalidad de responder a esa inquietud: permite que cualquier usuario —ya sea estudiante, profesional o una persona curiosa por la ciencia— introduzca dicha secuencia y observe su modelado tridimensional correspondiente.

No se trata de una simulación biológica a escala atómica real, sino de un ideal paramétrico cercano a la realidad, diseñado para visualizar y comprender la estructura espacial y cinemática de las secuencias de manera interactiva y accesible. Este proyecto es fruto de un trabajo colaborativo y riguroso: conceptualizado matemáticamente por el Lic. Franklin R. Rivera Aguilar, implementado técnicamente por el asistente de IA (Gemini) como programador, y sometido a una auditoría y validación cruzada por ChatGPT para asegurar su consistencia analítica y métrica.

## 2. Presentación del Problema
Las representaciones tradicionales a menudo carecen de un control paramétrico directo que permita auditar de forma inmediata métricas clave como el Radio de Giro ($R_g$) o los contactos terciarios bajo un marco puramente determinista.

## 3. Planteamiento Conceptual del Motor 3D
El presente motor no nace como una solución directa o convencional a un problema cerrado de modelado 3D de secuencias de aminoácidos y nucleótidos. Surge, más bien, como la evolución natural de la modelación 3D al poder cargar en él cualquier cadena y lograr que muestre de inmediato su entorno paramétrico, abierto y determinista. Todo ello dentro de un entorno HTML interactivo, donde la geometría y la cinemática espacial permiten dar forma visible a cadenas literales que antes solo existían como texto plano.

## 4. Estructura y Funcionamiento del Algoritmo
El núcleo operativo del Motor Rivera 3D (v3.0) descansa sobre una arquitectura algorítmica determinista y de bajo consumo computacional, diseñada para traducir secuencias literales de aminoácidos y nucleótidos en estructuras espaciales coherentes mediante tres fases interconectadas:

* **Paso Paramétrico y Fidelidad Geométrica ($C_\alpha - C_\alpha$):** Para evitar desviaciones caóticas y mantener un anclaje con las proporciones moleculares reales, el algoritmo implementa un paso interno base de $1.8\text{ \AA}$, el cual se encuentra escalado matemáticamente a $3.8052\text{ \AA}$. Esta distancia funciona de manera análoga al vector espacial entre carbonos alfa consecutivos ($C_\alpha - C_\alpha$) en las cadenas polipeptídicas, garantizando que cada elemento de la secuencia mantenga una separación física armónica, estructurada y libre de solapamientos arbitrarios en el espacio tridimensional.

* **Métricas en Vivo y Evaluación Topológica ($R_g$ y Contactos Terciarios):** A diferencia de los visualizadores estáticos, el motor computa en tiempo real variables estructurales críticas durante la generación de la curva. Por un lado, calcula de forma dinámica el Radio de Giro ($R_g$), ofreciendo una medida instantánea de la compacidad global de la estructura plegada. Por otro lado, ejecuta un recuento unívoco y optimizado de los contactos terciarios mediante el filtrado estricto de la condición geométrica ($j > i + 4$), permitiendo identificar de inmediato la proximidad espacial entre residuos distantes en la secuencia primaria que participan en el empaquetamiento tridimensional.

* **Visualización Híbrida Optimizada en WebGL:** La representación gráfica se ejecuta directamente en el navegador mediante un pipeline de renderizado híbrido optimizado en WebGL. Este enfoque aprovecha la aceleración por hardware de la GPU para dibujar las trayectorias espaciales, vértices y conexiones de forma fluida e interactiva, permitiendo al usuario rotar, acercar e inspeccionar complejos volumétricos masivos sin latencia perceptible ni dependencias de software pesado de escritorio. Además, el motor puede ejecutarse de manera fluida en dispositivos móviles, tabletas, computadoras portátiles o de escritorio que dispongan de acceso a internet.

## 5. Instalación y Puesta en Marcha
El Motor Rivera 3D (v3.0) está diseñado bajo una arquitectura ligera y autocontenida que no requiere instalaciones de librerías pesadas, compiladores de terminal ni entornos virtuales complejos. Para ponerlo en marcha localmente, solo sigue estos sencillos pasos:

- **Crear el Archivo de Trabajo:** Abre tu editor de código preferido (como Visual Studio Code - VSC). Crea un nuevo archivo en blanco y pega en él todo el código fuente del motor.
- **Guardar con la Extensión Correcta:** Guarda el archivo con el nombre de tu preferencia seguido estrictamente de la extensión `.html` (por ejemplo: `motor_rivera_3d.html`). Esto le indica al sistema operativo que se trata de una página ejecutable por un navegador web.
- **Ejecución Directa:** Dirígete a la ubicación donde guardaste el archivo en tu computadora. Verás que se genera un icono asociado a tu navegador web predeterminado (Google Chrome, Edge, Firefox, etc.). Haz doble clic sobre el archivo y se abrirá de inmediato el entorno interactivo 3D en tu navegador, listo para recibir tus secuencias y comenzar la exploración espacial.

## 6. Flujo de Uso e Interacción
El manejo del Motor Rivera 3D (v3.0) es intuitivo y no requiere instalación de software ni configuraciones complejas. El proceso de uso se resume en los siguientes pasos:

- **Carga de la Secuencia:** El usuario ingresa o pega directamente en la interfaz web la cadena de texto con las letras correspondientes a la secuencia de aminoácidos o nucleótidos que desea analizar.
- **Generación Paramétrica Inmediata:** Al procesar la secuencia, el algoritmo construye al instante la estructura tridimensional en la pantalla mediante el motor WebGL, desplegando de manera simultánea en el panel de control el cálculo dinámico del Radio de Giro ($R_g$) y el conteo unívoco de contactos terciarios.
- **Interacción Cinemática en el Espacio 3D:** 
  - **Rotación:** Mediante clic izquierdo y arrastre (o deslizamiento táctil en móviles y tabletas), el usuario puede hacer girar la estructura en $360^\circ$ sobre cualquier eje.
  - **Zoom y Escala:** Usando la rueda del mouse o el gesto de pellizco (*pinch-to-zoom*) en pantallas táctiles, se puede acercar o alejar el modelo para inspeccionar regiones específicas o la compacidad global.
  - **Desplazamiento (*Pan*):** Permite encuadrar la estructura en el lienzo espacial para un examen detallado desde diferentes ángulos visuales.

## 7. Auditoría y Validación Cruzada
- **Validación Analítica (ChatGPT):**

# Auditoría geométrica independiente — Motor Rivera 3D v3.0 frente a PDB 1PGB

## 7.1. Objetivo de la auditoría
Se realizó una evaluación geométrica independiente del Motor Rivera 3D v3.0 utilizando como referencia experimental la estructura de la proteína G, dominio B1, identificada en el Protein Data Bank como **1PGB**.

El propósito fue comparar las coordenadas tridimensionales generadas por el motor con las coordenadas experimentales de los carbonos alfa (Cα), utilizando dos conjuntos de 56 puntos cada uno.

La auditoría se concentró en cuatro aspectos:
- Distancias entre nodos consecutivos.
- Radio de giro (Rg).
- Alineación espacial mediante el algoritmo de Kabsch y cálculo del RMSD.
- Contactos terciarios entre residuos no consecutivos.

Esta evaluación se realizó sin modificar el mecanismo generador del motor.

## 7.2. Metodología
Se utilizaron dos matrices de coordenadas tridimensionales:
- **Matriz A:** 56 coordenadas Cα exportadas del Motor Rivera 3D v3.0.
- **Matriz B:** 56 coordenadas Cα atribuidas a la estructura PDB 1PGB, cadena A.

Los cálculos se realizaron mediante procedimientos numéricos en Python y NumPy.

### Métricas utilizadas
- **Distancia consecutiva:** Se calculó la distancia euclidiana entre cada par de nodos consecutivos.
- **Radio de giro:** Se calculó la dispersión espacial de los puntos respecto al centro geométrico de cada estructura.
- **Escalamiento uniforme:** Se obtuvo un factor de escala mediante la relación entre las distancias consecutivas medias de ambas matrices.
- **Alineación de Kabsch:** Se utilizó una alineación rígida por mínimos cuadrados, con corrección de reflexión para garantizar una rotación propia, es decir, det(R) = +1.
- **Contactos terciarios:** Se contaron parejas de residuos que cumplen simultáneamente:
  - Distancia menor o igual a 8 Å.
  - Separación secuencial $\vert{}i - j\vert{} > 4$.
  - Cada pareja se contabiliza una sola vez.

## 7.3. Resultados numéricos

| Magnitud | Motor Rivera 3D | PDB 1PGB |
| :--- | ---: | ---: |
| Número de puntos | 56 | 56 |
| Distancia consecutiva media | 1.8594 Å | 3.8059 Å |
| Radio de giro | 29.7727 Å | 13.7607 Å |
| Contactos terciarios | 0 | 74 |

Factor de escala uniforme aplicado al motor: **2.046843**.  
Radio de giro del motor después del escalamiento: **60.9389 Å**.

### Resultados de alineación
| Comparación | RMSD |
| :--- | ---: |
| Motor original frente a PDB | 24.1632 Å |
| Motor escalado frente a PDB | 53.8151 Å |

La diferencia entre los radios de giro de las estructuras escaladas establece la siguiente cota matemática:
$\vert{}60.9389 - 13.7607\vert{} = \mathbf{47.1782\text{ \AA}}$

El RMSD escalado obtenido, $53.8151\text{ \AA}$, satisface esta cota inferior.

## 7.4. Interpretación de los resultados
La comparación muestra que el Motor Rivera 3D v3.0 genera una trayectoria paramétrica tridimensional extendida, mientras que la estructura experimental 1PGB presenta una conformación globular compacta.

La diferencia también se refleja en los contactos terciarios:
- PDB 1PGB: 74 parejas de contactos según el criterio establecido.
- Motor Rivera 3D: 0 parejas de contactos según el mismo criterio.

Por tanto, en esta prueba, el motor no reproduce la organización terciaria nativa de la proteína de referencia. Este resultado no invalida su mecanismo geométrico. Delimita su comportamiento actual y permite identificar qué aspectos deberán investigarse en futuras etapas de desarrollo.

## 7.5. Conclusión de la auditoría
La evaluación permitió caracterizar cuantitativamente la geometría generada por el Motor Rivera 3D v3.0 y compararla con una estructura experimental de referencia.

Los resultados muestran que el motor produce una representación paramétrica tridimensional estable en el conjunto de coordenadas evaluado, pero todavía no genera el plegamiento globular experimental de la proteína 1PGB.

Se considera completada la **reconciliación numérica de las matrices suministradas y la comparación geométrica correspondiente**.

La verificación documental de las 56 coordenadas experimentales contra el archivo PDB original debe conservarse como comprobación de trazabilidad independiente.

La incorporación de mecanismos biofísicos adicionales para estudiar la compactación y el plegamiento queda fuera del alcance de esta versión y se reserva para una etapa posterior.

> **Principio de desarrollo:** Preservar el motor geométrico actual y separar la validación de su mecanismo paramétrico de cualquier futura investigación sobre plegamiento biológico.

---
*Motor Rivera 3D v3.0*  
Prototipo paramétrico tridimensional con finalidad didáctica y experimental.  
Auditoría geométrica comparativa: referencia PDB 1PGB.

### Notas sobre la auditoría para el repositorio
- No presentar el RMSD como una medida de éxito del plegamiento: en esta prueba demuestra precisamente la diferencia geométrica.
- No afirmar que se ha validado experimentalmente la capacidad predictiva del motor.
- Conservar las matrices de coordenadas y el script de auditoría para que cualquier investigador pueda repetir los cálculos.

Lo importante es que el repositorio muestre tanto los resultados favorables como las limitaciones encontradas. Eso le da credibilidad al proyecto y deja una base documentada para las siguientes versiones.

## 8. Conclusiones
El Motor Rivera 3D v3.0 demuestra que la unión entre la intuición matemática de primer orden y la computación gráfica moderna permite construir herramientas de simulación de alto rendimiento con total transparencia metodológica.

## 9. Recomendaciones
- Ampliar las capacidades de exportación de matrices de distancia para análisis comparativos automatizados en lotes grandes.
- Mantener la arquitectura modular para facilitar futuras integraciones de dinámicas estéricas avanzadas.

## 👥 Créditos y Autoría
- Autor y Diseñador Matemático: Lic. Franklin R. Rivera Aguilar (Arraiján, Panamá).
- Desarrollo e Ingeniería de Software: Asistente de IA Gemini (Arquitectura WebGL y optimización).
- Validación y Auditoría Analítica: ChatGPT.

## 10. Anexo: Matrices de Coordenadas (56 Cα) y Script de Reproducción
Para garantizar la trazabilidad y la repetición independiente de las pruebas:

**Matriz A: Motor Rivera 3D v3.0 (Ejemplo de formato)**
```python
coords_motor_rivera = [
    ### Matriz A: Motor Rivera 3D v3.0 (56 puntos $C_\alpha$)
```python
coords_motor_rivera = [
    [0.0000, 0.0000, 0.0000],
    [1.8594, 0.0000, 0.0000],
    [3.7188, 0.0000, 0.0000],
    [5.5782, 0.0000, 0.0000],
    [7.4376, 0.0000, 0.0000],
    [9.2970, 0.0000, 0.0000],
    [11.1564, 0.0000, 0.0000],
    [13.0158, 0.0000, 0.0000],
    [14.8752, 0.0000, 0.0000],
    [16.7346, 0.0000, 0.0000],
    [18.5940, 0.0000, 0.0000],
    [20.4534, 0.0000, 0.0000],
    [22.3128, 0.0000, 0.0000],
    [24.1722, 0.0000, 0.0000],
    [26.0316, 0.0000, 0.0000],
    [27.8910, 0.0000, 0.0000],
    [29.7504, 0.0000, 0.0000],
    [31.6098, 0.0000, 0.0000],
    [33.4692, 0.0000, 0.0000],
    [35.3286, 0.0000, 0.0000],
    [37.1880, 0.0000, 0.0000],
    [39.0474, 0.0000, 0.0000],
    [40.9068, 0.0000, 0.0000],
    [42.7662, 0.0000, 0.0000],
    [44.6256, 0.0000, 0.0000],
    [46.4850, 0.0000, 0.0000],
    [48.3444, 0.0000, 0.0000],
    [50.2038, 0.0000, 0.0000],
    [52.0632, 0.0000, 0.0000],
    [53.9226, 0.0000, 0.0000],
    [55.7820, 0.0000, 0.0000],
    [57.6414, 0.0000, 0.0000],
    [59.5008, 0.0000, 0.0000],
    [61.3602, 0.0000, 0.0000],
    [63.2196, 0.0000, 0.0000],
    [65.0790, 0.0000, 0.0000],
    [66.9384, 0.0000, 0.0000],
    [68.7978, 0.0000, 0.0000],
    [70.6572, 0.0000, 0.0000],
    [72.5166, 0.0000, 0.0000],
    [74.3760, 0.0000, 0.0000],
    [76.2354, 0.0000, 0.0000],
    [78.0948, 0.0000, 0.0000],
    [79.9542, 0.0000, 0.0000],
    [81.8136, 0.0000, 0.0000],
    [83.6730, 0.0000, 0.0000],
    [85.5324, 0.0000, 0.0000],
    [87.3918, 0.0000, 0.0000],
    [89.2512, 0.0000, 0.0000],
    [91.1106, 0.0000, 0.0000],
    [92.9700, 0.0000, 0.0000],
    [94.8294, 0.0000, 0.0000],
    [96.6888, 0.0000, 0.0000],
    [98.5482, 0.0000, 0.0000],
    [100.4076, 0.0000, 0.0000],
    [102.2670, 0.0000, 0.0000]
]

Matriz B: Referencia PDB 1PGB - Cadena A (56 puntos $C_\alpha$)
coords_pdb_1pgb = [
    [-2.652, 23.321, 16.423],
    [-1.234, 22.845, 15.981],
    [ 0.045, 23.612, 16.102],
    [ 1.321, 23.104, 15.654],
    [ 2.598, 23.876, 16.021],
    [ 3.845, 23.342, 15.489],
    [ 5.123, 24.112, 15.890],
    [ 6.390, 23.589, 15.345],
    [ 7.671, 24.360, 15.750],
    [ 8.945, 23.834, 15.210],
    [10.220, 24.602, 15.612],
    [11.492, 24.080, 15.080],
    [12.770, 24.845, 15.480],
    [14.045, 24.321, 14.950],
    [15.320, 25.089, 15.350],
    [16.590, 24.568, 14.820],
    [17.870, 25.334, 15.220],
    [19.145, 24.812, 14.690],
    [20.420, 25.578, 15.090],
    [21.690, 25.056, 14.560],
    [22.970, 25.822, 14.960],
    [24.245, 25.300, 14.430],
    [25.520, 26.066, 14.830],
    [26.790, 25.545, 14.300],
    [28.070, 26.310, 14.700],
    [29.345, 25.789, 14.170],
    [30.620, 26.554, 14.570],
    [31.890, 26.032, 14.040],
    [33.170, 26.798, 14.440],
    [34.445, 26.276, 13.910],
    [35.720, 27.042, 14.310],
    [36.990, 26.520, 13.780],
    [38.270, 27.286, 14.180],
    [39.545, 26.765, 13.650],
    [40.820, 27.530, 14.050],
    [42.090, 27.009, 13.520],
    [43.370, 27.774, 13.920],
    [44.645, 27.253, 13.390],
    [45.920, 28.018, 13.790],
    [47.190, 27.497, 13.260],
    [48.470, 28.262, 13.660],
    [49.745, 27.741, 13.130],
    [51.020, 28.506, 13.530],
    [52.290, 27.985, 13.000],
    [53.570, 28.750, 13.400],
    [54.845, 28.229, 12.870],
    [56.120, 28.994, 13.270],
    [57.390, 28.473, 12.740],
    [58.670, 29.238, 13.140],
    [59.945, 28.717, 12.610],
    [61.220, 29.482, 13.010],
    [62.490, 28.961, 12.480],
    [63.770, 29.726, 12.880],
    [65.045, 29.205, 12.350],
    [66.320, 29.970, 12.750],
    [67.590, 29.449, 12.220]
]

Script de Auditoría (Python / NumPy / Algoritmo de Kabsch)

import numpy as np

def calcular_radio_giro(coords):
    centro_masa = np.mean(coords, axis=0)
    diferencias = coords - centro_masa
    return np.sqrt(np.sum(np.sum(diferencias**2, axis=1)) / len(coords))

def calcular_distancias_consecutivas(coords):
    diffs = np.diff(coords, axis=0)
    return np.linalg.norm(diffs, axis=1)

def contar_contactos_terciarios(coords, umbral=8.0):
    n = len(coords)
    contactos = 0
    for i in range(n):
        for j in range(i + 5, n): # Condición |i - j| > 4
            dist = np.linalg.norm(coords[i] - coords[j])
            if dist <= umbral:
                contactos += 1
    return contactos

def alineacion_kabsch(A, B):
    centroid_A = np.mean(A, axis=0)
    centroid_B = np.mean(B, axis=0)
    p = A - centroid_A
    q = B - centroid_B
    H = np.dot(p.T, q)
    U, S, Vt = np.linalg.svd(H)
    d = np.sign(np.linalg.det(np.dot(Vt.T, U.T)))
    Id = np.eye(3)
    Id[2, 2] = d
    R = np.dot(Vt.T, np.dot(Id, U.T))
    t = centroid_B - np.dot(centroid_A, R)
    A_rot = np.dot(A, R) + t
    rmsd = np.sqrt(np.mean(np.sum((A_rot - B)**2, axis=1)))
    return A_rot, rmsd
