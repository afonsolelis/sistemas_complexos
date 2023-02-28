27.03.2023

Os sistemas complexos aumentam a complexidade com aumento do sistema?

## Modelo de Dinâmica Populacional (Euler 1748)

Euler tentou prever (criar) um modelo de crescimento de habitantes em Berlin

x * (t + Delta.t) = x * (t) + nascimento - morte + imigração - emigração
`sendo x a população em número de habitantes`

x * (t + Delta.t) = x(t) + (n * x(t) * Delta.t) - m * x(t) * Delta.t
`n e m (nascimento e morte) é uma constante positiva`

isolando o n (constante de nascimento)

n = (x(t) * Delta.t - x(t))/(Delta.t + x(t)) = (260 / 1 min) * (1/8*10^9)
m = (x(t) - x(t + Delta.t))/(Delta.t * x(t)) = (130/1 min) * (1/8*10^9)

*Adotando um Delta de 1 unidade de tempo*

Delta.t = 1
x(t + 1) = x(t) + nx(t) - mx(t)
x(t + 1) = (1 + n - m) * x(t) *q = m - n*
x(t + 1) = (1 + q) * x(t) *Mi = 1 + q*
x(t + 1) = Mi * x(t) --> Progressão Geométrica

*ou seja* - Resolvendo a equação

x(1) = Mi * x(0) --> t = 0,1,2,...
x(2) = Mi * x(1) --> Mi^2 * x(0)
x(3) = Mi * x(2) --> Mi^3 * x(1)
...
x(t) = x(0) * Mi ^ t

# Solução Estacionária

x(t + 1) = x(t) = x ^ a

_então_

x^a = Mi * x^a
x^a - Mi * x^a = 0
(1 - Mi) * x^a = 0 --> x^a = 0

# Estabilidade de x^a

Para 0 < Mi < 1

------------------- x^a = 0 -------------------- x(0) -------------------
