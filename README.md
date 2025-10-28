# NLP Spam Classifier

## Descripción
Este proyecto aplica técnicas de **Procesamiento de lenguaje Natural (NLP)** para detectar si una URL es **spam** o **no_spam**
Se probaron tres modelos de Machine Learning:

1. Logistic Regression
2. Random Forest
3. XGBoost

## Estructura del proyecto

NLP_Spam_Classifier/
│
├── data/ # Dataset original (url_spam.csv)
├── notebooks/ # Notebook principal con EDA y modelos
├── scripts/ # Código modular para preprocesamiento y modelado
├── outputs/ # Resultados, gráficas y tablas
├── README.md # Documentación del proyecto
├── requirements.txt # Librerías necesarias
└── .gitignore

## Exploración de datos

Se analizó la distribución de URL's spam vs no_spam, mostrando un posible desequilibrio de clases.
Se aplicó "CountVectorizer" para transformar texto en vectores numéricos (Bag of Words).

## Modelos

| Modelo              | Precisión | Observaciones                                  |
|---------------------|-----------|------------------------------------------------|
| Logistic Regression | ~0.95     | Rápido y simple, buen baseline                 |
| Random Forest       | ~0.97     | Robusto, captura relaciones no lineales        |
| XGBoost             | ~0.98     | mejor desempeño general, requiere más recursos |

## Conclusiones
- Los modelos de ensemble (Random Forest, XGBoost) superan al lineal.
- El proyecto puede ampliarse con TF-IDF o embeddings.
- ideal para integración en pipelines de seguridad web.

## Autor
Proyecto desarrollado por Angel Reséndiz Plata<br>
    LinkedIn: [www.linkedin.com/in/angel-resendiz-plata](www.linkedin.com/in/angel-resendiz-plata)
