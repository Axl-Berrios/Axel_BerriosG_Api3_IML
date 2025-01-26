# Axel_BerriosG_Api3_IML

# Análisis de Datos del Titanic

Este proyecto se centra en el análisis de datos del Titanic utilizando un conjunto de datos que contiene información sobre los pasajeros. El objetivo principal es predecir la supervivencia de los pasajeros utilizando un modelo de árbol de decisión.

## Contenido

- Descripción del conjunto de datos
- Manejo de valores faltantes
- Preprocesamiento de datos
- Entrenamiento del modelo
- Evaluación del modelo
- Cómo ejecutar el código

## Descripción del Conjunto de Datos

El conjunto de datos del Titanic contiene las siguientes columnas:

- `PassengerId`: ID del pasajero
- `Survived`: Indica si el pasajero sobrevivió (1) o no (0)
- `Pclass`: Clase del pasajero (1, 2 o 3)
- `Name`: Nombre del pasajero
- `Sex`: Sexo del pasajero (male, female)
- `Age`: Edad del pasajero
- `SibSp`: Número de hermanos/esposas a bordo
- `Parch`: Número de padres/hijos a bordo
- `Ticket`: Número de ticket
- `Fare`: Tarifa pagada
- `Cabin`: Número de cabina
- `Embarked`: Puerto de embarque (C = Cherbourg; Q = Queenstown; S = Southampton)

## Manejo de Valores Faltantes

El código realiza las siguientes operaciones para manejar los valores faltantes en el conjunto de datos:

1. **Descripción de Valores Faltantes**:
   Se calcula la cantidad de valores faltantes para cada variable utilizando el método `isnull().sum()`.

   ```python
   print(train_df.isnull().sum())
   print(test_df.isnull().sum())
