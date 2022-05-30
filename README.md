# Proyecto 3 - Ataques a modelos de Deep Learning
 Sergio Marchena - UVG 2022 - Security Data Science
 
 ## Parte 1 - Ataque de extracción 
 
![Alt text](1.1.png?raw=true "Title: Ataques CopycatCNN")

Como se observa en la grafica, en los atques probabilisticos, el ataque CopycatCNN tuvo una mejor accuracy que el KnockoffNets. Ahora bien, en los ataques no probabilisticos (argmax), los resultados son muy similares. Pero KnockoffNets es un poco mejor.

![Alt text](1.2.png?raw=true "Title: Ataques KnockoffNets")

Se puede observar que en los dos casos de ataques, el accuracy del modelo baja considerablemente con la capa de proteccion. En el caso de CopycatCNN baja de 0.9 aprox hasta 0.8 aprox. Y en KnockoffNets, baja de mas de 0.9 aprox hasta 0.75 aprox. Esto es un comportamiento totalmente esperado. 

 ## Parte 2 - Ataque de evasión 
 
 ![Alt text](2.png?raw=true "Title: Modelo Original vs Robusto")

Se puede ver que el clasificador robusto tuvo mejores predicciones correctas a pesar del ataque de evasionn FGM. Siempre tuvo mas de 1200 observaciones correctas, lo cual es el 85% de la data. Mientras que el modelo original es muy susceptible a confundirse, ya que paso de tener mas de 1300 predicciones correctas a tener menos de 300, lo cual es muy bajo y peligroso. Esto solo representa el 21% de la data. 

**¿Cómo podría proteger su modelo ante este tipo de ataques?**

Se puede mejorar o proteger el modelo entrenandolo de mejor manera y usando mas capas o diferentes capas de protección. Como se puede ver en la gráfica, un modelo protegido funcionana mucho mejor. 
