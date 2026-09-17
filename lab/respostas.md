# Atividade Avaliativa 2 - Respostas

Nomes:
LUCAS GARZUZE CORDEIRO
VITOR FELIPE LUCINDO DE ANDRADE

GRR:
GRR20250925
GRR20252106

Se a atividade foi feita em dupla, escreva aqui os dois nomes e os dois GRR. As
duas pessoas enviam o mesmo `.zip` na UFPR Virtual.

Ambiente (sistema operacional e versão do Go):

Saída de `go test ./...` na pasta que você vai enviar:

````
$ go test ./...
ok      ds143/atividade2/abb    0.990s
ok      ds143/atividade2/avl    0.992s
```

## Perguntas

1. Em uma frase, como a sua `EhABB` rejeita a árvore que tem o 60 na subárvore
   esquerda do 50, sendo que o 60 é maior que o pai 30?
   - A função rejeita a árvore porque, ao descer para a subárvore esquerda da raiz, ela atualiza o limite superior (max) para 50, fazendo com que o nó 60 falhe na validação por ser maior que o limite permitido para aquele lado.

2. Em uma frase, o que a sua `Sucessor` guarda durante a descida, e por que isso
   basta quando `v` não está na árvore.
   - A função realiza uma espécie de busca pelo valor v e guarda o último nó visitado (inicializado em nil) quando a busca for virar para a esquerda, dessa forma, esse nó representa o sucessor imediato na árvore do valor procurado, e quando v não está na árvore (não há sucessor), a busca só vai para a direita e o valor supracitado permanece nil.

3. A `VerificaAVL` confere duas condições independentes. Dê um exemplo de árvore
   que satisfaz a primeira e falha na segunda, desenhando-a com o campo `Alt` de
   cada nó.

         30 (Alt 2)
        /
      20 (Alt 1)
      /
    10 (Alt 0)

## Uso de IA

Diga se usou ferramentas de IA generativa nesta atividade e em que partes. Não
influencia a nota.

- Foram utilizadas discussões do Stack Overflow para auxiliar na resolução da primeira questão.
- A dupla conclui que não conseguiria finalizar a parte 2 em tempo hábil e por esta razão utilizou IA para compreender o código da árvore AVL e realizar ajustes. O desenvolvimento foi feito de forma gradual, utilizando a IA para esclarecer dúvidas e auxiliar na implementação ao longo da atividade. Modelo utilizado: Gemini Pro.
