# 🧙‍♂️ Desafio: Nível Mestre  
### Super Trunfo em C – Batalha de Cartas e Super Poder

Prepare-se para o desafio final! Após criar e enriquecer suas cartas com dados reais, agora é hora de colocá-las em confronto direto. Neste nível, você implementará **comparações** entre os atributos das cartas e criará um atributo especial: o **Super Poder**.

---

## 🧠 Objetivo

Expandir o programa dos níveis anteriores para:

- Calcular a **densidade populacional** e o **PIB per capita** como no nível Aventureiro.
- Calcular o **Super Poder** de cada carta.
- Comparar os atributos de duas cartas e **exibir qual vence em cada critério**.

---

## 📌 O Que Deve Ser Feito

### 🧾 Leitura dos Dados

Para **duas cartas**, leia:

- Estado (char)
- Código (string ou char[])
- Nome da Cidade (string ou char[])
- População (`unsigned long int`) ✅
- Área (`float`)
- PIB (`float`)
- Número de pontos turísticos (`int`)

### 🧮 Cálculos

#### 1. Densidade Populacional
```c
densidade = (float)populacao / area;
````

#### 2. PIB per Capita

```c
pib_per_capita = pib / populacao;
```

#### 3. Super Poder

```c
super_poder = (float)populacao + area + pib + numero_pontos_turisticos + pib_per_capita + (1.0 / densidade);
```

> Armazene o **Super Poder** como `float`.
> Preste atenção à conversão de tipos!

---

## ⚔️ Comparação de Cartas

* Compare **cada atributo numericamente**, seguindo estas regras:

| Atributo               | Regra de Vitória   |
| ---------------------- | ------------------ |
| População              | Maior vence        |
| Área                   | Maior vence        |
| PIB                    | Maior vence        |
| Pontos Turísticos      | Maior vence        |
| Densidade Populacional | **Menor vence** 🧠 |
| PIB per Capita         | Maior vence        |
| Super Poder            | Maior vence        |

* Para cada comparação, imprima:

```txt
[Atributo]: Carta 1 venceu (1) ou Carta 2 venceu (0)
```

---

### 🖥️ Exemplo de Saída

```txt
Comparação de Cartas:

População: Carta 1 venceu (1)
Área: Carta 1 venceu (1)
PIB: Carta 1 venceu (1)
Pontos Turísticos: Carta 1 venceu (1)
Densidade Populacional: Carta 2 venceu (0)
PIB per Capita: Carta 1 venceu (1)
Super Poder: Carta 1 venceu (1)
```

---

## ✅ Requisitos Funcionais

* Manter funcionalidades dos níveis anteriores.
* Calcular corretamente:

  * Densidade populacional
  * PIB per capita
  * Super Poder
* Comparar os atributos entre as duas cartas.
* Exibir qual carta venceu em cada atributo.

---

## 🚫 Restrições Técnicas

* ❌ **Sem estruturas de repetição** (`for`, `while`)
* ❌ **Sem estruturas de decisão** (`if`, `else`)
* ✅ Use expressões booleanas com operadores relacionais

---

## 🔚 Encerramento

Esse é o nível mais alto da jornada Super Trunfo! Você agora domina:

* Entrada e saída de dados
* Operações com diferentes tipos numéricos
* Conversão de tipos em C
* Lógica de comparação e estruturação de dados