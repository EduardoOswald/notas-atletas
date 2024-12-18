# Calculador de Média de Atletas

Este projeto é uma aplicação simples em JavaScript que calcula a média válida das notas de atletas em uma competição de ginástica, seguindo as regras fornecidas.

## Descrição
A aplicação recebe uma lista de atletas com seus respectivos nomes e notas atribuídas por cinco jurados. As notas são processadas de acordo com as seguintes regras:

1. Ordenar as notas em ordem crescente.
2. Descartar a menor e a maior nota.
3. Calcular a média das três notas restantes.
4. Exibir o nome do atleta, suas notas originais e a média calculada.

## Tecnologias Utilizadas

- **JavaScript**: Linguagem utilizada para implementar a lógica do código.

## Como Utilizar

### Passo 1: Preparar os dados
Os dados devem ser estruturados como um array de objetos, onde cada objeto representa um atleta. Cada objeto deve conter:
- **nome**: O nome do atleta.
- **notas**: Um array com cinco notas atribuídas ao atleta.

### Passo 2: Chamar a função
A função `calcularMedia` deve ser chamada passando o array de atletas como parâmetro.

### Exemplo de Entrada:
```javascript
let atletas = [
    {
        nome: "Cesar Abascal",
        notas: [10, 9.34, 8.42, 10, 7.88]
    },
    {
        nome: "Fernando Puntel",
        notas: [8, 10, 10, 7, 9.33]
    },
    {
        nome: "Daiane Jelinsky",
        notas: [7, 10, 9.5, 9.5, 8]
    },
    {
        nome: "Bruno Castro",
        notas: [10, 10, 10, 9, 9.5]
    }
];

calcularMedia(atletas);


### Exemplo de Saída:
```
Atleta: Cesar Abascal  
Notas Obtidas: 10,9.34,8.42,10,7.88  
Média Válida: 9.253333333333334

Atleta: Fernando Puntel  
Notas Obtidas: 8,10,10,7,9.33  
Média Válida: 9.11

Atleta: Daiane Jelinsky  
Notas Obtidas: 7,10,9.5,9.5,8  
Média Válida: 9  

Atleta: Bruno Castro  
Notas Obtidas: 10,10,10,9,9.5  
Média Válida: 9.833333333333334  
```

## Conceitos Aplicados

- **Manipulação de Arrays**:
  - Uso de `sort()` para ordenar as notas.
  - Uso de `slice()` para selecionar as notas válidas.
  - Uso de `reduce()` para calcular a soma das notas.

Sinta-se à vontade para adaptar o código às suas necessidades ou expandi-lo com mais funcionalidades.
