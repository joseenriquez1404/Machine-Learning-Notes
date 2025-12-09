## Types of Machine Learning Systems

- Aprendizaje supervisado: En el conjunto de datos de entrenamiento se le incluye al algoritmo las soluciones deseadas, las cuales son llamadas **labels**.
  - Una tarea tipica de aprendizaje supervisado es **clasificacion**
  - Otra tarea tipica es la de predecir un valor numerico **target**, dado un conjunto de caracteristicas llamadas **predictores**, esto se llama **regresion**
  - Los algoritmos mas importantes de aprendizaje supervisado son:
    - k-Nearest Neighbors
    - Linear Regression
    - Logistic Regression
    - Support Vector Machines (SVMs)
    - Decision Trees and Random Forests
    - Neural Networks
  
- Aprendizaje no supervisado: En el aprendizaje supervisado, los datos de entrenamiento no tienen las soluciones (labels).
  - Los algoritmos mas importantes son;
    - Clustering
      - K-Means
      - DBSCAN
    - Anomaly detection and novelty detection
      - One-class SVM
      - Isolation Forest
    - Visualization and dimensionality reduction
      - Principal Component Analysis (PCA)
      - Kernel PCA
      - Locally-Linear Embedding (LLE)
      - t-distributed Stochastic Neighbor Embedding (t-SNE)
    - Association rule learning
      - Apriori
      - Eclat

- Aprendizaje semisupervisado: Algunos algoritmos pueden trabajar con un conjunto de datos pacialmente etiquetado, suele tener mas datos sin etiquetado que con etiquetas. Suelen ser una combinacion de algoritmos supervisados y no supervisados.

- Aprendizaje por reforzamiento: En este caso el sistema que esta aprendiendo, llamado **agente** puede observar el ambiente, seleccionar y realizar acciones y obtener recompensas en retorno. Tiene que aprender por su propia cuenta la mejor estrategia, llamada **policy**, esta define que debe de hacer un agente cuando se le da una situacion

## Batch and Online Learning

- Batch Learning: El sistema no es capaz de aprender de manera incremental, debe ser entrenado usando todos los datos disponibles. Suele tomar mucho tiempo y usar muchos recursos de computo, se suele hacer offline. Primero se entrena y luego es lanzado a produccion. Si queremos que aprende nuevos datos se debe de volver a entrenar.

- Online Learning: Se entrena al modelo de mandera incremental, dandole informacion de manera sequencial, como individuual o mediante pequenios grupos llamados **mini-batches**. Puede ayudar a entrenar modelos los cuales tienen un dataset muy grande.
  - Un parametro muy importante es el **learning rate** el cual si es muy alto, se adaptara a nuevos datos muy rapido pero olvidara los datos antiguos y viceversa.