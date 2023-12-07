# Entendiendo _Machine Learning_
_Traducido y documentado por Alejandro Vázquez B._

## **Introducción**

## **Capítulo 1:** ¿Qué es _Machine Learning?_


Para entender qué es el _Machine Learning_ primero hay que hablar del termino: **Inteligencia Artifical** (IA). Hoy en día cuando la gente habla de _IA's_, suele referirse (sin saberlo) al _Machine Learning_.

La Inteligencia Artificial es un conjunto de herramientas para hacer que las computadoras tengan un "comportamiento" inteligente. Estas herramientas abarcan subcampos tales como la robótica y el _Machine Learning_.

![IA y Machine Learning](https://i.imgur.com/KwPW0uA.png)

Definir _Machine Learning_ no es una tarea sencilla, tiene muchas aplicaciones y se superpone con otros campos. Esto combinado con su exponencial crecimiento ha hecho que sus límites sean borrosos.

Nos gusta definir al _Machine Learning_ como un conjunto de herramientas que permiten realizar inferencias y predicciones a partir de datos.

Comparemos las tareas de inferencia y predicción para comprender mejor lo que puede hacer el _Machine Learning_.


---
### 1.1 ¿Qué puede hacer el _Machine Learning_?
---

- **Predice** eventos futuros:
    - Lloverá mañana?
        - Sí (75% de probabilidad) 

- **Infiere** las causas de los eventos y comportamientos:
    - Por qué llueve?
        - Época del año, humedad, temperatura, ubicación, etc.

- **Infiere** patrones:
    - Cuáles son los diferentes tipos de condiciones climáticas?
        - Lluvias, días soleados, neblina, etc.


Estas tareas pueden trabajar juntas porque las inferencias ayudan a hacer predicciones, sin embargo, requieren diferentes tipos de aprendizaje automático.


---
### 1.2 ¿Cómo funciona el _Machine Learning_?
---
Los métodos de aprendizaje automático se basan principalmente en las las estadísticas y la informática. Es una herramienta extremadamente poderosa debido a que le brinda a las computadoras la capacidad de aprender sin ser programadas explícitamente para hacerlo. Es decir, la computadora puede aprender sin instrucciones paso a paso.
Esencialmente el aprendizaje automático aprende patrones de datos existentes y los aplica a nuevos datos. Por ejemplo, puede procesar correos electrónicos archivados para saber cómo se ve el spam por sí solo, después, usando lo que aprendió, puede detectar spam en nuevos correos electrónicos. Es necesario aclarar que para que el aprendizaje automático sea exitoso, necesita datos de alta calidad.

**En resumen:**
- Es producto de una mezcla interdisciplinaria de estadísticas e informática
- Habilidad de aprender sin ser programada para ello
- Aprende patrones de datos existentes y los aplica a nuevos datos
- Requiere datos de alta calidad


---
### 1.3 Relación con la ciencia de datos
---
La ciencia de datos se trata de descubrir y comunicar información a partir de los datos. El aprendizaje automático suele ser una herramienta importante para el trabajo de ciencia de datos, especialmente para hacer predicciones a partir de datos.

![Ciencia de datos y Machine Learning](https://i.imgur.com/Lp1Qp9a.png)

---
1.4 Modelos de _Machine Learning_
---
Un modelo de aprendizaje automático es una representación estadística de un proceso del mundo real, como la forma en que reconocemos a los gatos o los cambios de hora en el tráfico.

Un proceso se modela utilizando datos. El modelo recibe datos de entrada que lo alimentan y éste crea una salida.

![Modelo ML](https://i.imgur.com/PlIIvok.png)

Por ejemplo, si hacemos un modelo basado en datos históricos de tráfico, podemos ingresar una fecha futura en el modelo para predecir qué tan pesado será el tráfico mañana por la tarde. 

![Modelo ML](https://i.imgur.com/noFs5V9.png)


---
### 1.5 Tipos de aprendizaje
---
Anteriormente se dijo mencionó que el _Machine Learning_ "aprende" patrones de datos existentes y los aplica a nuevos, dichos datos existentes son llamados "**datos de entrenamiento**". Cuando se está construyendo un modelo y aprendiendo de los datos de entrenamiento, lo llamamos "entrenar un modelo". Esto puede tomar desde nanosegundos, hasta semanas, dependiendo del tamaño de los datos.

Los datos de entrenamiento marcan la principal diferencia entre los tipos existentes de métodos de aprendizaje.

---
#### 1.5.1 Aprendizaje Reforzado
---

  El aprendizaje reforzado es utilizado para decidir acciones secuenciales, como un robot que decide su camino o su próximo movimiento en un juego de ajedréz. No es tan común como el resto de métodos de aprendizaje y utiliza matemáticas complejas, como la teoría de juegos. El aprendizaje supervisado y el no supervisado son los más comunes.

---
#### 1.5.2 Aprendizaje Supervisado
---
Nos gustaría entrenar un modelo para predecir si un paciente tiene una enfermedad cardíaca, por lo que se capturan registros existentes de pacientes que han experimentado dolores en el pecho y han sido examinados para detectar enfermedades del corazón. Nuestra variable objetivo (_target objective_) es "_Heart Disease_" (enfermedad cardíaca), porque esto es lo que queremos predecir.

![Datos de entrenamiento para técnica de aprendizaje supervisado](https://i.imgur.com/q8z54Ck.png)

Los valores "True" y "False" son etiquetas (_labels_) para la variable objetivo, indican si un paciente tiene o no una enfermedad cardíaca. Las etiquetas no tienen que estar en ese formato, podrían ser números o categorías.

![Datos de entrenamiento para técnica de aprendizaje supervisado objetivo](https://i.imgur.com/1Edquyo.png)


![Datos de entrenamiento para técnica de aprendizaje supervisado etiqueta](https://i.imgur.com/Okv9mQk.png)

Las filas son las observaciones o ejemplos de los que aprenderá nuestro modelo, deberíamos obtener tantas como sea posible.

![Datos de entrenamiento para técnica de aprendizaje supervisado filas](https://i.imgur.com/Kkxa9Iw.png)


Y estas columnas, son "características" (_features_), las características son diferentes piezas de información que pueden ayudar a predecir el objetivo. La edad, el colesterol y los hábitos de fumar son factores conocidos de enfermedades del corazón.

![Datos de entrenamiento para técnica de aprendizaje supervisado características](https://i.imgur.com/dPYXq7H.png)

La magia del aprendizaje automático es que podemos analizar muchas características  a la vez, incluso aquellas de las que no estamos seguros, y encontrar relaciones entre diferentes características.

Ingresamos etiquetas y características para entrenar el modelo y una vez que se realiza el entrenamiento, podemos darle al modelo una nueva entrada. En nuestro caso, un nuevo paciente.

![Datos de entrenamiento para técnica de aprendizaje supervisado nueva entrada](https://i.imgur.com/KVi1PPg.png)

Las características alimentan el modelo y a su vez, el modelo genera su predicción.

![Datos de entrenamiento para técnica de aprendizaje supervisado nueva entrada](https://i.imgur.com/xiR1MlI.png)

Es así como funciona esta técnica de aprendizaje automático, utilizando datos existentes de entrenamiento "etiquetados" para alimentar el modelo y en función a dichas etiquetas, se realiza una predicción de nuestro objetivo. Por ejemplo, sabíamos si los pacientes anteriores tenían enfermedades del corazón en función de las etiquetas "True" y "False".

---
#### 1.5.3 Aprendizaje No Supervisado
---

A diferencia del **Aprendizaje Supervisado**, el **Aprendizaje No Supervisado** no se vale de etiquetas, sino únicamente de las características.
Por lo general, tareas como la detección de anomalías y la agrupación (_clustering_), que divide los datos en grupos según la similitud. Exploremos esto con nuestro conjunto de datos.

Existen diferentes tratamientos para las enfermedades del corazón, diferentes tipos de pacientes responden mejor o peor a determinados tratamientos. Podemos utilizar el **Aprendizaje No Supervisado** para comprender los diferentes tipos de pacientes que tenemos.

Filtremos nuestro conjunto de datos para incluir sólo los pacientes con enfermedades cardíacas. Podemos pasarlo a un modelo de agrupamiento y obtener categorías de pacientes basadas en la similitud de características.

![Datos de entrenamiento para técnica de aprendizaje supervisado agrupamiento](https://i.imgur.com/tMGrgEH.png)

Por ejemplo, una categoría podría ser pacientes con colesterol alto y nivel de azúcar en la sangre de un cierto rango de edad. Tenga en cuenta que no conocíamos estas categorías e, incluso, la cantidad de categorías antes de ejecutar esto. Con esta salida podemos agrupar pacientes e investigar mejores tratamientos para cada grupo.

Ahora, con un nuevo paciente, podemos ingresar las características en el modelo y obtener el tipo de paciente en el que encajan mejor.

![Datos de entrenamiento para técnica de aprendizaje supervisado después del entrenamiento no supervisado](https://i.imgur.com/3f6baPV.png)

En realidad, los datos no siempre vienen con etiquetas, o es demasiado trabajo manual etiquetar o ni siquiera sabemos qué son las etiquetas. Piense en el esfuerzo que supondría etiquetar millones de imágenes de carreteras para coches autónomos, es ahí es cuando brilla el **Aprendizaje No Supervisado**.

En este sentido, el modelo no está supervisado y encuentra sus propios patrones.

---
### 1.6 Flujo de trabajo
---

Hasta ahora, sabemos que los datos de entrenamiento se usan para permitir que un modelo aprenda, luego ese modelo s epuede usar para hacer predicciones pero, **¿cuáles son los pasos intermedios?**

A continuación se presentará el flujo de ejecución del aprendizaje automático, que son cuatro pasos para construir un modelo.

Seguiremos los pasos con el siguiente escenario:
NYC publica sus registros mensuales de todos los apartamentos vendidos en la ciudad, incluye información sobre:

- Metros cuadrados del apartamento
- Nombre del vecindario
- Año de construcción
- Precio de venta
- etc.

Supongamos que queremos predecir el precio al que se venderán los apartamentos, por lo que  nuestro objetivo será el precio de venta. Dado que tenemos estas etiquetas podemos darnos cuenta de que se trata de un problema de Aprendizaje Supervisado, veamos su flujo de trabajo.

### Flujo de trabajo:
1. **Extraer características**
   
   Los conjuntos de datos normalmente no vienen con características claras, por lo que hay trabajo por hacer para reformatear el conjunto de datos. Además, debe decidir con qué características desea comenzar. En nuestro caso, mencionamos algunos como: metros cuadrados, vecindario, año, precio, etc. Sin embargo, hay más que podrían afectar a nuestro objetivo, como la distancia a la estación de metro más cercana.
  
2. **Dividir el conjunto de datos**
   
   Se divide en dos conjuntos de datos:
     1. Datos de prueba
     2. Datos de entrenamiento
  
        ![Paso 3 Entrenar el modelo](https://i.imgur.com/uAkTfGD.png)

3. **Entrenar el modelo**
   
   Para esto, el conjunto de datos del tren se ingresa en un modelo de aprendizaje automático elegido.
   
   ![Paso 3 Entrenar el modelo](https://i.imgur.com/iyparDW.png)

    Existen varios modelos diferentes de aprendizaje automático para elegir con diferentes casos de uso y niveles de complejidad, desde una red neuronal hasta una regresión logística.

4. **Evaluación**
   
    No podemos asumir que el modelo será funcional, entonces, ¿cuál sería la mejor manera de evaluar el modelo? En este caso, nos gustaría alimentar al modelo con las características conocidas de apartamentos vendidos y ver con qué precisión predice el precio de venta. No queremos utilizar ningún dato usado para entrenar el modelo, porque le modelo ya ha visto esos datos, esto es exactamente para lo que es el conjunto de datos de prueba creado en el paso 2.

    ![Paso 4 evaluar el modelo](https://i.imgur.com/MpNKvl5.png)
    
    Alimentamos al modelo con el conjunto de datos de prueba, también conocidos como "datos ocultos" (_unseen data_), y esperamos las predicciones del modelo.
    Hay muchas maneras de evaluar el rendimiento de nuestro modelo, por ejemplo, podríamos calcular el error medio de las predicciones o el porcentaje de los precios de venta de apartamentos que se pronosticaron con precisión dentro de un margen del 10%.
    Cualquiera que sea el método que se elija, se debe decidir un umbral de rendimiento. Por ejemplo, supongamos que nuestro modelo predice con precisión el 80% de los apartamentos, aquí surge la pregunta obligatoria: **¿Es mi modelo lo suficientemente bueno?**, en caso de obtener una respuesta afirmativa el modelo está listo para usarse, en el caso contrario habría que volver a entrenar el modelo y aplicar ciertas modificaciones (_tunes_), dicha smodificaciones puede significar un par de cosas diferentes, por ejemplo, ajustar las opciones o características del modelo.

    ![Paso 4 evaluacion de eficacia](https://i.imgur.com/f0OQgLC.png)

    Ajustar el modelo puede llevar un tiempo y si el rendimiento no mejora, muchas veces significa que no tiene suficientes datos.

    ![Paso 4 modelo final](https://i.imgur.com/IDUMOHV.png)

Esos son los 4 pasos del flujo de trabajo.

#### En resumen:
1. Extraer características
   - Elegir las características y manipular el conjunto de datos
  
2. Dividir el conjunto de datos
   - Dividirlo en dos conjuntos:
       1. datos para entrenamiento
       2. datos para pruebas

3. Entrenar el modelo
   - Entrenar el modelo con el conjunto de datos de entrenamiento creado en el paso 2 y un modelo de aprendizaje

4. Evaluar el modelo
   - Si el modelo no cumple con las expectativas, hay que aplicar "_tunearlo_" y repetir el paso 3 hasta obtener los resultados deseados.

---
## **Capítulo 2: Métodos de Aprendizaje del _Machine Learning_**

2.1 Aprendizaje Supervisado
---

El aprendizaje supervisado es básicamente una máquina de etiquetado, toma una observación y le asigna una etiqueta.

Hay dos métodos de aprendizaje supervisado: 
1. **Clasificación:** consiste en asignar una categoría a una observación, estamos prediciendo una variable discreta, una variable que sólo puede tomar unos cuantos valores diferentes.
   - "¿Este cliente detendrá su suscripción?"
     - Sí, No.
   - "¿Qué clase de vino es este?"
     - Rosado, Tinto, Blanco.
   - "¿Qué flor es esa?"
     - Rosa, Clavel, Tulipán.
   
   Por ejemplo, de la siguiente table tomemos las admisiones universitarias donde queremos predecir la aceptación. Para simplificar, mostramos dos características: GPA y Resultados de la Prueba (_Test Results_).

   ![MLS clasificación](https://i.imgur.com/0LrT84I.png)

   Se podría tener más funciones, como: participación en organizaciones estudiantiles, deportes o premios que hayan ganado los solicitantes, etc.

   El objetivo es lo que queremos prececir y hay dos etiquetas posibles _True_ o _False_, que quiere decir, si son aceptados en la universidad o no.

   ![MLS objetivo](https://i.imgur.com/5sETjqX.png)

   El objetivo sólo puede contener una de esas dos etiquetas, lo que lo convierte en un problema de clasificación.

   A continuación se muestran las observaciones trazadas:

   ![MLS grafico estado de solicitudes](https://i.imgur.com/Ne5fLcM.png)
   _Gráfica sobre los aspirantes aceptados y no aceptados por la universidad._

   Los puntos azules representan a los solicitantes aceptados, los puntos rojos representan a los solicitantes rechazados.
   Mantenemos el 80% de nuestros datos para entrenar nuestro modelo.

   ![MLS grafico clasificación manual de de solicitudes](https://i.imgur.com/mLO3SZ3.png)
   _Grafico clasificación manual de solicitudes de aspirantes_

   Debido a que sólo usamos dos funciones, podemos trazar e interpretar los resultados. Para nosotros, los humanos, es bastante claro; el gráfico demuestra que si se obtiene un puntaje superior a 4 tanto en el GPA como ne la prueba de ingreso, es aceptado. Si agregaramos más funciones como extracurriculares o premios, necesitaríamos más ejes y sería muy díficil para nosotros interpretar los datos con nuestro ojo humano. Sin embargo, un modelo no lucharía en lo absoluto. Podríamos usar una máquina de soporte de vectores, suena temible, pero sólo es una línea que separa nuestros puntos. Así entrenamos nuestro algoritmo y clasificamos el 20% de las observaciones que dejamos de lado.

   ![MLS grafico máquina de soporte de vectores - clasificación líneal de solicitudes de aspirantes](https://i.imgur.com/epxOcX8.png)
   _Grafico máquina de soporte de vectores: clasificación líneal de solicitudes de aspirantes_.
   
   Sólo clasifica errónamente dos puntos azules como rojos, lo que significa que se predijo erróneamente que dos solicitantes fueran rechazados.
   
   El problema es que intenta separarse con una línea recta, por lo que es poco probable que lo haga mejor que eso, pero, ¿Qué pasaría si permitimos una línea curva? Hay maneras para modificar el comportamiento de un modelo, como permitir curvas, por ejemplo:

   ![MLS grafico máquina de soporte de vectores - clasificación polinomial de solicitudes de aspirantes](https://i.imgur.com/nUhxL6u.png)
   _Grafico máquina de soporte de vectores: clasificación polinomial de solicitudes de aspirantes_

   ¡Ahora clasifica todo correctamente!


2. **Regresión:** Asigna una variable continua que puede tomar cualquier valor. Por ejemplo:
   - ¿Cuánto valdrá esta acción?
   - ¿Qué tan alto será ese niño cuando crezca?
   - ¿Cuál será la masa de éste exoplaneta?

   Para ejemplificar utilicemos lecturas meteorológicas para predecir la temperatura:

   ![MLC tabla lecturas meteorológicas](https://i.imgur.com/mzL5cpi.png)
   
   ¿Podemos predecir la temperatura en función del porcentaje de humedad?, usamos el 80% de los datos para entrenar nuestro modelo. Parece que cuando sube la humedad, baja la temperatura.

   ![MLC gráfica de evolución de la temperatura basada en la humedad](https://i.imgur.com/U5IdryN.png)
   _Gráfica de evolución de la temperatura basada en la humedad_

   De hecho, nuestro modelo de regresión lineal capta esto:

   ![MLC gráfica de evolución de la temperatura basada en la humedad](https://i.imgur.com/GpPpj1Z.png)
   
   ![MLC gráfica de evolución de la temperatura basada en la humedad 2](https://i.imgur.com/i0iySQG.png)
   _Gráficas regresión líneal sobre la evolución de la temperatura basada en la humedad_

   Según nuestro modelo, si el índice de humedad es 0.5, entonces la temperatura es de 18.5 C°.

   Y es así como se comporta el modelo en datos reales. Identificó la tendencia, pero sigue siendo malo para predecir. Más características como el viento, nubosidad, ubicación, temporada, entre otras; podrían hacerlo más preciso.
  
   #### En resumen:
   - Regresión == Valores Continuos
     - Cualquier valor finito (altura) o intervalo infinito (tiempo) 
       - Una temperatura exacta: 20 C°, 18 C°, 45 C°...
   
   - Clasificación == Etiquetas de Categorías
     - Uno de unos cuantos valores específicos
       - Frío, templado, caluroso...
     - Bebé, niño, adolescente, adulto...

**El método de aprendizaje supervisado debe ser elegido a conciencia, considerando si desea enmarcar un problema como el problema como uno de regresión o uno de clasificación.**

---
2.2 Aprendizaje No Supervisado
---

El Aprendizaje No Supervisado es bastante similar al Aprendizaje Supervisado, excepto que no tiene como objetivo una columna específica, de ahí la parte no supervisada.

### Entonces, ¿cúal es el punto?
Lo que vuelve realmente interesante y poderoso al Aprendizaje No Supervisado es que aprende del conjunto de datos e intenta encontrar patrones, es decir, podemos encontrar información sin saber muhco sobre nuestro conjunto de datos, lo que lo hace ideal para tratar con cantidades enormes de datos díficiles de interpretar a _"ojo de buen cubero"_.



### 2.2.1 Aplicaciones
Puede tener diversas aplicaciones, principalmente la agrupación, detección de anomalías y asociaciones. 

#### Agrupación (_clustering_)
Consiste en identificar grupos en su conjunto de datos. Las observaciones en estos grupos comparten similitudes más fuertes con miembros de su grupo, que con miembros de otros grupos.

Por ejemplo, dígamos que tenemos un conjunto de datos con seis observaciones, ¿Qué grupos detectaría el algoritmo?

![Aprendizaje No Supervisado: Agrupacion de especies](https://i.imgur.com/7e14qlW.png)
_Ejemplo del conjunto de datos_

Es una pregunta cuya respuesta depende de diversos factores.

Del conjunto de datos original pueden surgir dos grupos: "Perros" y "Gatos".

![Aprendizaje No Supervisado: Agrupacion de especies por raza](https://i.imgur.com/ipq5lvJ.png)

O bien, podría hacer cuatro grupos por color: negro, gris, blanco y café.

![Aprendizaje No Supervisado: Agrupacion de especies por color](https://i.imgur.com/M1xHCWD.png)

También podría agrupar los elementos del conjunto de datos por país origen, en este caso: "Europa" y "Japón".

![Aprendizaje No Supervisado: Agrupacion de especies por nacionalidad](https://i.imgur.com/mT5ZFZX.png)

Se ha ejemplificado lo que representa cada grupo, sin embargo, en la práctica no se suele tener conocimiento sobre qué diferencia a los _clústeres_ (grupos); el modelo no le dirá por qué o cómo se decidió formar los grupos. Dependerá de usted investigar y averiguarlo.

**Modelos de _clustering_**
- _K Means_:
  - Requiere especificar de antemano el número de clústeres que le gustaría identificar
- DSCAN _(density-based spatial clustering of applications with noise)_:
  - No requiere que especifique el número de clústeres por adelantado. En cambio, requieren que defina qué constituye un grupo, como el número mínimo de observaciones en un grupo.
  
Dígamos que tenemos flores de especies desconocidas y todo lo que conocemos es su ancho y largo del pétalo:

![ANS Dataset](https://i.imgur.com/ZdlF7S4.png)

Ahora el problema de clasificación se vuelve visible. Aquí no tenemos una columna con etiquetas de la especie, ni siquiera sabemos con cuáles y cuántas especies estamos hay.

Si planteamos la hipótesis de que hay 4 especies, podemos usar _K Means_ y requerir 4 _clusters_ distintos.

![ANS K-Means 4 clusters](https://i.imgur.com/fbZCRki.png)

 Si suponemos que hay 3 especies, necesitamos 3 _clusters_ diferentes. Estos grupos son realmente correctos, ya que hay tres especies en el conjunto de datos: _Setosa, Virginica_ y _Versicolor_.

 ![ANS K-Means 3 clusters](https://i.imgur.com/CGy1itt.png)


 #### Detección de anomalías
La detección de anomalías consiste en detectar valores atípicos _(outliers)_.
Los valores atípicos son observaciones que difieren bastante del resto. En la siguiente imagen, todos los puntos están agrupados en la parte inferior izquierda, excepto uno en la parte superior derecha.

![ANS Detección de Anomalías](https://i.imgur.com/EbXwLX0.png)

Resulta que ese pinto es la suma total de las otras observaciones , la fila total no se eliminó antes de trazar los datos. En este caso, eliminar del conjunto de datos (_dataset_) el valor atípico nos permitiría apreciar de mejor manera el gráfico, tal como se muestra a continuación.

![ANS Detección de Anomalías 2](https://i.imgur.com/RrmNrRM.png)

Con dos dimensiones, es sencillo encontrar valores atípicos a simple vista. Intente encontrar valores atípicos e 3 dimensiones; eso podría ser factible, pero, ¿qué tal 4, 10, 20, 100?, es por eso que necesitamos métodos de aprendizaje no supervisados.

En el ejemplo anterior tratamos la anomalía como un error, pero las anomalías no deben ser tratadas siempre como errores, su detección nos permitiría, por ejemplo, descubrir qué dispositivos fallan más rápido que otros, descubrir personas mal intencionadas que vulneran un sistema o algún paciente que sorprendentemente sea resistente a una enfermedad mortal. La detección de anomalías permite descubrir cualquier evento poco común en cualquier tipo de contexto.

#### Asociación
La asociación nos permite encontrar relaciones entre datos observados. En otras palabras, se trata de encontrar eventos que suceden juntos.

Un uso común de esta característica es el análisis del un carrito de compras virtual, que se trata únicamente de "¿Qué objetos se compran juntos?".

![ANS Asociación: carrito de compras](https://i.imgur.com/H2xUTHt.png)

Por ejemplo, es probable que las personas que compran mermelada compren pan, las personas que compran  cerveza compre bótanas y las personas que compren vino probablemente compren queso.


#### En resumen
- Aprendizaje No Supervisado = Análisis sin un objetivo específico
  - Sin gúia
  - Análiza el conjunto de datos en su totalidad
  - Intenta detectar patrones
  - Agrupa las observaciones con función en lo que se le solicite
  - Detecta anomalías en las observaciones
  - Asocia las observaciones entre sí

---
2.3 Evaluación del rendimiento
---

Recordemos el paso 4 del flujo de trabajo.

![Paso 4 modelo final](https://i.imgur.com/IDUMOHV.png)

Lo primero que se busca evaluar es el _overfitting_ (sobreajuste). Es **cuando nuestro modelo funciona muy bien con los datos de entrenamiento, pero mal con los datos de prueba.** 

Cuando esto ocurre significa que nuestro modelo aprendió el entrenamiento establecido de memoria y es incapaz de aplicar los aprendizajes a nuevos _datasets_, que es lo que originalmente queríamos. Es por ello que necesitamos dividir nuestro conjunto de datos en dos conjuntos.


Por ejemplo, la línea verde aquí se sobreajusta, haciendo todo lo posible para clasificar los puntos perfectamente, por lo tanto, funciona muy bien en este conjunto de datos, pero deficientemente en datos no vistos.

![ER: overfitting ejemplo](https://i.imgur.com/WqD3R7H.png)

La línea negra comete más errores en ese _dataset_, pero generaliza mejor.

#### _Accuracy_ (precisión)
En el ejemplo de la aceptación universitaria, ¿cómo mediríamos el desempeño del modelo? Podríamos usar la precisión (_accuracy_), que es el número de las observaciones clasificadas correctamente (OCC) divididas entre la cantidad total de observaciones (CTO).

***_Accuracy_ = OCC / CTO***

![ER: Accuracy](https://i.imgur.com/6CmiXMM.png)

Sin embargo, la precisión no es siempre la mejor métrica para evaluar el rendimiento de un modelo.

Considere el fraude donde sólo una pequeña minoría de transacciones son fraudulentas. Dígamos que entrenenamos un modelo para predecir si una transacción es fraudulenta o legítima.

Aquí hay un gráfico que muestra su rendimiento en 30 puntos de datos de prueba:

![ER: Limite de la precisión - ejemplo de fraude](https://i.imgur.com/SI8QJeI.png)

_Limite de la precisión: ejemplo de fraude_

Sólo clasifica erróneamente 2 puntos, lo que le da una precisión de alrededor del 93%, lo que suena bien. Pero el modelo en realidad pasa por alto la mayoría de las transacciones fraudulentas, lo cual sería un problema si implementamos éste modelo en el mundo real. Incluso podemos decir que todos los puntos son legítimos y obtendríamos una precisión del 90%, pero no detectamos a todos los estafadores.

Para subsanar estos conflictos se introdujo la matríz de confusión.

#### Matriz de Confusión

En el ejemplo, se predijo una transacción fraudulenta que en verdad era fraudulenta, de manera que se agrega un 1 a la matriz donde la columna Valores actuales 


|             ||          Valores Actuales          | Valores Actuales|
| --          | --              | --                | --              |
|             |                 | Fraudulentos      | No Fraudulentos |
| Predichos   | Fraudulentos    | 1                 |         0       |
| Predichos   | No Fraudulentos | 2                 |         27      |

![ER: Matriz de confusión](https://i.imgur.com/Pr2YeB9.png)

#### Interpretación de la matriz
- Los **Verdaderos Positivos**, son puntos clasificados correctamente. En este caso, sólo hay un punto fraudulento clasificado correctamente como fraudulento en el área roja.

- Los **Falsos Negativos** so observaciones fraudilentas que se clasifican incorrectamente como legítimas. En este caso se han clasificado 2, representadas por los 2 puntos rojos en el área azul.
Los Falsos negativos son como decirle a una mujer embarazada que no está embarazada

- Los **Falsos positivos** son observaciones legítimas que se clasifican incorrectamente como ilegítimas. En este caso hay 0.

- Los **Verdaderos Negativos** son observaciones legítimas predichas clasificadas correctamente como legítimas en la predicción. En este caso hay 27 puntos legítimos predichos correctamente como no fraudulentos.

  Si sumamos todos los cuadrangulares de la matriz se debería obtener el total de observaciones, que en este caso es de 30 puntos.

#### Sensibilidad (_Sensitivity_)
Recordemos que estábamos en busca de una métrica que funcionara mejor que la presición (_accuracy_) para medir el rendimiento de nuestro modelo en nuestro caso específico de fraude, y es aquí donde entra en juego la **sensibilidad**. Esta valora la predicción precisa de transacciones fraudulentas específicamente valorando más los verdaderos positivos.

**Fórmula de la Sensibilidad**

| Sensibildad |
| --          |
|Sensibilidad = Verdaderos Positivos / (Verdaderos Positivos + Falsos Positivos)|
|![ER: formula sensibilidad](https://i.imgur.com/BOhKuMk.png)|
|*_No es necesario aprenderla de memoria_*|
||

En este caso obtuvimos una sensiblidad del 33%, la cual es una mala puntuación. **Optimizar la sensiblidad significa que preferimos marcar transacciones legítimas como sosopechosas antes que autorizar transacciones fraudulentas.**

Ahora vemos que nuestro modelo no es bueno para predecir el fraude y necesita mejoras. 

#### Especifidad (_Specificity_)
Por otro lado tenemos la **especifidad** que valora los verdaderos negativos.

**Fórmula de la Especifidad (_Specificity_)**

| Especifidad |
| --          |
|Especifidad = Verdaderos Negativos / (Verdaderos Negativos + Falsos Positivos)|
|*_No es necesario aprenderla de memoria_*|
||

Esta es una métrica útil para los filtros de spam. Para un usuario es preferible enviar correo no deseado a la bandeja de entrada principal, antes que enviar correos reales a la carpeta de correo no deseado.

Esa es la clasificación.

---
### Evaluación de la Regresión
Esencialmente, queremos la diferencia entre el valor real y el valor predicho. Esta puede ser la distancia entre los puntos y la línea predicha.

![ER: Evaluacion de la regresión](https://i.imgur.com/P61Afdp.png)

Hay varias formas de calcular este error, como el error cuadrático medio, pero esta es la idea general.

---

#### ¿Y qué sucede con el Aprendizaje No Supervisado?
Recuerde que éste no tiene variables predichas, por lo que no hay una salida correcta con la que comparar. El rendimiento de su modelo de aprendizaje no supervisado depende del problema que esté resolviendo. Por lo tanto, usted evalúa el desempeño en función de qué tan bien los resultados avanzan en su objetivo inicial.

---
2.4 Mejorando el desempeño
---

Ahora que ya sabes cómo elegir entre clasificación, regresión o técnicas de aprendizaje no supervisado y cómo evaluar sus resultados.

Después de evaluar nuestro modelo, tenemos que decidir si el rendimiento es lo suficientemente bueno.

![2.4 MD diagrama](https://i.imgur.com/uZGfJxn.png)

Existen varias opciones para mejorar su modelo en caso de que no esté satisfecho con su rendimiento, pero nos centraremos en tres.

---
####  **2.4.1 Reducción de la dimensionalidad**

**Dimensión:** Una dimensión denota la cantidad de características (_features_) en sus datos.

| Técnica | Funcionamiento |
| ------- | -------------- |
Reducción de la<br>dimensionalidad | Elimina características completamente irreleventes. Demuestra que más información no es siempre mejores predicciones.

**Ejemplo**  
Para predecir cuánto tiempo nos tomará llegar a la oficina; la hora del día y el clima son factores interesantes, pero es poco probable que la cantidad de vasos que bebimos ayer sea muy útil.

![2.4.1 ejemplo](https://i.imgur.com/sLfijXB.png)

Algunas características pueden estar altamente correlacionadas y llevar información similar, podríamos mantener una sola característica y agún tener la mayor parte de la información.
Por ejemplo, la altura y el tamaño de un zpato están altamente correlacionados. Es muy probable que las personas altas tengan una talla de zapatos grande.  
También podríamos colapsar varias funciones en una sola función subyacente. Si tenemos dos características, como la altura y el peso podríamos calcular una característica de índice de masa corporal en su lugar.

---
#### **2.4.2 Ajuste de Hiperparámetros**

**Hiperparámetro:**  
Es un parámetro, del modelo, que uno elige antes de comenzar su entrenamiento.

antes de comenzar el entrenamiento.
Un modelo de aprendizaje automático es como una consola de producción musical, dependiendo de si estás mezclando música _pop_, _rap_ o _heavy metal_ se deben aplizarlos ajustes pertinentes a los instrumentos y la voz.  
Algunos ajustes sonarán mejor con ciertos géneros que con otros. Bueno, en nuestro caso, el género es el conjunto de datos y la configuración de los instrumentos son los hiperparámetros. Dependiedo del _dataset_, diferentes valores de hiperparámetros´darán mejores o peores resultados.

|Técnica | Funcionamiento|
|--------|---------------|
|Ajuste de <br> hiperparámetros|Se trata de personalizar los ajustes específicamente para los requerimientos del modelo de aprendizaje automático.|

**Ejemplo**  
Cuando entrenamos la SVM en la primera lección del capítulo, cambiamos de una línea recta a una curva.

![MLS grafico máquina de soporte de vectores - clasificación líneal de solicitudes de aspirantes](https://i.imgur.com/epxOcX8.png)

![MLS grafico máquina de soporte de vectores - clasificación polinomial de solicitudes de aspirantes](https://i.imgur.com/nUhxL6u.png)

Eso es porque ajustamos el hiperparámetro "nucleo" de "lineal" a "polinomio"

<p align = "center">

|_kernel: 'linear' --> 'poly'_|
|----|
</p>

Hay muchos más hiperparámetros que se pueden ajustar en el modelo SVM:
* C
* degree
* gamma
* shrinking
* coef-
* tol
* ...

Jugar con diferentes valores para cada hiperparámetro afectará el rendimiento de nuestro modelo. No tienes que adivinar combinaciones al azar, hay combinaciones estructuradas maneras de encontrar los valores óptimos, pero eso está fuera del alcance de este curso.

---

#### **2.4.3 Métodos de conjunto**

|Técnica| Funcionamiento |
|----|----|
|Métodos de Conjunto|La última opción que queremos cubrir son los métodos de conjunto. Esto es una técnica que combina varios modelos para producir un modelo óptimo.|

<br>

Imagina que estamos usando tres modelos diferentes: A, B y C.  

![MD 2.4.3 metodos de conjunto](https://i.imgur.com/wM14YVj.png)

En un entorno de clasificación, usaríamos la votación. Si el modelo A y C dicen que el estudiante es aceptado y el modelo B dice que no, entonces se acepta la observación, ya que fue la predicción más común entre todos los modelos.  

![MD 2.4.3 metodos de conjunto 2](https://i.imgur.com/bisCq8E.png)

En una configuración de regresión, usamos el promedio. Si el modelo A predice una temperatura de 5°, el modelo B una temperatura de 8° y el Modelo C una temperatura de 4°, a la observación se le asigna el valor promedio 5.67°

![MD 2.4.3 metodos de conjunto 3](https://i.imgur.com/20iQH06.png)  

---

---