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
