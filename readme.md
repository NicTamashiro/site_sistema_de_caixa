# CaixaFácil — Sistema de Gestão de Caixa

Sistema de gerenciamento de caixa desenvolvido em **C**, com interface web de apresentação, criado para a disciplina de **Algoritmos — UNISANTOS**.

O projeto permite cadastrar notas e moedas, visualizar o saldo detalhado do caixa e simular vendas com cálculo automático de troco utilizando **algoritmo guloso**.

---

##  Preview

Sistema web demonstrativo apresentando:

- Interface institucional moderna
- Explicação do algoritmo
- Código comentado
- Fluxogramas do sistema
- Download do código-fonte em C

---

##  Funcionalidades

###  Cadastro de Notas e Moedas
Permite registrar a quantidade disponível de cada denominação do sistema monetário brasileiro:

- R$ 200,00
- R$ 100,00
- R$ 50,00
- R$ 20,00
- R$ 10,00
- R$ 5,00
- R$ 2,00
- R$ 1,00
- R$ 0,50
- R$ 0,25
- R$ 0,10
- R$ 0,05
- R$ 0,01

---

###  Visualização do Caixa

Exibe:

- Quantidade de cada nota/moeda
- Subtotal por denominação
- Valor total armazenado

---

###  Simulação de Venda

Recebe:

- Valor da compra
- Valor pago pelo cliente

Realiza:

- Validação de pagamento insuficiente
- Cálculo do troco
- Decomposição automática
- Atualização segura do caixa

---

###  Algoritmo Guloso

O cálculo do troco utiliza estratégia **gulosa**:

1. Começa pela maior denominação
2. Usa a maior quantidade possível
3. Atualiza o valor restante
4. Repete até completar o troco

Se o troco não puder ser formado, o caixa **não é alterado**.

---

##  Conceitos aplicados

O projeto explora:

- `struct`
- Ponteiros
- Arrays
- `memcpy()`
- `memset()`
- Validação de entrada
- Aritmética inteira
- Algoritmo guloso
- Atomicidade de operação
- Modularização em funções

---

##  Por que usar centavos inteiros?

Valores monetários são armazenados como inteiros.

Exemplo:

```c
R$ 10,50 → 1050
```

Isso evita erros clássicos de ponto flutuante como:

```c
0.1 + 0.2 != 0.3
```

Garantindo precisão absoluta no cálculo financeiro.

---

##  Estrutura do projeto

```bash
├── cashier.c      # Sistema principal em C
├── index.html     # Site de apresentação
├── style.css      # Estilização
└── README.md
```

---



##  Equipe

- **Cauê Nunes**
- **Ícaro Pelegrini**
- **Nicolas Tamashiro**
- **Paulo Pimenta**

---

##  Disciplina

**Algoritmos — UNISANTOS**

Projeto acadêmico com foco em:

- Estruturas de dados básicas
- Organização modular
- Boas práticas em C
- Resolução algorítmica aplicada

