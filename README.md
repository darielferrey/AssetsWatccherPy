# AssetsWatcherPy

Programa sencillo utilizando la biblioteca yfinance para obtener precios de criptomonedas y acciones de bolsa. Graficado con streamlit y pandas

## Descripción del Proyecto

Este programa le permite al usuario investigar sobre el precio de una criptomoneda o acción en la bolsa de Estados Unidos durante todo el tiempo que ha estado público, pudiendo ver las variaciones que ha tenido y como se ha comportado desde el primer día hasta la fecha y hora actual.

- **yfinance**: Como la librería principal y encargada de mediante una API obtener en tiempo real el precio de un determinado activo en Yahoo Finance
- **Streamlit**: Para mostrar los gráficos de precios de criptomonedas y acciones de manera visual y amigable
- **Pandas**: Para el manejo de los datos


## Características Principales

1. **Fácil de Usar**: Hecha de forma que resulta al usuario muy intuitiva, ya que se basa en botones y a base de clics.
3. **Interfaz Gráfica Interactiva**: Selección entre las diferentes opciones, fechas en el calendario o incluso saber el precio con solo poner encima de la gráfica en un punto determinado el cursor.
4. **Resultados Detallados**: Muestra la gráfica con los precios a la cual se le puede hacer "zoom" para verlo lo más detallado que se desee.

## Cómo Funciona

1. El usuario elige si desea saber acerca de una criptomoneda o de una acción.
2. Luego elige la fecha inicial desde la que desea comenzar a ver el precio.
3. Selecciona entre las criptomonedas/acciones la que desea visualizar.
4. La librería yfinance se encarga de obtener los precios de la API.
5. Se grafican todos los resultados con streamlit.

## Instrucciones de Uso

1. Se debe correr como un proyecto en streamlit. Abriendo el terminal, navegar al directorio donde se encuentra el script de Python y luego escribir streamlit run nombre_de_tu_proyecto.py
2. En caso de que el nombre contenga espacios streamlit run "nombre de tu proyecto.py"
3. Seguir los pasos del 1 al 3 de la sección "Cómo funciona"
4. Si se hace scroll dentro de la gráfica puede moverse desde el año hasta la hora de un día específico. Todo depende que tan preciso se busque un resultado.


## Notas Adicionales

1. Funciona para todas las acciones de Yahoo Finance (lo que se resume a la gran mayoría de las que existen). En el caso de que se quiera buscar una que no está en el programa solo es necesario buscar el símbolo de la acción (la notación con que se escriben) y agregarla en la lista de acciones del script.
2. Pasa exactamente lo mismo con las criptomonedas con el único cambio de que hay que poner el nombre (símbolo de la criptomoneda) y -USD seguido ya que como las criptomonedas se analizan mayormente con un par Fiat (dinero común ((USD, EUR...)) ) hay que escribirlo así para ver la paridad que tiene con el dólar en cuanto a precio.
3. El calendario en el script tiene fecha 2014 porque solo deja seleccionar en un rango de 20 años por lo que va de 2004 a 2024 (Año actual), pero si se le da clic al lado del número en la fecha y se escribe manual por el teclado funciona con cualquier fecha que se ponga sin importar el rango inicial. 
