### Descrição do Componente

Este código é um exemplo de um componente React que utiliza o hook useEffect para interagir com uma API mockada e buscar dados sobre raças de cachorros.

## useEffect Inicial

No primeiro useEffect, ao carregar o componente pela primeira vez, é feito um fetch para obter uma lista de raças de cachorros da API mockada em http://localhost:8080/doguinhos. Os dados recebidos são armazenados no estado racas usando o setRacas.

## useEffect Dependente de busca

O segundo useEffect é acionado sempre que o estado busca é alterado. Se o valor de busca for uma string com mais de 3 caracteres, é feito um fetch para a API com um parâmetro de consulta (nome). Os dados recebidos são novamente armazenados no estado racas.

## Input de Busca

O campo de input permite ao usuário digitar um termo de busca, que atualiza o estado busca conforme o valor do input muda.
## Renderização da Lista de Raças

A lista de raças é renderizada dinamicamente no componente ul, onde cada raça é exibida como um item da lista li.

Esse componente exemplifica como fazer requisições a uma API e atualizar o estado do componente em resposta a essas requisições e entradas do usuário.
