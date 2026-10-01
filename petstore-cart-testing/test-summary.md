# PetStore — Resumo Final dos Testes Manuais

## 1. Visão geral

Este projeto foi desenvolvido durante minha formação em QA Engineering na Mate Academy, utilizando o carrinho de compras da aplicação JPetStore.

A atividade permitiu praticar as quatro fases do STLC (Software Testing Life Cycle):

1. Análise de requisitos.
2. Desenvolvimento dos testes.
3. Execução dos testes.
4. Elaboração do relatório de resultados.

A documentação deste portfólio foi organizada a partir dos registros originais do exercício.

## 2. Objetivo dos testes

Verificar se o carrinho de compras atende aos requisitos funcionais estabelecidos, incluindo:

* Adição e remoção de produtos.
* Atualização de quantidades e valores.
* Validação do limite máximo de cinco unidades do mesmo produto.
* Verificação de estoque.
* Acesso ao carrinho e redirecionamento para checkout.
* Comportamento do carrinho entre diferentes sessões.

## 3. Resultados registrados

A contagem abaixo foi obtida a partir dos resultados individuais do Checklist original.

| Indicador                               | Resultado |
| --------------------------------------- | --------: |
| Requisitos organizados para o portfólio |        21 |
| Verificações planejadas                 |        37 |
| Testes executados (Passed + Failed)     |        36 |
| Testes aprovados (Passed)               |        26 |
| Testes reprovados (Failed)              |        10 |
| Testes bloqueados (Blocked)             |         1 |
| Bugs documentados                       |         4 |

**Taxa de execução:** 97,3%.

**Taxa de aprovação entre os testes executados:** 72,2%.

O teste CT-37, relacionado à tentativa de adicionar produtos sem estoque, foi registrado como Blocked. O motivo específico do bloqueio não pôde ser confirmado nos materiais recuperados.

## 4. Problemas documentados

Durante a atividade, foram registrados quatro relatórios de bugs:

| ID organizado para o portfólio | Problema                                                         |
| ------------------------------ | ---------------------------------------------------------------- |
| PS-001                         | Carrinho não acessível pelas páginas de categoria.               |
| PS-002                         | Tooltip "Cart" não apresentado no ícone do carrinho.             |
| PS-003                         | Indicador do carrinho não atualizado após adicionar produtos.    |
| PS-004                         | Carrinho aceita quantidade superior ao limite de cinco unidades. |

Os detalhes, as precondições, os passos de reprodução e os resultados observados estão disponíveis em [bug-reports.md](bug-reports.md).

## 5. Limitações e observações

Durante a revisão da documentação original para o portfólio, foram identificados os seguintes pontos:

* A aba Report apresentava 27 testes aprovados, enquanto a contagem individual do Checklist indicava 26 Passed, 10 Failed e 1 Blocked.
* Os relatórios da guia Bugs utilizavam o mesmo identificador PS-001. Os IDs foram reorganizados neste portfólio conforme as referências existentes no Checklist.
* A distribuição de severidade da aba Report não correspondia às classificações apresentadas nos quatro relatórios de bugs recuperados.
* Nem todos os testes reprovados tinham um relatório individual de bug associado.
* O motivo específico do teste bloqueado não foi recuperado.
* Algumas referências às evidências originais utilizavam links internos `blob:`, inadequados para compartilhamento público.

Os documentos do portfólio preservam os comportamentos observados e identificam as divergências encontradas.

**A revisão da documentação não representa uma nova execução dos testes.**

## 6. Aprendizados do projeto

Este exercício permitiu praticar conhecimentos importantes para a atuação em QA:

* Analisar requisitos antes de elaborar os testes.
* Criar um checklist com cenários positivos e negativos.
* Utilizar análise de valores-limite para verificar regras de quantidade.
* Registrar separadamente testes aprovados, reprovados e bloqueados.
* Documentar defeitos com passos de reprodução, resultados esperados e resultados observados.
* Relacionar requisitos, verificações e relatórios de bugs.
* Revisar a consistência das informações antes de apresentar um relatório.

Um dos principais pontos observados foi que diferentes verificações podem falhar devido a um mesmo defeito. Por isso, a quantidade de testes reprovados não precisa ser igual à quantidade de bugs documentados.

## 7. Documentação do projeto

* [Apresentação do projeto](README.md)
* [Requisitos](requirements.md)
* [Checklist](checklist.md)
* [Casos de teste detalhados](test-cases.md)
* [Relatório de execução](test-execution.md)
* [Relatórios de bugs](bug-reports.md)
* [Planilha original da atividade na Mate Academy](https://docs.google.com/spreadsheets/d/1xH7R7dJAD5C0wRHcpoKnw4UtwJm8ZaRzwH1tkbfMB_U/edit?usp=sharing)

---

**Autora:** Renata Meirelles da Silva
**Formação:** QA Engineering — Mate Academy
**Tipo de projeto:** Prática educacional de testes manuais.
