# Practica-tema-5
# Modelo 3D simplificado: Burney Relief - Queen of the Night

Este repositorio forma parte de la práctica del Tema 5 del Módulo 2 del curso sobre Digitalización del Patrimonio Cultural. El objetivo ha sido crear, simplificar, texturizar y publicar un modelo 3D a partir de una nube de puntos proporcionada.

## 👤 Autora
**Carolina Padilla Martínez**

## 🖼️ Modelo seleccionado
**burney_relief_queen_of_the_night.ply**

Este modelo representa un bajorrelieve mesopotámico conocido como "Burney Relief" o "Queen of the Night".
---
## 🔧 Proceso seguido

1. **Triangulación:**  
   Se realizó la reconstrucción de superficie a partir de la nube de puntos utilizando el filtro `Surface Reconstruction: Poisson` en MeshLab. Se generó una malla con normales válidas y caras cerradas.

2. **Simplificación:**  
   Se aplicó el filtro `Quadric Edge Collapse Decimation` para reducir el número de vértices a menos de 10.000 (conservando las proporciones y los detalles esenciales del relieve).

3. **Parametrización UV:**  
   Se realizó la parametrización de la malla con el filtro `Parameterization: Trivial Per-Triangle`.

4. **Creación de textura:**  
   A partir del color por vértice de la malla original, se generó una textura para el modelo simplificado mediante el filtro `Transfer: Vertex Attributes to Texture`.
