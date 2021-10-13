# GoLang_Study
O Golang é uma linguagem criada pelo google com o foco em performance para substituir os sistemas em C++ e C.

* A linguagem GO - é uma linguagem moderna e simples para compilação.
* O GO é uma linguagem muito bem modularizada.
* Sintaxe com 25 palavras chaves.
* Uma linguagem simples sem foco em convenção.
* Sempre que chamamos uma função externa no golang o pacote externo é chamado através do seu nome e a primeira letra é maiuscula. por exemplo 
```	
fmt.Println()
```
## Tipos de Variavies

* string 
* float32
* float64
* int

Quando nao atribuimos valores para variavies inteiras o Go assume o valor 0 para essa variavel.
<br> O go não deixa buildar codigo com variaveis inutilizadas.<br>

Para concatenar um texto em go precisamos passar o nome da variavel após a virgula depois de uma string.
```
fmt.Println("O preço do leite é R$", precoLeite)
```
### Inferências de tipos

Um ponto importante da linguagem GO é que ele pode inferir a variavel onde não precisamos declarar o tipo de dados, onde ele automáticamente reconhece o datatype, por exemplo:
```
var nome = "Anderson Xavier"
var idade = 10
**ou** 
nome := "Anderson Xavier"
idade := 10
```
Um ponto importante é sempre tomar cuidado ao inferir variaveis 

### Coleções em GO

**Array** - Precisa determinar o tamanho do conjunto de dados.
```
var estados [4]string
```
Como iterar um array
```
	estados[0] = "RJ"
	estados[1] = "SP"
	estados[2] = "MG"
	estados[3] = "ES"
```


**Slice** - Trata-se de um array por baixo dos panos, ele basicamente cria um array com o numero de posições e capacidade igual ao número de valores atribuidos.<br>
Um fator importante é que quando populamos um slice, ele automáticamente dobra a sua capacidade que pode ser notada pelo comando ```cap(nomes)```

* **```len(nomes)```** quantidade de itens no slice/array 
```
nomes:= [] string{"Douglas","Daniel","Bernardo"}
//esta é a forma que usamos para popular um slice.
nomes = append(nomes, "Marilson")
```
Montagem do ambiente 

é importante mudar os valores dos arquivos bash do root e do usuário para que consiga usar o GOPAHT

### Estruturas de repetição
* **```for i, item := range sites { //instrução}```** Forma mais adequada 
* **```for i := 0; i < len(sites); i++ {
        fmt.Println(sites[i])
    }```** forma antiga.

