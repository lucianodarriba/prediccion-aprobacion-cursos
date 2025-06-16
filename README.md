# 🏠 Predicción de Precios Inmobiliarios

## 🎯 Descripción del Problema

El mercado inmobiliario es complejo y los compradores no pueden estimar con precisión el valor real de una propiedad. Esto lleva a decisiones de compra poco informadas y potenciales pérdidas económicas.

## 🔧 Solución Propuesta

Desarrollo de un modelo de Machine Learning que predice el precio de propiedades basándose en características como ubicación, tamaño, antigüedad y amenities. El modelo alcanza una precisión del **92%** en el conjunto de prueba.

## 📊 Resultados Principales

- **R² Score:** 0.92
- **Error absoluto medio:** $8,500 USD
- **Variables más importantes:** Ubicación (35%), Superficie (28%), Antigüedad (18%)

![Predicciones vs Valores Reales](images/predictions_plot.png)

## 🚀 Cómo Ejecutar el Proyecto

### 1. Clonar el repositorio
```bash
git clone https://github.com/usuario/prediccion-inmobiliaria.git
cd prediccion-inmobiliaria
```

### 2. Instalar dependencias
```bash
pip install -r requirements.txt
```

### 3. Ejecutar análisis completo
```bash
# Exploración de datos
jupyter notebook notebooks/01_exploracion.ipynb

# Entrenamiento del modelo
python src/train_model.py

# Generar predicciones
python src/predict.py --input data/new_properties.csv
```

## 📁 Estructura del Proyecto

```
├── data/
│   ├── raw/                 # Datos originales
│   ├── processed/           # Datos procesados
│   └── sample.csv          # Muestra de datos (anonimizada)
├── notebooks/
│   ├── 01_exploracion.ipynb    # Análisis exploratorio
│   └── 02_modelado.ipynb       # Desarrollo del modelo
├── src/
│   ├── data_cleaning.py        # Funciones de limpieza
│   ├── feature_engineering.py  # Creación de variables
│   ├── train_model.py          # Entrenamiento
│   └── predict.py              # Predicciones
├── images/                     # Gráficos y visualizaciones
├── README.md
└── requirements.txt
```

## 🛠️ Tecnologías Utilizadas

- **Python 3.9+**
- **Pandas** - Manipulación de datos
- **Scikit-learn** - Machine Learning
- **XGBoost** - Modelo principal
- **Matplotlib/Seaborn** - Visualizaciones
- **Jupyter** - Análisis interactivo

## 📈 Metodología

1. **Recolección de datos:** Web scraping de portales inmobiliarios
2. **Limpieza:** Tratamiento de valores faltantes y outliers
3. **Feature Engineering:** Creación de variables derivadas
4. **Modelado:** Comparación de múltiples algoritmos
5. **Validación:** Cross-validation y métricas de evaluación

## 🔍 Conclusiones y Aprendizajes

- La ubicación es el factor más determinante en el precio (35% de importancia)
- Los modelos ensemble (XGBoost) superaron significativamente a modelos lineales
- La ingeniería de características mejoró el performance en un 15%
- El modelo generaliza bien en zonas no vistas durante el entrenamiento

## 📞 Contacto

**Tu Nombre**
- LinkedIn: [tu-perfil](https://linkedin.com/in/tu-perfil)
- Email: tu.email@gmail.com
- Portfolio: [tu-website.com](https://tu-website.com)

---

⭐ Si este proyecto te resulta útil, no olvides darle una estrella al repositorio