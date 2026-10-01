# PetStore — Casos de Teste Manuais

## 1. Objetivo

Apresentar casos de teste detalhados para funcionalidades do carrinho de compras da aplicação JPetStore.

Os casos foram organizados para o portfólio a partir dos requisitos e do checklist desenvolvidos durante a atividade STLC da Mate Academy.

Cada caso contém precondições, passos e resultados esperados.

**Importante:** este documento apresenta a especificação dos cenários. Não representa uma nova execução dos testes. Os resultados históricos estão registrados separadamente em `test-execution.md`.

---

## TC-01 — Adicionar um produto ao carrinho

**Requisitos relacionados:** REQ-03 e REQ-09
**Checklist relacionado:** CT-01
**Tipo:** Teste positivo

### Precondições

* Aplicação JPetStore acessível.
* Existência de um produto disponível para compra.

### Passos

1. Acessar a aplicação JPetStore.
2. Selecionar uma categoria de produtos.
3. Abrir os detalhes de um produto disponível.
4. Clicar em "Add to Cart".
5. Acessar o carrinho.

### Resultado esperado

O produto selecionado deve aparecer no carrinho com suas informações correspondentes.

---

## TC-02 — Adicionar cinco unidades do mesmo produto

**Requisito relacionado:** REQ-13
**Checklist relacionado:** CT-31
**Tipo:** Teste de valor-limite — cenário positivo

### Precondições

* Usuário autenticado.
* Produto disponível no carrinho, com estoque suficiente para cinco unidades.

### Passos

1. Acessar o carrinho.
2. Localizar o campo "Quantity" do produto.
3. Informar a quantidade 5.
4. Clicar em "Update Cart".

### Resultado esperado

A aplicação deve aceitar cinco unidades do mesmo produto, desde que exista estoque suficiente, pois essa é a quantidade máxima permitida pelo requisito.

---

## TC-03 — Tentar adicionar seis unidades do mesmo produto

**Requisitos relacionados:** REQ-13, REQ-14 e REQ-15
**Checklist relacionado:** CT-31, CT-33 e CT-34
**Bug documentado na execução original:** PS-004
**Tipo:** Teste de valor-limite — cenário negativo

### Precondições

* Usuário autenticado.
* Produto adicionado ao carrinho.

### Passos

1. Acessar o carrinho.
2. Localizar o campo "Quantity".
3. Informar a quantidade 6.
4. Clicar em "Update Cart".

### Resultado esperado

A aplicação deve impedir a compra de mais de cinco unidades do mesmo produto e apresentar a mensagem prevista no requisito:

"We are sorry, but you can’t buy more than 5 items of the product."

### Referência à execução histórica

Na atividade original, foi registrado que o carrinho aceitou a quantidade 6 e atualizou o preço total. Esse comportamento está documentado no bug PS-004.

Este caso de teste foi estruturado para o portfólio; não corresponde a uma nova execução.

---

## TC-04 — Remover um produto informando quantidade zero

**Requisito relacionado:** REQ-17
**Checklist relacionado:** CT-36
**Tipo:** Teste positivo

### Precondições

* Usuário autenticado.
* Existência de pelo menos um produto no carrinho.

### Passos

1. Acessar o carrinho.
2. Localizar o produto que será removido.
3. Alterar o campo "Quantity" para 0.
4. Clicar em "Update Cart".

### Resultado esperado

O produto deve ser removido do carrinho.

---

## TC-05 — Validar o redirecionamento para checkout de usuário não autenticado

**Requisito relacionado:** REQ-07
**Checklist relacionado:** CT-26
**Tipo:** Teste funcional

### Precondições

* Usuário não autenticado.
* Existência de pelo menos um produto no carrinho.

### Passos

1. Acessar o carrinho.
2. Clicar em "Proceed to Checkout".

### Resultado esperado

A aplicação deve redirecionar o usuário para a página de login.

---

## TC-06 — Verificar a atualização do indicador do carrinho

**Requisito relacionado:** REQ-10
**Checklist relacionado:** CT-29
**Bug documentado na execução original:** PS-003
**Tipo:** Teste funcional

### Precondições

* Usuário autenticado.
* Produto disponível para compra.

### Passos

1. Acessar uma página com produtos disponíveis.
2. Adicionar um ou mais produtos ao carrinho.
3. Observar o ícone do carrinho no cabeçalho.

### Resultado esperado

O indicador do ícone deve apresentar a quantidade atual de produtos adicionados ao carrinho.

### Referência à execução histórica

Na atividade original, foi registrado que o ícone não apresentava o número de itens adicionados. Esse comportamento foi documentado no bug PS-003.

---

## 2. Técnicas utilizadas na elaboração

**Testes positivos:** verificam o comportamento esperado quando o usuário realiza ações permitidas.

**Testes negativos:** verificam como a aplicação responde a entradas ou ações que não devem ser aceitas.

**Análise de valores-limite:** aplicada aos cenários de quantidade máxima, utilizando os valores 5 (limite permitido) e 6 (primeiro valor acima do limite).

## 3. Referências

* [Requisitos originais do carrinho PetStore](https://docs.google.com/document/d/1s2oyY-t5lZSZhv0DYItE3V9-Djn5acGgRNf7hyen97A/edit?usp=sharing)
* [Planilha original da atividade STLC](https://docs.google.com/spreadsheets/d/1xH7R7dJAD5C0wRHcpoKnw4UtwJm8ZaRzwH1tkbfMB_U/edit?usp=sharing)
* [Checklist deste portfólio](checklist.md)
* [Relatório de execução](test-execution.md)
* [Relatórios de bugs](bug-reports.md)

**Documentação organizada por:** Renata Meirelles da Silva.
