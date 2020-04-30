
# Funções

### getSign(day, month)
Usando a função getSign(day, month) você consegue definir o Signo do Zodíaco de uma determinada data, atualmente o parâmetro **month** aceita entradas númericas e String em **en-US** (de acordo com o nome de cada mês do calendário, não sendo Case-Sensitive).

**Exemplo c/ mês Inteiro:**
```javascript
const user_sign = getSign(23, 1);
```
```Return: Aquário```

**Exemplo c/ mês String:**
```javascript
const user_sign = getSign(23, "January"); // ou "Jan"
```
```Return: Aquário```

> Obs: A função c/ String não é case-senstive. (Isto é: pode se usar: jan, january ou até JaNuarY)

------------

### returnMonth(stringMonth)
Usando a função returnMonth(stringMonth) você consegue retornar o mês em formato aceito pela função principal, atualmente é aceito **Pt-BR** e **ES**.


**Exemplo (em Português):**
```javascript
const user_month = returnMonth('Abril');
```
```Return: April```

**Exemplo (em Espanhol):**
```javascript
const user_month = returnMonth('Enero');
```
```Return: January```

------------

## Exemplo Prático:
Abaixo iremos desenvolver um simples algortmo para descobrir o signo do nosso usuário com prompt() e alert():

```javascript
var birth_day = prompt("What is the day of your birth?");
var birth_month = prompt("What is the month of your birth?");

birth_month = returnMonth(birth_month);

var user_sign = getSign(birth_day, birth_month);
alert("Your sign is: " + user_sign);
```
##### Contribua com o Signs-JS.Contribua com o Signs-JS. :tw-1f606: :tw-1f525:
