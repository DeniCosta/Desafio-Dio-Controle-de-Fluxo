# Desafio: Controle de Fluxo

Este projeto tem como objetivo exercitar os conceitos de controle de fluxo em Java, por meio de um pequeno sistema que recebe dois parâmetros inteiros via terminal e realiza a impressão de uma sequência numérica.

---

## Requisitos do Desafio

1. O sistema deve receber **dois números inteiros como argumentos** na execução via terminal.
2. A aplicação deve imprimir no console a quantidade de interações correspondente à diferença entre os dois números.
3. A saída deve seguir o padrão:
   ```
   Imprimindo o número 1
   Imprimindo o número 2
   ...
   ```
4. Caso o **primeiro número seja maior que o segundo**, o sistema deve lançar uma exceção customizada chamada `ParametrosInvalidosException` com a mensagem:
   ```
   O segundo parâmetro deve ser maior que o primeiro
   ```

---

## Estrutura do Projeto

- `DesafioControleFluxo/`
  - `src/`
    - `Contador.java`: Classe principal responsável pela lógica do programa.
    - `ParametrosInvalidosException.java`: Classe da exceção customizada.

---

## Como executar

1. Compile os arquivos:
   ```bash
   javac Contador.java ParametrosInvalidosException.java
   ```

2. Execute o programa passando dois números inteiros como parâmetros:
   ```bash
   $ java Contador
   $ 12 
   $ 30
   ```

---

## Exemplo de Execução

**Entrada:**
```bash
$ java Contador
$ 12
$ 30
```

**Saída esperada:**
```
Imprimindo o número 1
Imprimindo o número 2
...
Imprimindo o número 18
```

---

## Tratamento de Erros

Se o primeiro número for maior que o segundo:
```bash
$ java Contador
$ 30 
$ 12
```

**Saída esperada:**
```
O segundo parâmetro deve ser maior que o primeiro
```
