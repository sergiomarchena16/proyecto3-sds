# Proyecto 3 - Ataques a modelos de Deep Learning
 Sergio Marchena - UVG 2022 - Security Data Science
 
 ## Parte 1 - Ataque de extracción 
 
![Alt text](1.1.png?raw=true "Title: Ataques CopycatCNN")

En la grafica se puede ver la comparacion de el ataque CopycatCNN para ambos modelos, el orginal y uno protegido. Se puede ver que la accuracy baja considerablemente usando un modelo protegido, de aproximandamente 90% a menos del 80%. Esto es totalmente esperado y se podría decir que el modelo protegido funciona. 

![Alt text](1.2.png?raw=true "Title: Ataques KnockoffNets")

Ahora bien, para la comparacion entre el atque de KnockoffNets para ambos modelos. Tambien se aprecia un rendimiento mejor para el modelo protegido, incluso mucho mejor que CopycatCNN. El accuracy baja de mas de 90% a menos de 75%. Esto es una respuesta esperada. Se podria decir que el modelo robado de KnockoffNets es más efectivo que CopycatCNN en este caso. 

 ## Parte 2 - Ataque de evasión 
 
 ![Alt text](2.png?raw=true "Title: Modelo Original vs Robusto")

Se puede ver que el clasificador robusto tuvo mejores predicciones correctas a pesar del ataque de evasionn FGM. Siempre tuvo mas de 1200 observaciones correctas, lo cual es el 85% de la data. Mientras que el modelo original es muy susceptible a confundirse, ya que paso de tener mas de 1300 predicciones correctas a tener menos de 300, lo cual es muy bajo y peligroso. Esto solo representa el 21% de la data. 

**¿Cómo podría proteger su modelo ante este tipo de ataques?**

Se puede mejorar o proteger el modelo entrenandolo de mejor manera y usando mas capas o diferentes capas de protección. Como se puede ver en la gráfica, un modelo protegido funcionana mucho mejor. 
