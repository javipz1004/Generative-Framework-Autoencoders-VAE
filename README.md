# Generative Framework: Autoencoders & VAEs

Este repositorio explora el aprendizaje no supervisado mediante la implementación de arquitecturas de codificación y generación de datos sobre el dataset **Fashion-MNIST**.

## Proyectos Incluidos

### 1. Denoising Autoencoder (DAE)
Implementación de un autocodificador diseñado para la reconstrucción de imágenes y eliminación de ruido.
- **Aprendizaje de Identidad:** Capacidad de comprimir la entrada en un espacio latente de dimensiones reducidas.
- **Robustez:** Entrenamiento con factor de ruido para forzar a la red a aprender características estructurales de las prendas.
- **Visualización:** Análisis de la topología del espacio latente mediante **t-SNE**.



### 2. Variational Autoencoder (VAE)
Uso de modelos generativos probabilísticos para la creación de nuevas muestras.
- **Espacio Latente Estocástico:** En lugar de mapeos deterministas, el VAE aprende distribuciones gaussianas ($\mu, \sigma^2$).
- **Pérdida de Divergencia KL:** Regularización del espacio latente para permitir una interpolación suave.
- **Interpolación de Prototipos (Morphing):** Generación de transiciones visuales entre diferentes clases (ej. de sandalia a bota).



## Estructura
- `notebooks/`: Implementaciones detalladas en PyTorch.
- `images/`: Visualizaciones de mapas t-SNE e interpolaciones.

## Resultados Visuales
El modelo VAE permite navegar por el espacio latente, demostrando que prendas similares se agrupan geográficamente, lo que facilita la generación de "híbridos" mediante morphing.

---
**Autor:** Francisco Javier Pérez Cazorla  
*Proyecto académico para la asignatura de Programación para la Inteligencia Artificial.*
