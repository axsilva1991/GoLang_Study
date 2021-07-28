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

**array** - Precisa determinar o tamanho do conjunto de dados.
```
var estados [4]string
```
**Slice**
```
```
