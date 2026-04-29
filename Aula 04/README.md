# Aula 04 - Funções de Texto, Contagem e Data no Excel

Nesta aula iremos abordar funções importantes para trabalhar com textos, contagens e datas no Excel: MAIÚSCULA, MINÚSCULA, PRI.MAIÚSCULA, NÚM.CARACT, UNIRTEXTO, CONT.NÚM, CONT.VALORES, CONT.VAZIO e HOJE. Essas funções ajudam a organizar informações, padronizar textos, contar dados e inserir datas automaticamente nas planilhas.

## Funções de Texto

### 1. MAIÚSCULA

A função MAIÚSCULA converte um texto para letras maiúsculas.

**Sintaxe:** =MAIÚSCULA(texto)

**Exemplo:**

- Dado: maria
- Fórmula: =MAIÚSCULA(A1)
- Resultado: MARIA

**Uso prático:** Padronizar nomes, cidades ou códigos digitados em letras minúsculas.

### 2. MINÚSCULA

A função MINÚSCULA converte um texto para letras minúsculas.

**Sintaxe:** =MINÚSCULA(texto)

**Exemplo:**

- Dado: MARIA
- Fórmula: =MINÚSCULA(A1)
- Resultado: maria

**Uso prático:** Padronizar e-mails, nomes de usuários ou textos digitados em letras maiúsculas.

### 3. PRI.MAIÚSCULA

A função PRI.MAIÚSCULA deixa a primeira letra de cada palavra em maiúscula.

**Sintaxe:** =PRI.MAIÚSCULA(texto)

**Exemplo:**

- Dado: maria da silva
- Fórmula: =PRI.MAIÚSCULA(A1)
- Resultado: Maria Da Silva

**Uso prático:** Organizar nomes de pessoas, produtos ou endereços.

### 4. NÚM.CARACT

A função NÚM.CARACT conta a quantidade de caracteres de um texto, incluindo espaços.

**Sintaxe:** =NÚM.CARACT(texto)

**Exemplo:**

- Dado: Excel Básico
- Fórmula: =NÚM.CARACT(A1)
- Resultado: 12

**Uso prático:** Verificar o tamanho de textos, senhas, códigos ou descrições.

### 5. UNIRTEXTO

A função UNIRTEXTO une textos de diferentes células, podendo usar um separador entre eles.

**Sintaxe:** =UNIRTEXTO(delimitador; ignorar_vazio; texto1; texto2; ...)

**Exemplo:**

- Dados: Maria em A1 e Silva em B1
- Fórmula: =UNIRTEXTO(" "; VERDADEIRO; A1; B1)
- Resultado: Maria Silva

**Uso prático:** Juntar nome e sobrenome, montar descrições ou criar frases com dados de várias células.

## Funções de Contagem

### 6. CONT.NÚM

A função CONT.NÚM conta quantas células possuem números em um intervalo.

**Sintaxe:** =CONT.NÚM(intervalo)

**Exemplo:**

- Dados: 10, 20, texto, vazio
- Fórmula: =CONT.NÚM(A1:A4)
- Resultado: 2

**Uso prático:** Contar quantas notas, valores de venda ou quantidades foram preenchidas.

### 7. CONT.VALORES

A função CONT.VALORES conta quantas células não estão vazias em um intervalo.

**Sintaxe:** =CONT.VALORES(intervalo)

**Exemplo:**

- Dados: 10, Maria, vazio, 25
- Fórmula: =CONT.VALORES(A1:A4)
- Resultado: 3

**Uso prático:** Contar quantos cadastros, respostas ou informações foram preenchidos.

### 8. CONT.VAZIO

A função CONT.VAZIO conta quantas células vazias existem em um intervalo.

**Sintaxe:** =CONT.VAZIO(intervalo)

**Exemplo:**

- Dados: 10, vazio, Maria, vazio
- Fórmula: =CONT.VAZIO(A1:A4)
- Resultado: 2

**Uso prático:** Identificar campos que ainda precisam ser preenchidos em uma planilha.

## Função de Data

### 9. HOJE

A função HOJE retorna a data atual do computador.

**Sintaxe:** =HOJE()

**Exemplo:**

- Fórmula: =HOJE()
- Resultado: data atual

**Uso prático:** Criar controles de prazos, relatórios diários ou calcular a diferença entre datas.

### 10. DATADIF

A função DATADIF calcula a diferença entre duas datas em dias, meses ou anos.

**Sintaxe:** =DATADIF(data_inicial; data_final; unidade)

**Exemplo:**

- Data inicial: 01/01/2024
- Data final: 01/01/2026
- Fórmula: =DATADIF(A1; B1; "Y")
- Resultado: 2

**Uso prático:** Calcular idade, tempo de empresa, duração de projetos ou quantidade de dias entre duas datas.

---

## Dicas Gerais

- As funções de texto ajudam a padronizar informações digitadas de formas diferentes.
- A função NÚM.CARACT também conta espaços entre palavras.
- Use CONT.NÚM quando quiser contar apenas números.
- Use CONT.VALORES quando quiser contar qualquer célula preenchida.
- Use CONT.VAZIO para encontrar informações que ainda faltam na planilha.
- A função HOJE atualiza automaticamente a data quando a planilha é aberta ou recalculada.
- Na função DATADIF, use "Y" para anos, "M" para meses e "D" para dias.
