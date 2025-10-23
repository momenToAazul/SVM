# Análisis de Expresión Génica y Modelado con SVM

## Descripción

Este proyecto presenta un análisis estadístico y de modelado sobre un conjunto de datos de **expresión génica**, con el objetivo de identificar genes diferencialmente expresados entre tipos de tejido y evaluar la capacidad predictiva de modelos **SVM (Support Vector Machines)**.  

El flujo de trabajo combina enfoques de inferencia estadística y aprendizaje supervisado, integrando pruebas **t de Student**, **ANOVA** y **correcciones por pruebas múltiples** (Bonferroni, Holm y Benjamini–Hochberg), seguidas del entrenamiento de modelos con distintos kernels de SVM para clasificar las muestras.

Se buscó entender tanto la **significancia estadística de los genes** como su **utilidad en la clasificación automática**, comparando el rendimiento de diferentes configuraciones de kernel bajo un esquema controlado de entrenamiento y prueba.

---

## Contenido del proyecto

- Carga y exploración del conjunto de datos génico (`Khan.csv`).
- Cálculo de **pruebas t** entre dos clases (2 vs 4) con correcciones Bonferroni, Holm y FDR.
- Aplicación de **ANOVA** para comparar las medias de las cuatro clases.
- Identificación de genes con diferencias significativas de expresión.
- División de datos en **entrenamiento y prueba** (70/30) y escalado estandarizado.
- Entrenamiento y evaluación de tres modelos **SVM**:
  - Kernel **lineal**.  
  - Kernel **polinomial (grado 3)**.  
  - Kernel **radial (RBF)**.
- Evaluación mediante métricas de **accuracy**, **F1-macro** y **matrices de confusión**.
- Interpretación comparativa de resultados y selección del kernel más adecuado.

---

## **Documentos**  

- [Notebook editable en formato .ipynb](./A3.1_653602.ipynb)  
- [Reporte en formato .html](./A3.1_653602.html)  
- [Versión en formato .pdf](./A3.1_653602.pdf)  

---

## **Base de datos**  

- [Base de datos Khan.csv](./A3.1_Khan.csv)

---

## Referencias

- *Scikit-learn Documentation*. (2024). Support Vector Machines.  
- *Statsmodels Documentation*. (2024). Multiple testing correction methods.  
- Khan, J. et al. (2001). *Classification and diagnostic prediction of cancers using gene expression profiling and artificial neural networks.* Nature Medicine, 7(6), 673–679.

---

## Autor

**Carlos Hernández Márquez**  
Universidad de Monterrey (UDEM) · Ingeniería Mecatrónica  
Proyecto académico – Curso de Inteligencia Artificial
