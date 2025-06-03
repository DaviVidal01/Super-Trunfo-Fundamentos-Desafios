# ⚙️ Desafio: Nível Aventureiro  
### Super Trunfo em C – Cálculo de Densidade Populacional e PIB per Capita

Neste desafio, o seu programa evolui! Após cadastrar as cartas no nível anterior, agora é hora de incluir **cálculos importantes** que trarão mais realismo ao jogo Super Trunfo baseado em cidades brasileiras.

---

## 🧠 Objetivo

Aprimorar o programa em C do **nível novato** para que ele:

- Continue **lendo os mesmos dados** das duas cartas (estado, código, nome da cidade, população, área, PIB e número de pontos turísticos).
- Calcule e exiba:
  - **Densidade Populacional**: população ÷ área
  - **PIB per Capita**: PIB ÷ população

---

## 📌 O Que Deve Ser Feito

### 🧾 Leitura dos Dados
- Estado (char)
- Código da carta (string ou char[])
- Nome da cidade (string ou char[])
- População (int)
- Área (float)
- PIB (float)
- Número de pontos turísticos (int)

### 🧮 Cálculos
- **Densidade Populacional**  
  `densidade = (float)populacao / area;`

- **PIB per Capita**  
  `pib_per_capita = pib / populacao;`

> Ambos os valores devem ser armazenados em variáveis do tipo `float`.

### 📤 Saída Esperada

O programa deve exibir as informações da carta **formatadas**, incluindo os dois novos atributos:

```txt
Carta 1:
Estado: A
Código: A01
Nome da Cidade: São Paulo
População: 12325000
Área: 1521.11 km²
PIB: 699.28 bilhões de reais
Número de Pontos Turísticos: 50
Densidade Populacional: 8102.47 hab/km²
PIB per Capita: 56724.32 reais
````

---

## ✅ Requisitos Funcionais

* Manter a funcionalidade de cadastro das cartas (como no desafio anterior).
* Calcular e exibir **corretamente**:

  * Densidade populacional
  * PIB per capita

---

## 🚫 Restrições Técnicas

* ❌ **Sem estruturas de repetição** (`for`, `while`)
* ❌ **Sem estruturas de decisão** (`if`, `else`)
* ✅ Pode usar **variáveis do tipo `float`** e **conversões de tipo**

---

## 📎 Observações

* Os valores de ponto flutuante devem ser **formatados com duas casas decimais** na saída.
* O foco aqui é aplicar **operações matemáticas básicas** com tipos diferentes, e garantir **formatação e clareza** na exibição.