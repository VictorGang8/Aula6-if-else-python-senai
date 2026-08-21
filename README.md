# Atividades de Estruturas Condicionais em Python

Este repositório reúne exercícios introdutórios de **estruturas condicionais em Python**, utilizando `if`, `elif`, `else`, operadores relacionais e operadores lógicos.

## Objetivos

- Compreender o funcionamento de `if`, `elif` e `else`;
- Aplicar operadores relacionais em condições;
- Utilizar o operador módulo (`%`);
- Combinar condições com operadores lógicos;
- Desenvolver pequenos programas interativos em Python.

## Pré-requisitos

- Python 3 instalado;
- Editor de código, como Visual Studio Code, PyCharm ou IDLE;
- Conhecimentos básicos sobre variáveis, entrada e saída de dados.

## Como executar

1. Salve o código da atividade desejada em um arquivo com a extensão `.py`;
2. Abra o terminal na pasta onde o arquivo foi salvo;
3. Execute o programa com o comando:

```bash
python nome_do_arquivo.py
```

---

## Atividade 1: Classificação de número

### Objetivo

Utilizar estruturas condicionais com `if`, `elif` e `else`.

### Descrição

Crie um programa que solicite um número ao usuário e verifique se ele é:

- Positivo;
- Negativo;
- Nulo, quando o valor for igual a zero.

### Código

```python
numero = float(input("Digite um número: "))

if numero > 0:
    print("O número é positivo.")
elif numero == 0:
    print("O número é nulo.")
else:
    print("O número é negativo.")
```

### Exemplo de execução

```text
Digite um número: -8
O número é negativo.
```

---

## Atividade 2: Par ou ímpar

### Objetivo

Introduzir a lógica condicional com o operador módulo (`%`).

### Descrição

Crie um programa que solicite um número inteiro ao usuário e verifique se ele é:

- Par;
- Ímpar.

> **Dica:** um número é par quando o resto da divisão por `2` é igual a `0`.

### Código

```python
numero = int(input("Digite um número: "))

if numero % 2 == 0:
    print("O número é par.")
else:
    print("O número é ímpar.")
```

### Exemplo de execução

```text
Digite um número: 984984
O número é par.
```

> **Observação:** o número zero também é par, pois `0 % 2` resulta em `0`.

---

## Atividade 3: Sistema de notas

### Objetivo

Utilizar `elif` para verificar diferentes faixas de valores.

### Descrição

Crie um programa que solicite a nota de um aluno e apresente sua situação conforme os seguintes critérios:

- Nota maior ou igual a `7`: **Aprovado**;
- Nota maior ou igual a `5` e menor que `7`: **Recuperação**;
- Nota menor que `5`: **Reprovado**.

### Código

```python
nota = float(input("Digite a nota do aluno: "))

if nota >= 7:
    print("Aluno aprovado com a nota: {}".format(nota))
elif nota >= 5:
    print("Aluno em recuperação com a nota: {}".format(nota))
else:
    print("Aluno reprovado com a nota: {}".format(nota))
```

### Exemplo de execução

```text
Digite a nota do aluno: 2
Aluno reprovado com a nota: 2.0
```

---

## Atividade 4: Simulação de login simples

### Objetivo

Aplicar estruturas condicionais em uma situação mais próxima de um sistema real.

### Descrição

Crie um programa que solicite um usuário e uma senha. O acesso será autorizado somente quando as seguintes credenciais forem informadas:

- **Usuário:** `admin`
- **Senha:** `1234`

### Código

```python
usuario = input("Login: ")
senha = input("Senha: ")

if usuario == "admin" and senha == "1234":
    print("Login realizado.")
elif usuario != "admin":
    print("Usuário incorreto.")
elif senha != "1234":
    print("Senha incorreta.")
else:
    print("Usuário ou senha inválidos!")
```

### Exemplo de execução

```text
Login: admin
Senha: 12555
Senha incorreta.
```

---

## Conceitos utilizados

### Estruturas condicionais

- `if`: executa um bloco quando uma condição é verdadeira;
- `elif`: verifica uma nova condição quando a anterior é falsa;
- `else`: executa um bloco quando nenhuma das condições anteriores é verdadeira.

### Operadores

- `>`: maior que;
- `>=`: maior ou igual a;
- `==`: igual a;
- `!=`: diferente de;
- `%`: retorna o resto de uma divisão;
- `and`: exige que todas as condições sejam verdadeiras.

## Tecnologias utilizadas

- Python 3

## Autor

Desenvolvido por **Victor Gabriel Tavares Oliveira** como parte dos estudos de lógica de programação com Python.
