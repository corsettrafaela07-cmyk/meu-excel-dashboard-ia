# Dashboard de clientes

Este pacote tem dois arquivos:

- `tabela_clientes.xlsx`: planilha com 15 clientes de exemplo.
- `dashboard_clientes.html`: painel que lê essa planilha e mostra resumo, gráfico e tabela.

## Como usar

1. Salve os dois arquivos na mesma pasta (por exemplo, Downloads).
2. Abra `dashboard_clientes.html` no navegador (clique duas vezes no arquivo).
3. Clique em **Carregar planilha (.xlsx)** e escolha `tabela_clientes.xlsx` ou outra planilha sua.

Ao abrir, o painel já mostra os dados de exemplo. Depois de carregar uma planilha, ele passa a mostrar os dados dela.

## Formato da planilha

A primeira aba precisa ter estas colunas, com estes nomes na linha 1:

| Coluna  | Conteúdo                         |
|---------|----------------------------------|
| ID      | número do cliente                |
| Nome    | nome do cliente                  |
| Produto | produto comprado                 |
| Valor   | número, sem texto (ex.: 349.50)  |
| Data    | data da compra                   |

Pode ter quantas linhas quiser. Linhas sem nome são ignoradas.

## O que o painel mostra

- **Resumo:** número de clientes, receita total, ticket médio e maior compra.
- **Valor por cliente:** barras ordenadas do maior para o menor valor.
- **Todos os clientes:** tabela completa.

## Problemas comuns

- **"A biblioteca de leitura não carregou":** o painel baixa a biblioteca SheetJS da internet para ler o .xlsx. Conecte-se à internet e recarregue a página.
- **"Não encontrei linhas":** confira se os nomes das colunas estão escritos exatamente como na tabela acima.
- **Os dados não mudam quando edito a planilha:** o painel não acompanha o arquivo em tempo real. Salve a planilha e carregue-a de novo pelo botão.
