# Milk_quality_prediction




¿Cuál es el desafío?

**Apoyar** a empresas del rubro de la leche y sus         derivados, por medio de la **implementación de       modelos de aprendizaje automático de clasificación supervisada, para hacer predicciones de la calidad de la leche** basándose en algunas características del      producto.


¿Cuáles son los datos disponibles?

Información obtenida sobre conjunto de datos limpios (1.059 filas y 8 columnas)

- Objetivo: nivel de calidad de la leche en categorías.
  - Baja →  40,5%
  - Media →  35,3%
  - Alta → 24,2%
- Características: relacionadas al producto.
1. pH → numérica [3-9,5]
1. Temperatura → numérica [34-90] °F
1. Sabor → nominal [0: No óptimo ó 1: Óptimo]
1. Olor →  nominal [0: No óptimo ó 1: Óptimo]
1. Grasa →  nominal [0: No óptimo ó 1: Óptimo]
1. Turbidez →  nominal [0: No óptimo ó 1: Óptimo]
1. Color → numérico [240-255] en escala de grises
- Fuente de datos: <https://www.kaggle.com/datasets/cpluzshrijayan/milkquality>

¿Qué muestran los datos sobre la calidad de 

la leche y sus características?

1 2![](Aspose.Words.fc323d74-1433-47a2-bc57-43149ae36282.003.png)![](Aspose.Words.fc323d74-1433-47a2-bc57-43149ae36282.004.png)![](Aspose.Words.fc323d74-1433-47a2-bc57-43149ae36282.005.png)![](Aspose.Words.fc323d74-1433-47a2-bc57-43149ae36282.006.png)![](Aspose.Words.fc323d74-1433-47a2-bc57-43149ae36282.007.png)

1. Mayor dispersión del pH y temperatura en leche de baja calidad.
1. Mayor dispersión del color en leche de calidad media.

la leche y sus características?

1 ![](Aspose.Words.fc323d74-1433-47a2-bc57-43149ae36282.008.png) ![](Aspose.Words.fc323d74-1433-47a2-bc57-43149ae36282.009.png)![](Aspose.Words.fc323d74-1433-47a2-bc57-43149ae36282.010.png)![](Aspose.Words.fc323d74-1433-47a2-bc57-43149ae36282.011.png)![](Aspose.Words.fc323d74-1433-47a2-bc57-43149ae36282.012.png)![](Aspose.Words.fc323d74-1433-47a2-bc57-43149ae36282.013.png)

2 ![](Aspose.Words.fc323d74-1433-47a2-bc57-43149ae36282.014.png) ![](Aspose.Words.fc323d74-1433-47a2-bc57-43149ae36282.015.png) ![](Aspose.Words.fc323d74-1433-47a2-bc57-43149ae36282.016.png)![](Aspose.Words.fc323d74-1433-47a2-bc57-43149ae36282.017.png)![](Aspose.Words.fc323d74-1433-47a2-bc57-43149ae36282.018.png)![](Aspose.Words.fc323d74-1433-47a2-bc57-43149ae36282.019.png)![](Aspose.Words.fc323d74-1433-47a2-bc57-43149ae36282.020.png)

La leche de calidad “Media y alta”, medida según         parámetros de Sabor, Olor, Grasas y Turbiedad óptimos se agrupa a temperaturas <50°F (10 °C) y pH Neutro (6-7).


Resultados de la predicción de calidad Desempeño ML



|**Modelo**|**accuracy**|**precision**|**recall**|**AUC**|
| - | - | - | - | - |
|**Árbol de decisiones**|**0,990**|**6 1,000**|**0 0,976**|**7 0,988**|
|Árbol de decisiones (max\_Depth=3)|0,990|6 1,000|0 0,976|7 0,988|
|Bagging|0,990|6 1,000|0 0,976|7 0,988|
|Bagging (n\_estimators=20)|0,990|6 1,000|0 0,976|7 0,988|
|RandomForest|0,990|6 1,000|0 0,976|7 0,999|
|RandomForest (n\_estimators=20)|0,990|6 1,000|0 0,976|7 0,991|
|KNN (n\_neighbors=5)|0,984|3 1,000|0 0,961|2 0,988|
|KNN (n\_neighbors=4 weights=uniform)|0,984|3 1,000|0 0,961|2 0,988|
|LogisticRegression|0,833|3 0,822|0 0,751|9 0,895|
|LogisticRegression\_penalty\_l1\_C\_1|0,839|6 0,836|2 0,751|9 0,895|
Aplicando el criterio de selección de >accuracy, >precisión, >recall y >AUC **Árbol de decisiones**

Conclusiones y recomendaciones

**Para apoyar a empresas del rubro leche y derivados**, por medio de la implementación de modelos de aprendizaje automático de clasificación supervisada, para hacer predicciones de la calidad de la leche basándose en algunas características del producto. **Se recomienda lo siguiente**:

- Utilizar modelo de **Árbol de decisiones** para predecir calidad de la leche.
- Enriquecer el conjunto de datos con nuevas características del producto, como por ejemplo: **tipo de envase, fecha de producción, tipo de procesamiento de la leche, origen geográfico**, entre otras.
- Aplicar la técnica a otros productos lácteos, tales como: **mantequilla, quesos, yogur, cremas, entre otros**.






![Diapositiva1](https://user-images.githubusercontent.com/106708017/194420992-f0404c44-ed19-4ba7-a331-5d73aaa9d3a3.JPG)
![Diapositiva2](https://user-images.githubusercontent.com/106708017/194420997-928932b9-263f-4054-a111-39f57c54bf5e.JPG)
![Diapositiva3](https://user-images.githubusercontent.com/106708017/194420998-3aa588a3-ff06-4eb8-ba74-0918fb89bc51.JPG)
![Diapositiva4](https://user-images.githubusercontent.com/106708017/194421002-b12932fa-a497-48d8-bf71-91699905d421.JPG)
![Diapositiva5](https://user-images.githubusercontent.com/106708017/194421003-ceafdcd7-03b2-4847-ac32-902813e542c1.JPG)
![Diapositiva6](https://user-images.githubusercontent.com/106708017/194421004-a71cf032-6739-4ff4-9ce7-a1af234ca034.JPG)
![Diapositiva7](https://user-images.githubusercontent.com/106708017/194421007-d62493fd-d606-49e2-865e-ecb0cf74aa89.JPG)
![Diapositiva8](https://user-images.githubusercontent.com/106708017/194421011-1591d124-742a-4a2b-a54a-0f3f7dadc79e.JPG)
![Diapositiva9](https://user-images.githubusercontent.com/106708017/194421013-533ed750-9da6-472c-96b7-3fc1d6534f12.JPG)



















