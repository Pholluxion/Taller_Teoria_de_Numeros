# Ejercicios Teoría de Números 
## Estudiante: Carlos Daniel Peñaloza Torres  -  2172336

 **1.** Defina una función **son_congruentes(a,b,m)** cuyo output es el string **"Si!"** si <img src="https://i.upmath.me/svg/a%E2%89%A1b%5C%20mod(m)" alt="a≡b\ mod(m)" /> , **"NO!"** en caso contrario.
 
 **2.** Si <img src="https://i.upmath.me/svg/b%3E1" alt="b&gt;1" />, sabemos que dado un entero positivo <img src="https://i.upmath.me/svg/n" alt="n" />, este se puede expresar de forma única de la forma <img src="https://i.upmath.me/svg/n%3Da_kb%5Ek%2Ba_%7Bk-1%7Db%5E%7Bk-1%7D%2B%E2%8B%AF%2Ba_2b%5E2%2Ba_1b%2Ba_0" alt="n=a_kb^k+a_{k-1}b^{k-1}+⋯+a_2b^2+a_1b+a_0" /> donde <img src="https://i.upmath.me/svg/0%20%5Cleq%20a_i%20%3C%20b" alt="0 \leq a_i &lt; b" /> y <img src="https://i.upmath.me/svg/a_k%20%5Cneq%200" alt="a_k \neq 0" /> . Dicho de otra forma la expansión de <img src="https://i.upmath.me/svg/n" alt="n" /> en base <img src="https://i.upmath.me/svg/b" alt="b" /> es. 

Codifique una función **expansion(n,b)** que reciba <img src="https://i.upmath.me/svg/n%2Cb" alt="n,b" /> **enteros positivos** con <img src="https://i.upmath.me/svg/b%3E1" alt="b&gt;1" />  y que tenga como output la representación en base <img src="https://i.upmath.me/svg/b" alt="b" /> como una lista conlos valores , es decir: <img src="https://i.upmath.me/svg/%5Ba_k%2Ca_%7Bk-1%7D%2C%5Cdots%2Ca_1%2Ca_0%5D" alt="[a_k,a_{k-1},\dots,a_1,a_0]" />. Por ejemplo **expansion(12,2)** el output será **[1,1,0,0]**.
 
**3.** El Teorema Fundamental de la Aritmética menciona que todo número se puede descomponer de forma única como producto de factores primos. Por ejemplo <img src="https://i.upmath.me/svg/60%20%3D%202%5E2*3%5E1*5%5E1" alt="60 = 2^2*3^1*5^1" />. Codifique una función **factoriza(n)** que reciba un entero positivo <img src="https://i.upmath.me/svg/n" alt="n" /> y cuyo output sea un array donde la primera fila contiene los numeros primosde la factorización en orden ascendente y la segunda fila contiene las potencias correspondientes. 

Por ejemplo **factoriza(60)** el output será el **numpy array[[2,3,5],[2,1,1]]**.

Adicionalmente cree una función llamada **test(?,?,..?)** (como usted desee) que le ayude a verificar los calculos que hizo la función factoriza.

 **4.** Codifique una función **mcd(a,b)** que reciba dos enteros positivos <img src="https://i.upmath.me/svg/a%2Cb" alt="a,b" /> y cuyo output sea el valor del máximo común divisor entre <img src="https://i.upmath.me/svg/a" alt="a" /> y <img src="https://i.upmath.me/svg/b" alt="b" />.

Adicionalmente cree una función llamada **primos_relativos(a,b)** cuyo output es **"Si!"** si  <img src="https://i.upmath.me/svg/a" alt="a" /> y <img src="https://i.upmath.me/svg/b" alt="b" />  son primos relativos y **"NO!"** en caso contrario.

**5.** Codificar una función **coefs_bezout(a,b)** que reciba dos números enteros positivos  <img src="https://i.upmath.me/svg/a%2Cb" alt="a,b" />  y calcule los coeficientes de bezout. Es decir suoutput sean dos números <img src="https://i.upmath.me/svg/s" alt="s" /> y <img src="https://i.upmath.me/svg/t" alt="t" />  tales que <img src="https://i.upmath.me/svg/a*s%20%2B%20b*t%20%3D%20mcd(a%2Cb)" alt="a*s + b*t = mcd(a,b)" />.

Adicionalmente cree una función **inverso_modulo(a,m)** cuyo output es un entero: elinverso de <img src="https://i.upmath.me/svg/a" alt="a" /> en <img src="https://i.upmath.me/svg/Z_m" alt="Z_m" />.

**6.** Una raiz primitiva módulo <img src="https://i.upmath.me/svg/p" alt="p" /> (siendo <img src="https://i.upmath.me/svg/p" alt="p" /> primo) es un entero <img src="https://i.upmath.me/svg/r%20%5Cin%20Z_p" alt="r \in Z_p" />  tal que todo elemento diferente de cero en <img src="https://i.upmath.me/svg/Z_P" alt="Z_P" /> es una potencia de <img src="https://i.upmath.me/svg/r" alt="r" />. 

Codificar una función **es_raiz_primitiva(n,p)** que reciba un número entero positivo <img src="https://i.upmath.me/svg/n%20%5Cin%20Z_p" alt="n \in Z_p" /> **(o sea?)** y un número primo <img src="https://i.upmath.me/svg/p" alt="p" /> y cuyo output es **"Si!"** si es raiz primitiva módulo <img src="https://i.upmath.me/svg/p" alt="p" /> **"NO!"** en caso contrario.

**7.** Los códigos ISBN-10 son códigos de 10 dígitos  asignados por el publicador. El dígito de verificación para la identificación ISBN-10 es un dígito o la letra X (para representar el número 10). Este dígito se selecciona dela siguiente forma 

<img src="https://i.upmath.me/svg/x_%7B10%7D%20%3D%20%5Csum_%7Bi%3D1%7D%5E9ix_i(mod%5C%2011)" alt="x_{10} = \sum_{i=1}^9ix_i(mod\ 11)" />

Codificar una función **digito_verificacion(n)** que reciba los primeros nueve digitos de un código y cuyo output sea: el código de verificación ISBN-10. (Ver pag. 291 Libro Kenneth,"Discrete Mathematics and its applications")
