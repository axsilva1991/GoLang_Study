# GoLang_Orientação a Objetos  
Neste arquivo iremos aprender como estruturar a orientação a objetos em GOLANG

## Struct
- Trata-se da forma de criação de uma estrutura de objetos em GOLANG  

Criando a estrutura:  
```
type ContaCorrente struct {
    titular       string 
    numeroAgencia int
    numeroConta   int
    saldo         float64
}
```
_Podemos instanciar o objeto de 3 formas:_    
1 - passando o nome do campo e 2 pontos (para quando tivermos que passar apenas alguns parametrsp) 
```
	contaDoGuilherme := ContaCorrente{titular: "Guilherme",
	numeroAgencia: 589, numeroConta: 123456, saldo: 125.5}

```
2 - Passando apenas os campos preenchidos, ideal para quando tivermos que preencher todos os campos.
```
	contaDaBruna := ContaCorrente{"Bruna", 222, 111222, 200}
```
3 - Iniciando e usando algo parecido com o set.   

```
var contaDaCris *ContaCorrente
contaDaCris = new(ContaCorrente)
contaDaCris.titular = "Cris"
contaDaCris.saldo = 500


fmt.Println(*contaDaCris)
```
O **asterisco (*)**  serve como um ponteiro.

### Multiplos Retornos
No golang, podemos ter o retorno de mais de 1 parametro em funções, por exemplo:  

```
func (c *ContaCorrente) Depositar(valorDoDeposito float 64) (string, float 64) {
    if valorDoDeposito > 0 {
        c.saldo += valordoDeposito
        return "Deposito realizado com sucesso", c.saldo
    } else { 
        retur "Valor do depósito menor que zero", c.saldo
    }
}
```
Exemplo de invocação de função que retorna mais de 1 parametro.  
```
status, valor := contaDaSilvia.Depositar(2000)

```





## Referencias:
https://github.com/alura-cursos/go_oo  
https://github.com/alura-cursos/go_oo/tree/aula2
