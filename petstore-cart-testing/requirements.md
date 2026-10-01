# PetStore — Requisitos do Carrinho de Compras

## Sobre este documento

Este arquivo apresenta os requisitos funcionais utilizados na atividade prática de STLC (Software Testing Life Cycle) da Mate Academy.

Os requisitos foram organizados e numerados para facilitar o planejamento, a rastreabilidade e a documentação dos testes manuais.

**Aplicação:** [JPetStore](https://jpetstore.mate.academy/actions/Catalog.action)

**Fonte:** [PetStore Cart Requirements — Mate Academy](https://docs.google.com/document/d/1s2oyY-t5lZSZhv0DYItE3V9-Djn5acGgRNf7hyen97A/edit?usp=sharing)

---

## 1. Requisitos gerais do carrinho

| ID     | Requisito                                                                                                                                  |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------ |
| REQ-01 | O usuário deve conseguir acessar o carrinho a partir de qualquer página da aplicação.                                                      |
| REQ-02 | O ícone do carrinho deve apresentar o tooltip "Cart".                                                                                      |
| REQ-03 | O carrinho deve apresentar uma tabela com as colunas Item ID, Product ID, Name, Description, In Stock?, Quantity, List Price e Total Cost. |
| REQ-04 | A última linha da tabela deve apresentar o valor total identificado como "Sub Total" e o botão "Update Cart".                              |
| REQ-05 | O carrinho deve estar vazio inicialmente e apresentar a mensagem "Your cart is empty.".                                                    |
| REQ-06 | O botão "Proceed to Checkout" deve aparecer abaixo da tabela quando houver pelo menos um produto no carrinho.                              |
| REQ-07 | O botão de checkout deve direcionar usuários autenticados à página de checkout e usuários não autenticados à página de login.              |
| REQ-08 | O usuário deve conseguir sair da página do carrinho pelo link "Return to Main Menu".                                                       |

## 2. Adição, remoção e atualização de produtos

| ID     | Requisito                                                                                                                                       |
| ------ | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| REQ-09 | O usuário deve conseguir adicionar produtos pelo botão "Add to Cart", tanto na página de detalhes do produto (PDP) quanto na lista de produtos. |
| REQ-10 | Ao adicionar produtos, o ícone do carrinho deve apresentar um indicador (badge) com a quantidade de produtos adicionados.                       |
| REQ-11 | Os campos "Item ID" e "Name" dos produtos no carrinho devem conter links clicáveis.                                                             |
| REQ-12 | O campo "Quantity" deve aceitar somente números.                                                                                                |
| REQ-13 | O usuário não deve conseguir adicionar mais de cinco unidades do mesmo produto por pedido.                                                      |
| REQ-14 | A validação da quantidade deve ocorrer após pressionar Enter ou clicar em "Update Cart".                                                        |
| REQ-15 | O sistema deve apresentar as mensagens de validação previstas quando a quantidade ultrapassar cinco unidades ou o estoque disponível.           |
| REQ-16 | O usuário deve conseguir remover produtos utilizando o botão "Remove".                                                                          |
| REQ-17 | Ao informar quantidade zero e clicar em "Update Cart", o produto deve ser removido do carrinho.                                                 |
| REQ-18 | Produtos sem estoque não devem poder ser adicionados ao carrinho.                                                                               |

### Mensagens previstas no REQ-15

**Quantidade superior a cinco:**

"We are sorry, but you can’t buy more than 5 items of the product."

**Quantidade superior ao estoque disponível:**

"We are sorry, but we have only N items of this product for now. Would you like to subscribe to notifications when this product will be available?"

## 3. Comportamento do carrinho entre sessões

| ID     | Requisito                                                                                                   |
| ------ | ----------------------------------------------------------------------------------------------------------- |
| REQ-19 | Os produtos adicionados por um usuário autenticado devem aparecer nas demais sessões desse usuário.         |
| REQ-20 | Quando o usuário autenticado sair da conta, o carrinho deve ficar vazio na sessão em que realizou o logout. |
| REQ-21 | Quando o usuário remover um produto do carrinho, a remoção deve ser refletida nas demais sessões.           |

---

## Documentação da atividade

* [Documento original dos requisitos](https://docs.google.com/document/d/1s2oyY-t5lZSZhv0DYItE3V9-Djn5acGgRNf7hyen97A/edit?usp=sharing)
* [Planilha utilizada nas atividades STLC Practice — Test Design e Test Execution & Reporting](https://docs.google.com/spreadsheets/d/1xH7R7dJAD5C0wRHcpoKnw4UtwJm8ZaRzwH1tkbfMB_U/edit?usp=sharing)

**Observação:** este documento registra o comportamento esperado da aplicação. Os resultados efetivamente observados durante os testes serão apresentados separadamente no relatório de execução.

**Organização da documentação:** Renata Meirelles da Silva.
