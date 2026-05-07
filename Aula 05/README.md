# Aula 05 - Funcao IF/SE no Excel

Nesta aula iremos abordar a funcao IF do Excel, chamada de SE na versao em portugues. Essa funcao permite criar testes logicos dentro da planilha, retornando um resultado quando a condicao for verdadeira e outro resultado quando a condicao for falsa.

## Funcao Condicional

### 1. IF / SE

A funcao IF/SE verifica uma condicao e mostra um resultado diferente de acordo com a resposta do teste.

**Sintaxe em ingles:** =IF(teste_logico; valor_se_verdadeiro; valor_se_falso)

**Sintaxe em portugues:** =SE(teste_logico; valor_se_verdadeiro; valor_se_falso)

**Exemplo:**

- Dado: nota 7 em A1
- Formula: =SE(A1>=6; "Aprovado"; "Reprovado")
- Resultado: Aprovado

**Uso pratico:** Verificar aprovacao de alunos, metas de vendas, situacao de pagamentos ou qualquer condicao que tenha dois resultados possiveis.

## Exemplos de Uso

### 2. Verificar Aprovacao

Neste exemplo, o Excel analisa se a nota do aluno e maior ou igual a 6.

**Formula:** =SE(B2>=6; "Aprovado"; "Reprovado")

**Exemplo:**

- Nota: 8
- Formula: =SE(B2>=6; "Aprovado"; "Reprovado")
- Resultado: Aprovado

**Uso pratico:** Criar uma coluna de situacao em uma planilha de notas.

### 3. Verificar Meta de Vendas

A funcao SE tambem pode comparar valores de vendas com uma meta definida.

**Formula:** =SE(B2>=1000; "Meta atingida"; "Abaixo da meta")

**Exemplo:**

- Venda: 850
- Formula: =SE(B2>=1000; "Meta atingida"; "Abaixo da meta")
- Resultado: Abaixo da meta

**Uso pratico:** Acompanhar desempenho de vendedores, lojas ou equipes.

### 4. Verificar Pagamento

Podemos usar a funcao SE para identificar se um pagamento foi realizado.

**Formula:** =SE(C2="Pago"; "Finalizado"; "Pendente")

**Exemplo:**

- Status: Pago
- Formula: =SE(C2="Pago"; "Finalizado"; "Pendente")
- Resultado: Finalizado

**Uso pratico:** Controlar contas a pagar, mensalidades, pedidos ou entregas.

### 5. SE com Valores Numericos

A funcao SE pode retornar textos ou numeros. Neste exemplo, o Excel aplica um bonus quando o funcionario bate a meta.

**Formula:** =SE(B2>=1000; 100; 0)

**Exemplo:**

- Venda: 1200
- Formula: =SE(B2>=1000; 100; 0)
- Resultado: 100

**Uso pratico:** Calcular bonus, descontos, taxas ou comissoes simples.

### 6. SE Aninhado

O SE aninhado acontece quando usamos uma funcao SE dentro de outra funcao SE. Isso permite trabalhar com mais de dois resultados.

**Formula:** =SE(B2>=9; "Otimo"; SE(B2>=6; "Aprovado"; "Reprovado"))

**Exemplo:**

- Nota: 7
- Formula: =SE(B2>=9; "Otimo"; SE(B2>=6; "Aprovado"; "Reprovado"))
- Resultado: Aprovado

**Uso pratico:** Classificar notas, faixas de vendas, niveis de estoque ou prioridades.

## Operadores Logicos

Os operadores logicos sao usados para montar o teste da funcao SE.

| Operador | Significado | Exemplo |
| --- | --- | --- |
| = | Igual a | =SE(A1=10; "Sim"; "Nao") |
| <> | Diferente de | =SE(A1<>10; "Diferente"; "Igual") |
| > | Maior que | =SE(A1>10; "Maior"; "Menor ou igual") |
| < | Menor que | =SE(A1<10; "Menor"; "Maior ou igual") |
| >= | Maior ou igual a | =SE(A1>=6; "Aprovado"; "Reprovado") |
| <= | Menor ou igual a | =SE(A1<=5; "Baixo"; "Adequado") |

---

## Dicas Gerais

- No Excel em portugues, a funcao IF e chamada de SE.
- O teste logico sempre deve comparar valores, textos, datas ou celulas.
- Textos dentro da formula devem ficar entre aspas, como "Aprovado" ou "Pendente".
- Use ponto e virgula para separar os argumentos da funcao no Excel em portugues.
- A funcao SE retorna apenas um dos dois resultados: verdadeiro ou falso.
- Para mais de duas possibilidades, utilize SE aninhado ou combine a funcao SE com outras funcoes.
- Evite criar formulas muito longas; quando necessario, organize os dados em colunas auxiliares.
