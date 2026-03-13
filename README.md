[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/1rbxKkyt)
[![Open in Codespaces](https://classroom.github.com/assets/launch-codespace-2972f46106e565e64193e422d61a12cf1da4916b45550586e14ef0a7c637dd04.svg)](https://classroom.github.com/open-in-codespaces?assignment_repo_id=23102957)
# Ánalisis S&P500


## Integrantes

- Hernández Coutiño José de Jesús 


## Uso e instalación

Aquí escribe qué necesitas que instale para ejecutar tu código:

Se uso el código de la página proporcionada.


## Visualiza el precio de las acciones del S&P500 de los últimos 5 años, ¿dependen del precio anterior? ¿cómo argumentarías tu respuesta matemáticamente?
El precio del S&P500 muestra una dependencia temporal. Matemáticamente puede modelarse como un paseo aleatorio $P_t=P_{t-1}+\gamma_t$.La correlación entre precios consecutivos es alta eso quiere decir que el precio actual depende del precio anterior.


## Visualiza el precio de las acciones del S&P500 de los últimos 5 años, ¿los rendimientos de las acciones del S&P500 de los últimos 5 años dependen del rendimiento anterior? ¿cómo argumentarías tu respuesta matemáticamente?
A diferencia de los precios, los rendimientos del S&P500 presentan muy poca correlación. Empíricamente se observa que $Corr(r_t,r_{t-1})\approx 0$. Esto sugiere que los rendimientos se comportan como una variable aproximadamente independiente en el tiempo, consistente con la hipótesis de mercado eficiente.

## ¿Cómo intentarías predecir los rendimientos del S&P500?
Para predecir rendimientos se podrían utilizar modelos de series de tiempo como ARIMA o modelos de volatilidad como GARCH. También es posible usar regresiones con variables macroeconómicas. Pero la capacidad predictiva suele ser limitada debido a la baja autocorrelación de los rendimientos.

## ¿Debería invertir todos mis ahorros en CETES ó en el S&P500 (suponiendo que se mantiene el retorno histórico) a 1 año?
A un horizonte de 1 año, CETES ofrece menor riesgo y mayor certidumbre en el rendimiento. El S&P500 tiene un retorno esperado mayor, pero también una volatilidad significativa. Por lo que para un horizonte corto podría ser más prudente invertir en CETES.

## ¿Cambiaría tu respuesta anterior si sólo invirtieras fondos discrecionales (i.e. que su pérdida no afecta de forma sustancial tu patrimonio)?
Si el dinero y su pérdida no afecta de forma directa el patrimonio, el S&P500 puede ser una opción razonable debido a su mayor retorno esperado pero conlleva el mayor riesgo.

## ¿Cambiaría alguna de tus respuestas anteriores si el plazo aumentara de 1 año a 20 años? 
Hablando en un plazo de 20 años, históricamente el S&P500 ha superado el rendimiento de opciones libres de riesgo como CETES. Además, en horizontes largos la volatilidad relativa tiende a reducirse, por lo que la inversión en el S&P500 suele ser más atractiva.

## Conclusión
Durante los últimos cinco años se observa que los precios del S&P500 presentan dependencia temporal, ya que el precio actual está fuertemente relacionado con el precio del periodo anterior. En contraste, los rendimientos muestran un comportamiento más cercano al de una variable aleatoria independiente. Empíricamente, la autocorrelación entre rendimientos consecutivos tiende a ser cercana a cero, lo que implica que el rendimiento pasado contiene poca información útil para predecir el rendimiento futuro.

Un pequeño comentario conceptual para que lo tengas claro (esto casi nunca lo explican bien en clase): en finanzas ocurre algo curioso. Los precios parecen muy predecibles porque están correlacionados con el pasado, pero los cambios de precio (rendimientos) no lo están. Es una propiedad típica de procesos estocásticos usados en mercados, como el paseo aleatorio.

En otras palabras: el nivel del río depende del nivel de ayer, pero la subida o bajada de hoy es casi impredecible
