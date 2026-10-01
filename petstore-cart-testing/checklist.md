# PetStore — Checklist de Testes Manuais

## Objetivo

Documentar as verificações planejadas para avaliar as funcionalidades do carrinho de compras da aplicação JPetStore.

Este checklist foi elaborado durante a atividade **STLC Practice – Test Design**, da Mate Academy, a partir dos requisitos fornecidos para o exercício.

**Total de verificações planejadas:** 37.

**Importante:** este documento apresenta o planejamento dos testes. Os resultados reais (Passed, Failed e Blocked) serão apresentados separadamente no relatório de execução.

## Checklist

| ID    | Verificação                                                                                                  | Prioridade |
| ----- | ------------------------------------------------------------------------------------------------------------ | ---------- |
| CT-01 | Verificar se o usuário consegue adicionar um produto ao carrinho.                                            | Critical   |
| CT-02 | Verificar se o usuário consegue adicionar várias unidades do mesmo produto.                                  | High       |
| CT-03 | Verificar se o usuário consegue adicionar produtos diferentes ao carrinho.                                   | High       |
| CT-04 | Verificar se nome, quantidade e preço dos produtos são exibidos corretamente.                                | High       |
| CT-05 | Verificar se o valor total do carrinho é calculado corretamente.                                             | Critical   |
| CT-06 | Verificar se a quantidade de um produto pode ser atualizada.                                                 | High       |
| CT-07 | Verificar se o total é atualizado após alterar a quantidade.                                                 | Critical   |
| CT-08 | Verificar se um produto pode ser removido do carrinho.                                                       | Critical   |
| CT-09 | Verificar se o carrinho fica vazio após a remoção de todos os produtos.                                      | High       |
| CT-10 | Verificar o comportamento do campo de quantidade ao informar zero ou um número negativo.                     | High       |
| CT-11 | Verificar se o campo de quantidade aceita somente valores numéricos.                                         | Medium     |
| CT-12 | Verificar se os produtos permanecem no carrinho após atualizar a página.                                     | Medium     |
| CT-13 | Verificar se o botão de checkout está disponível quando existem produtos no carrinho.                        | Critical   |
| CT-14 | Verificar se não é possível prosseguir com o checkout quando o carrinho está vazio.                          | Critical   |
| CT-15 | Verificar se a mensagem de carrinho vazio é exibida corretamente.                                            | Medium     |
| CT-16 | Verificar se o usuário consegue continuar comprando a partir do carrinho.                                    | Medium     |
| CT-17 | Verificar se o carrinho de um usuário autenticado aparece em outras sessões.                                 | Medium     |
| CT-18 | Verificar se o carrinho fica vazio na sessão após o logout.                                                  | Medium     |
| CT-19 | Verificar se um produto removido também desaparece das demais sessões.                                       | High       |
| CT-20 | Verificar se o carrinho pode ser acessado a partir de qualquer página.                                       | Medium     |
| CT-21 | Verificar se o ícone do carrinho apresenta o tooltip "Cart".                                                 | Low        |
| CT-22 | Verificar se a tabela apresenta todas as colunas exigidas nos requisitos.                                    | High       |
| CT-23 | Verificar se a última linha da tabela apresenta o "Sub Total".                                               | High       |
| CT-24 | Verificar se o botão "Update Cart" é exibido.                                                                | Medium     |
| CT-25 | Verificar se o checkout direciona usuários autenticados à página de checkout.                                | Critical   |
| CT-26 | Verificar se o checkout direciona visitantes não autenticados à página de login.                             | Critical   |
| CT-27 | Verificar se um produto pode ser adicionado pelo Product Details Page (PDP).                                 | Critical   |
| CT-28 | Verificar se um produto pode ser adicionado pela lista de produtos.                                          | Critical   |
| CT-29 | Verificar se o indicador do ícone do carrinho é atualizado após adicionar produtos.                          | High       |
| CT-30 | Verificar se "Item ID" e "Name" possuem links clicáveis.                                                     | Medium     |
| CT-31 | Verificar se a quantidade máxima permitida do mesmo produto é de cinco unidades.                             | High       |
| CT-32 | Verificar a validação da quantidade após pressionar Enter.                                                   | High       |
| CT-33 | Verificar a validação da quantidade após clicar em "Update Cart".                                            | High       |
| CT-34 | Verificar se a mensagem de validação aparece quando a quantidade ultrapassa cinco unidades.                  | High       |
| CT-35 | Verificar se a mensagem de validação aparece quando a quantidade solicitada ultrapassa o estoque disponível. | High       |
| CT-36 | Verificar se informar quantidade zero e clicar em "Update Cart" remove o produto.                            | High       |
| CT-37 | Verificar se produtos sem estoque não podem ser adicionados ao carrinho.                                     | Critical   |

## Fonte da documentação

* [Requisitos originais da PetStore](https://docs.google.com/document/d/1s2oyY-t5lZSZhv0DYItE3V9-Djn5acGgRNf7hyen97A/edit?usp=sharing)
* [Planilha original — Checklist e execução dos testes](https://docs.google.com/spreadsheets/d/1xH7R7dJAD5C0wRHcpoKnw4UtwJm8ZaRzwH1tkbfMB_U/edit?usp=sharing)

## Observação sobre a revisão

A redação da verificação CT-10 foi ajustada para evitar conflito com a CT-36. Conforme o requisito original, informar quantidade zero e atualizar o carrinho deve remover o produto. O comportamento esperado para valores negativos será tratado separadamente.

Os resultados da execução não foram modificados neste documento.

**Documentação organizada por:** Renata Meirelles da Silva.
