---
Index: "[[Calculo Aplicado]]"
---
---
# OBJETIVOS DE APRENDIZAGEM

➢ Identificar e esboçar gráficos de funções elementares de uma variável
real: funções constantes, potência, afim, quadrática, exponencial,
logarítmicas e trigonométricas.
➢ Construir gráficos de funções utilizando movimentação gráfica.
➢ Identificar e construir gráfico de funções definidas por várias sentenças.
➢ Analisar gráfico de funções definidas por várias sentenças e reconhecer os
limites laterais, limites e continuidade no ponto, limites infinitos e no
infinito.

# INTRODUÇÃO

<span style="font-weight:bold; color:rgb(192, 0, 0)">O Cálculo Diferencial e Integral</span> é um ramo importante da matemática, desenvolvido a partir da Álgebra e da Geometria. Foi desenvolvido por Isaac Newton (1643-1727) e Gottfried Leibniz (1646-1716) simultaneamente em trabalhos independentes.

<span style="font-weight:bold; color:rgb(192, 0, 0)">O Cálculo Diferencial e Integral</span> é a base para o curso de computação e afins, muitas funções são implementadas com bases matemáticas, essas operações auxiliam a entende a variação de condições matemática de situações reais com relação as mudanças dessas próprias condições.

Limites é uma teoria matemática que estuda o comportamento das funções para valores próximo de um número dado.

Exemplo: Suponha que um físico deseja obter determina medida quando a pressão do ar é zero. Como, no laboratório, é extremamente difícil obter a pressão exatamente igual a zero, isto é, vácuo perfeito. O físico deverá obter medidas a pressões cada vez menores. Se, quando as pressões tendem para zero, as medidas correspondentes tendem para um número n, então ele concluirá, naturalmente, que se a pressão for zero, o valor da medida será n.

# NOÇÃO INTUITIVA DE LIMITE – LIMITES LATERAIS

Seja a função ***f*: R -> R**, definida por *f*(x) = x + 4. Vamos dar valores a **x** que se aproximem de 1, pela sua direita ( valores maiores que 1) e pela esquerda (valores menores que 1)  e calcular o valor correspondente de **y**:

|  **x**   |    **y = x +4**     |
| :------: | :-----------------: |
| **0,5**  |  y = 0,5 + 4 = 4,5  |
| **0,7**  |  y = 0,7 + 4 = 4,7  |
| **0,9**  |  y = 0,9 + 4 = 4,9  |
| **0,95** | y = 0,95 + 4 = 4,95 |
| **0,98** | y = 0,98 + 4 = 4,98 |
| **0,99** | y = 0,99 + 4 = 4,99 |

|  **x**   |    **y = x +4**     |
| :------: | :-----------------: |
| **1,5**  |  y =1,5 + 4 = 5,5   |
| **1,3**  |  y = 1,3 + 4 = 5,3  |
| **1,1**  |  y = 1,1 + 4 = 5,1  |
| **1,05** | y =1,05 + 4 = 5,05  |
| **1,02** | y = 1,02 + 4 = 5,02 |
| **1,01** | y = 1,01 + 4 = 5,01 |

- o limite de f(x), quando x tende a 1, pela esquerda, é igual a 5 ou, abreviadamente:
$$
\\lim_{ x \to \ 1^- \\ } f(x) = 
$$
- o limite de f(x), quando x tende a 1, pela direita, é igual a 5 ou, abreviadamente:
$$
\\lim_{ x \to \ 1^+ \\ } f(x) = 
$$
Estes dois limites são chamados de limites laterais. Quando existirem os limites laterais e forem iguais, dizemos que existe o limite de f(x) quando x tende para 1 e escrevemos, simplesmente:
$$
\\lim_{ x \to \ 1 \\ } f(x) = 
$$
De forma geral, escrevemos:

$$
\\lim_{ x \to \ a \\ } f(x) = b
$$

se, quando x se aproxima de a (x ->a), f(x) se aproxima de b (f(x) -> b).

O limite de uma função existe se e somente se os limites laterais existirem e forem iguais.
Simbolicamente:
$$
\lim_{ x \to \ a \\ } f(x) = \left\{ \frac{x^2 + x - 2}{\underset{\text{2, se x=1}}{x - 1}} \right\}, \quad x \neq 1
$$

# Propriedades dos limites de Funções

Ao definir limite, chegou-se à expressão $\lim_{ n \to a } f(x)=b$. Sejam as funções $f(x)$ e $g(x)$, definidas em certos domínios D, tais que $\lim_{ x \to a}f(x)=L  \text{ e}\lim_{x \to a} g(x)=M$
A seguir, estão descritas algumas propriedades que auxiliam à obtenção de b.

## 1) Limite de uma constante
O limite de uma constante é a própria constante.
$$ \lim_{n \to a} k = k $$
$$\text{Exemplo:}\lim_{x \to 2} 3 = 3$$
## 2) Limite da soma
O limite da soma de duas funções é a soma dos limites dessas funções
$$\lim_{ n \to a } [f(x) + g(x)] = \lim_{n \to a} f(x) + \lim_{n \to a} g(x) = L +M$$Exemplo:
$$\lim_{x \to 1}[x^3 + 3x^3] = \lim_{ x \to 1 } x^3 + \lim_{ x \to 1 } x^3 = 1+3=4$$

CONTINUAAAAAAAAAAAAAR