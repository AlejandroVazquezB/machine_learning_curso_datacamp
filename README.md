# Entendiendo _Machine Learning_
_Traducido y documentado por Alejandro Vázquez B._

---
## **Introducción**

### **Cap. 1:** ¿Qué es _Machine Learning?_
---
Primero hay que hablar del termino: **Inteligencia Artifical** (IA). Hoy en día cuando la gente habla de _IA's_, suele referirse (sin saberlo) al _Machine Learning_.

La Inteligencia Artificial es un conjunto de herramientas para hacer que las computadoras tengan un "comportamiento" inteligente. Estas herramientas abarcan subcampos tales como la robótica y el _Machine Learning_.

![IA y Machine Learning](https://i.imgur.com/KwPW0uA.png)

Definir _Machine Learning_ no es una tarea sencilla, tiene muchas aplicaciones y se superpone con otros campos. Esto combinado con su exponencial crecimiento ha hecho que sus límites sean borrosos.

Nos gusta definir al _Machine Learning_ como un conjunto de herramientas que permiten realizar inferencias y predicciones a partir de datos.

Comparemos las tareas de inferencia y predicción para comprender mejor lo que puede hacer el _Machine Learning_.


---
1.1 ¿Qué puede hacer el _Machine Learning_?
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
1.2 ¿Cómo funciona el _Machine Learning_?
---
Los métodos de aprendizaje automático se basan principalmente en las las estadísticas y la informática. Es una herramienta extremadamente poderosa debido a que le brinda a las computadoras la capacidad de aprender sin ser programadas explícitamente para hacerlo. Es decir, la computadora puede aprender sin instrucciones paso a paso.
Esencialmente el aprendizaje automático aprende patrones de datos existentes y los aplica a nuevos datos. Por ejemplo, puede procesar correos electrónicos archivados para saber cómo se ve el spam por sí solo, después, usando lo que aprendió, puede detectar spam en nuevos correos electrónicos. Es necesario aclarar que para que el aprendizaje automático sea exitoso, necesita datos de alta calidad.

**En resumen:**
- Es producto de una mezcla interdisciplinaria de estadísticas e informática
- Habilidad de aprender sin ser programada para ello
- Aprende patrones de datos existentes y los aplica a nuevos datos
- Requiere datos de alta calidad


---
1.3 Relación con la ciencia de datos
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
### **Cap. 2:** Tipos de _Machine Learning_
---
Anteriormente se dijo mencionó que el _Machine Learning_ "aprende" patrones de datos existentes y los aplica a nuevos, dichos datos existentes son llamados "**datos de entrenamiento**". Cuando se está construyendo un modelo y aprendiendo de los datos de entrenamiento, lo llamamos "entrenar un modelo". Esto puede tomar desde nanosegundos, hasta semanas, dependiendo del tamaño de los datos.

Los datos de entrenamiento marcan la principal diferencia entre los tipos existentes de métodos de aprendizaje.

---
2.1 Aprendizaje Reforzado
---

  El aprendizaje reforzado es utilizado para decidir acciones secuenciales, como un robot que decide su camino o su próximo movimiento en un juego de ajedréz. No es tan común como el resto de métodos de aprendizaje y utiliza matemáticas complejas, como la teoría de juegos. El aprendizaje supervisado y el no supervisado son los más comunes.

---
2.2 Aprendizaje Supervisado
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
2.3 Aprendizaje No Supervisado
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
### **Cap. 3:** Flujo de ejecución
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


