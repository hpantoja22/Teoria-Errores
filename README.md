[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=hpantoja22/Teoria-Errores)

# Teoria de Errores y Cifras Significativas con Series de Maclaurin

## Autor
Dr. Hermes Yesser Pantoja Carhuavilca.

# Enunciado

La **serie de Maclaurin** es una representación de funciones en forma de una suma infinita de términos calculados a partir de las derivadas de la función en un punto específico (en este caso, $0$ ). La serie de Maclaurin para la función \(\cos ⁡(x) \) está dada por:

$$\cos (x)=\sum_{n=0}^{\infty } \frac{(-1)^n x^{2n} }{(2n)!}$$

Queremos aproximar el valor de $\cos ⁡(x)$ utilizando un número finito de términos de esta serie.


**Datos:**

-  Valor de $x=0.3\pi$ 
## Objetivo
1.  Determinar el **número mínimo de términos** necesarios en la serie de Maclaurin para aproximar $\cos ⁡(0.3\pi )$ con **9 cifras significativas**.
2. Implementar esta aproximación en **MATLAB** utilizando un **Live Script**.
3. Utilizar un **slider interactivo** para visualizar cómo el número de términos afecta la precisión de la aproximación.
4. Calcular y visualizar el **error relativo** asociado a cada aproximación.
## Conceptos Teóricos
### Serie de Maclaurin para $\cos (x)$ 

La serie de Maclaurin es una expansión en serie de una función en torno a $x=0$ . Para la función $\cos (x)$ , la serie de Maclaurin está dada por: 

 $$ \cos (x)=\sum_{n=0}^{\infty } \frac{(-1)^n x^{2n} }{(2n)!}=1-\frac{x^2 }{2!}+\frac{x^4 }{4!}-\frac{x^6 }{6!}+\cdots $$ 

 Esta serie se utiliza para aproximar el valor de $\cos (x)$ utilizando un número finito de términos.

### Cifras Significativas y Error Relativo

Cuando realizamos aproximaciones numéricas, es importante evaluar cuán preciso es el resultado obtenido. Las **cifras significativas** son los dígitos en un número que contribuyen a su precisión. Para determinar si una aproximación tiene $n$ cifras significativas, utilizamos el concepto de **error relativo**. El  **error relativo**  $\delta_r$ se define como: 

 $$ \delta_r =\left|\frac{\textrm{Valor}\;\textrm{real}-\textrm{Valor}\;\textrm{aproximado}}{\textrm{Valor}\;\textrm{real}}\right| $$ 

Para que una aproximación tenga $n$ cifras significativas, el error relativo debe cumplir con la siguiente condición:

 $$ \delta_r \le 5\times 10^{-n} $$ 

Por ejemplo, para obtener **8 cifras significativas**, el error relativo debe ser menor o igual a $5\times 10^{-8}$ .

## Preguntas

¿Cuántos términos de la serie de Maclaurin se requieren para aproximar $\cos (0.3\pi )$ con una precisión de 9 cifras significativas?

1.  Desarrolle un script en MATLAB que:

-  Calcule la aproximación de $\cos ⁡(0.3\pi )$ usando la serie de Maclaurin con el número mínimo de términos encontrado. 
-  Calcule el **error relativo** de la aproximación. 
-  Incluya un **slider interactivo** que permita variar el número de términos de la serie y observe cómo afecta la aproximación y el error relativo. 
-  Presente los resultados de manera clara y concisa, mostrando el valor aproximado y el error relativo correspondiente. 

