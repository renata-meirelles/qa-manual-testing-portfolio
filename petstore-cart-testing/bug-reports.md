# PetStore — Relatórios de Bugs

## Sobre este documento

Este arquivo organiza os quatro defeitos documentados durante a atividade prática **STLC Practice – Test Execution & Reporting**, realizada na Mate Academy.

Os relatos foram recuperados da guia **Bugs** da planilha original e relacionados aos testes registrados no Checklist.

### Observação sobre os identificadores

Na guia Bugs original, os quatro relatórios aparecem com o identificador repetido `PS-001`.

Para facilitar a leitura e a rastreabilidade neste portfólio, foram utilizados os identificadores PS-001, PS-002, PS-003 e PS-004, seguindo as referências já existentes na coluna **Bug ID** do Checklist.

Essa organização não representa a descoberta de novos bugs nem uma nova execução dos testes.

---

## PS-001 — Carrinho não está acessível pelas páginas de categoria

**Teste relacionado:** CT-20
**Severidade registrada na guia Bugs:** Moderate

### Precondição

* Usuário autenticado na aplicação.

### Passos para reproduzir

1. Fazer login no JPetStore.
2. Abrir uma categoria, como Fish ou Dogs.
3. Tentar acessar o carrinho de compras.

### Resultado esperado

O carrinho de compras deve estar acessível a partir de qualquer página da aplicação.

### Resultado atual registrado

Não existe link ou botão para acessar o carrinho nas páginas de categoria.

---

## PS-002 — Tooltip "Cart" não aparece no ícone do carrinho

**Teste relacionado:** CT-21
**Severidade registrada na guia Bugs:** Moderate

### Precondição

* Usuário autenticado na aplicação.

### Passos para reproduzir

1. Fazer login no JPetStore.
2. Posicionar o mouse sobre o ícone do carrinho.
3. Aguardar de 2 a 3 segundos.

### Resultado esperado

O ícone do carrinho deve apresentar o tooltip "Cart".

### Resultado atual registrado

Nenhum tooltip aparece ao posicionar o mouse sobre o ícone do carrinho.

---

## PS-003 — Indicador do carrinho não atualiza após adicionar produtos

**Teste relacionado:** CT-29
**Severidade registrada na guia Bugs:** Moderate

### Precondição

* Usuário autenticado na aplicação.

### Passos para reproduzir

1. Fazer login no JPetStore.
2. Adicionar um ou mais produtos ao carrinho.
3. Observar o ícone do carrinho no cabeçalho da página.

### Resultado esperado

O ícone do carrinho deve apresentar a quantidade atual de produtos adicionados.

### Resultado atual registrado

O ícone do carrinho não apresenta o número de itens adicionados.

---

## PS-004 — Carrinho aceita quantidade superior ao limite de cinco unidades

**Testes relacionados:** CT-31 a CT-35, conforme as referências registradas no Checklist original.
**Severidade registrada na guia Bugs:** Moderate

### Precondições

* Usuário autenticado na aplicação.
* Produto adicionado ao carrinho.

### Passos para reproduzir

1. Fazer login no JPetStore.
2. Adicionar um produto ao carrinho.
3. Informar a quantidade 6 no campo Quantity.
4. Clicar em "Update Cart".

### Resultado esperado

O carrinho não deve aceitar quantidades superiores a cinco unidades do mesmo produto. Deve apresentar a mensagem de validação prevista no requisito e respeitar a quantidade máxima permitida.

Mensagem especificada:

"We are sorry, but you can’t buy more than 5 items of the product."

### Resultado atual registrado

O carrinho aceita a quantidade 6 e atualiza o preço total.

### Técnica de teste relacionada

Análise de valores-limite: foi utilizada uma quantidade superior ao máximo permitido pelo requisito.

---

## Ambiente informado nos relatórios originais

| Campo               | Valor registrado |
| ------------------- | ---------------- |
| Sistema operacional | Windows 11       |
| Navegador           | Chrome (latest)  |
| Versão da aplicação | Demo             |

## Evidências

Os relatórios originais contêm referências a capturas de tela e vídeos. Alguns desses registros utilizam endereços internos do Google Docs (`blob:`), que não funcionam como links públicos permanentes.

Por esse motivo, nenhuma imagem ou gravação foi reproduzida neste arquivo sem a recuperação e verificação do material original.

**Fonte:** [Planilha original da atividade — guia Bugs](https://docs.google.com/spreadsheets/d/1xH7R7dJAD5C0wRHcpoKnw4UtwJm8ZaRzwH1tkbfMB_U/edit?usp=sharing)

## Observações sobre a documentação

* A guia Bugs original apresenta os quatro registros com o mesmo ID (`PS-001`).
* Os quatro relatórios visíveis apresentam severidade Moderate.
* A aba Report apresenta uma distribuição de severidade diferente: 1 Major, 2 Moderate e 1 Minor.
* A divergência será mantida documentada até que exista confirmação sobre a classificação correta.
* Nem todos os testes marcados como Failed possuem um relatório de bug individual associado no Checklist.

Esta revisão reorganiza os registros da atividade original, sem alterar os resultados observados.

**Documentação organizada por:** Renata Meirelles da Silva.
