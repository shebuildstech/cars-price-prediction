# Predicción del precio de un vehículo🚗
<img width="250" align="right" src="https://i.pinimg.com/564x/1c/b6/c4/1cb6c40182aa1e1decce6a13df5802f9.jpg" />


### 💡 El escenario
Tom quiere vender su automóvil. Pero el problema es que no sabe por cuánto debería venderlo. Tom quiere vender su vehículo por todo lo que pueda, pero también quiere fijar el precio razonablemente, de manera que alguien quiera comprarlo. Así que el precio que establezca debe representar el valor del vehículo.</p>
<b>¿Cómo podemos ayudar a Tom a determinar el mejor precio para su vehículo? 🤔 </b></p>
Pensemos como científicos de datos y definamos claramente algunos de sus problemas 🤓. </p> Por ejemplo, 
- ¿Hay datos sobre los precios de otros vehículos y sus características? 
- ¿Qué características de los vehículos afectan a su precio? ¿El color? ¿Marca? 
- ¿Los caballos de potencia también afectan el precio de venta, o tal vez algo más?</p>

Como analista de datos o científico de datos, estas son algunas de las preguntas en las que podemos empezar a pensar. 

#### Nota: 
Este proyecto lo desarrollé durante los laboratorios del curso [Análisis de datos con Python](https://es.coursera.org/learn/analisis-de-datos-con-python) dictado por IBM y coursera el cual finalicé en el mes de enero del 2022.

---

### 📑 Contenido:
- [Descripción de los datos](https://github.com/abloominghill/cars-price-prediction/blob/916bd57b773e6d9a479b90d12a8bdeb78221988a/Descripci%C3%B3n%20de%20los%20datos.md)
- [Data wrangling](https://github.com/abloominghill/cars-price-prediction/blob/a3a32b1304382ba1c19d49490540d723e810403e/notebooks/cars-notebook1.ipynb)
- [Análisis exploratorio](https://github.com/abloominghill/cars-price-prediction/blob/72f2d82116b2126bc9f159b02f17e3a19e6cdd59/notebooks/cars-notebook2.ipynb)
- [Desarrollo del Modelo]

--- 

### 🔍 Conclusiones del proyecto
**1. Cuál es el ritmo de consumo de combustible (L/100km) de un automóvil de diesel?** </p>
<img width="650" align="center" src="https://github.com/abloominghill/cars-price-prediction/blob/bc9a39f5fc5415c419f03bec59f181788b399465/images/consumo-diesel.jpg" /><img width="650" align="center" src="https://github.com/abloominghill/cars-price-prediction/blob/bc9a39f5fc5415c419f03bec59f181788b399465/images/diferencia-diesel.jpg" /></p>

Respecto al consumo de combustible (L/100km) de un automóvil de diesel se concluye lo siguiente:
- De las 22 marcas de carro en el conjunto de datos, solo siete tienen asociado combustible de tipo diesel.
- La marca "mercedes-benz" es la que más consume combustible por cada 100km y la marca "nissan" es la que menos consume.
- La marca "volvo" es la que menos diferencia presenta entre el consumo en la ciudad y en carretera.
- Las marcas "merces-benz" y "mazda" son las que más diferencia tienen entre el consumo en la ciudad y en carretera.
- Las marcas "toyota" y "peugot" tienen un comportamiento parecido respecto a la diferencia de consumo en la ciudad y en carretera.</p></p></p>

#    
**2. ¿Qué pasaría si solo nos ocuparamos de las diferencias de precio entre automoviles con altos, medios y pocos caballos de fuerza? ¿Podríamos reacomodarlos dentro de tres "contenedores" para facilitar el análisis?**</p>
<img width="650" align="center" src="https://github.com/abloominghill/cars-price-prediction/blob/bc9a39f5fc5415c419f03bec59f181788b399465/images/Horsepower-bins.jpg" /><img width="650" align="center" src="https://github.com/abloominghill/cars-price-prediction/blob/bc9a39f5fc5415c419f03bec59f181788b399465/images/Hpbins-price.jpg" /></p>

Respecto a las diferencias de precio entre automoviles con altos, medios y pocos horsepower se concluye lo siguiente:
- El 76.1% de los datos pertenecen a la categoría de "pocos" horsepower. 
- El 21.4% de los datos pertenecen a la categoría de "medios" horsepower.
- Tan solo el 2.5% de los datos pertenecen a la categoría de "altos" horsepower.
- Los automoviles de categoría "pocos" tienen un costo promedio de 9989.752
- Los automoviles de categoría "medios" tienen un costo promedio de 22486.465
- Los automoviles de categoría "pocos" tienen un costo promedio de 31856.600
- Respecto a lo anterior, entonces se puede decir que la potencia del vehículo influye fuertemente en su precio, aunque se presentan con mayor frecuencia los que tienen baja potencia.</p>

#      

**3. ¿Cuáles son las caracteristicas principales que más impactan en el precio de un coche?**

**- Variables númericas de correlación positiva**

- Bore: es estadísticamente significativa y la correlación con la variable precio es moderada (0.54)
  <img width="650" align="center" src="https://github.com/abloominghill/cars-price-prediction/blob/86cdcfc6d4f4bf964c496a931128bab9b08791de/images/borevsprice.jpg" />
- Wheel-base: es estadísticamente significativa y la correlación con la variable precio es moderada (0.58)
  <img width="650" align="center" src="https://github.com/abloominghill/cars-price-prediction/blob/86cdcfc6d4f4bf964c496a931128bab9b08791de/images/wheel-basevsprice.jpg" />
- Length: es estadísticamente significativa y la correlación con la variable precio es moderadamente fuerte (0.69)
  <img width="650" align="center" src="https://github.com/abloominghill/cars-price-prediction/blob/86cdcfc6d4f4bf964c496a931128bab9b08791de/images/lengthvsprice.jpg" />
- Width: es estadísticamente significativa y la correlación con la variable precio es fuerte (0.75)
  <img width="650" align="center" src="https://github.com/abloominghill/cars-price-prediction/blob/86cdcfc6d4f4bf964c496a931128bab9b08791de/images/widthvsprice.jpg" />
- Curb-weight: es estadísticamente significativa y la correlación con la variable precio es fuerte (0.83)
  <img width="650" align="center" src="https://github.com/abloominghill/cars-price-prediction/blob/86cdcfc6d4f4bf964c496a931128bab9b08791de/images/curb-weightvsprice.jpg" />
- Engine-size: es estadísticamente significativa y la correlación con la variable precio es fuerte (0.87)
  <img width="650" align="center" src="https://github.com/abloominghill/cars-price-prediction/blob/86cdcfc6d4f4bf964c496a931128bab9b08791de/images/engine-sizevsprice.jpg" />
- Horsepower: es estadísticamente significativa y la correlación con la variable precio es fuerte (0.87)
  <img width="650" align="center" src="https://github.com/abloominghill/cars-price-prediction/blob/86cdcfc6d4f4bf964c496a931128bab9b08791de/images/horsepowervsprice.jpg" />
  
**- Variables númericas de correlación negativa**

- City-mpg: es estadísticamente significativa y la correlación con la variable precio es moderadamente fuerte (-0.68)
  <img width="650" align="center" src="https://github.com/abloominghill/cars-price-prediction/blob/86cdcfc6d4f4bf964c496a931128bab9b08791de/images/city-mpgvsprice.jpg" />
- Highway-mpg: es estadísticamente significativa y la correlación con la variable precio es fuerte (-0.70)
  <img width="650" align="center" src="https://github.com/abloominghill/cars-price-prediction/blob/86cdcfc6d4f4bf964c496a931128bab9b08791de/images/highway-mpgvsprice.jpg" />

 **Nota:** Al analizar la correlación entre las viables métricas City y Highway en L/100Km la correlación da positiva.
 <img width="650" align="center" src="https://github.com/abloominghill/cars-price-prediction/blob/86cdcfc6d4f4bf964c496a931128bab9b08791de/images/city-L100kmvsprice.jpg" />
 <img width="650" align="center" src="https://github.com/abloominghill/cars-price-prediction/blob/0e67055bb780f85143ee4e48513c2b0848cac4bd/images/highway-L100kmvsprice.jpg" />
 
**- Variables catégoricas:**

- Drive-wheels: la distribución de precios entre las diferentes categorías de drive-wheels es diferente; por tanto, esta variable es buena predictora del precio.
 <img width="650" align="center" src="https://github.com/abloominghill/cars-price-prediction/blob/9ec207a6694539f5845bd9dbaacf37ea911152f3/images/drive-wheelsvsprice.jpg" />
- Las variables body-style y engine-location no son unas buenas predictoras del precio ya que, las distribución de precios entre las diferentes categorías de la primera tienen una superposición significativa y, la distribución de precios entre las diferentes categorías de la segunda son demasiado distintas.
 <img width="650" align="center" src="https://github.com/abloominghill/cars-price-prediction/blob/9ec207a6694539f5845bd9dbaacf37ea911152f3/images/body-stylevsprice.jpg" />
 <img width="650" align="center" src="https://github.com/abloominghill/cars-price-prediction/blob/9ec207a6694539f5845bd9dbaacf37ea911152f3/images/engine-locationvsprice.jpg" />




