En este repositorio evaluaremos la posibilidad de supervivencia del Titanic con un árbol de decisión. Para ello, usaré la famosa base de datos de posibilidad de supervivencia al impacto del Titanic, modificada por un usuario de Kaggle (https://www.kaggle.com/datasets/heptapod/titanic). En esta, tenemos las siguientes variables:

. Passangerid: id de cada pasajero
. Age: edad de cada pasajero
. Fare: precio ticket
. Sex: sexo del pasajero: 0 = Hombre, 1 = Mujer
. sibsp: número de hermanos/cónyuges a bordo
. Parch: número de padres/hijos a bordo
. Pclass: clase del ticket: 1 = Upper, 2 = Middle, 3 = Lower.
. Embarked: puerta de embarque: 0 = Cherbourg, 1 = Queentown, 2 = Southampton.
. 2urvived: si sobrevivió: 0 = No, 1 = Si.

Luego de aplicar 'ctree' del paquete 'party' y hacer la matriz de confusión, en la cual indica los errores de acierto del modelo, obtenemos con 78% de precisión que todas las mujeres sobrevivien, así como los hombres con ticket de clase 'middle' o 'lower' de 4 años o menos, mientras que los hombres mayores a 4 años, independientemente de la clase del ticket, mueren.
