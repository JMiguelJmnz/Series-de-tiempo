# Series de tiempo

Análisis exploratorio de series de tiempo para realizar pronósticos simples mediante el método de promedios móviles.

Cargamos las librerías a utilizar y cargamos los datos de IBM y Walmart
<br>![image](https://github.com/user-attachments/assets/a17fbdfe-f5db-425d-b2bc-7951b50ab67d)

Realizamos una visualización general de los datos de ambas compañias
<br>![image](https://github.com/user-attachments/assets/2e4941fe-e452-49f0-8815-faaac90cf815)

La comparación de precios entre las dos compañías muestran una tendencia similar, al no estar completamente relacionadas las compañías podria haber una influencia de una sobre la otra
<br>![image](https://github.com/user-attachments/assets/7289baf7-6977-4b3a-a52e-aa9fef19094e)

Vemos por medio de un diagrama de dispersión la correlación entre las dos compañías
<br>![image](https://github.com/user-attachments/assets/264e3437-6f2c-4fa6-98f1-314c7dd77435)

Podemos observar que existe una correlación muy débil entre las dos compañías y el diagrama de dispersión no muestra una relación clara

Realizamos la prueba de mínimos de cuadrados para obtener más información
<br>![image](https://github.com/user-attachments/assets/95d8e1f8-2029-4962-b773-16b596ecec0e)

Podemos intuir que los valores pasados tienen mucha influencia en valores futuros

Realizamos la prueba Dickey-Fuller para ambas compañías para saber si las series tienen un proceso de caminata aleatoria 
<br>H0: Se tiene un proceso de caminata aleatoria 
<br>Ha: No se tiene un proceso de caminata aleatoria
<br>![image](https://github.com/user-attachments/assets/f3d99d0c-646b-4af2-a4c2-bdd0a38d096d)

El valor para ambas compañías muestra que podemos rechazar la H0, por lo que no son estacionarias y siguen una tendencia o caminata aleatoria

Tomamos los valores diarios para realizar la descomposición para ambas compañías
<br>![image](https://github.com/user-attachments/assets/38308427-507c-475f-b357-565a8ef0ff2a)
<br>![image](https://github.com/user-attachments/assets/bae9769c-a3d7-4632-8906-fceaf2a55672)
<br>![image](https://github.com/user-attachments/assets/104e57b8-6d30-441d-9900-a2e035dd04aa)

Podemos observar como en ambas compañías la tendencia y estacionalidad se comportan de forma similar y en el caso de la tendencia, se muestra acorde a el valor de los precios a lo largo del tiempo

Realizamos un análisis gráfico de promedios moviles
<br>![image](https://github.com/user-attachments/assets/23d8ee48-faf5-4c26-86d2-f44aa6db3c49)
<br>![image](https://github.com/user-attachments/assets/78843939-50f2-4308-b477-0657a32fea03)

El pronóstico para el día siguiente de IBM es de: 254.446
<br>![image](https://github.com/user-attachments/assets/bc166cc5-23fc-4954-b173-684bf7595795)
<br>![image](https://github.com/user-attachments/assets/62c79275-1c1f-454f-a37a-db76f1f2549d)

El pronóstico para el día siguiente de Walmart es de: 98.311667
