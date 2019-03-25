# Conceitos de Programação Orientada a Objetos
Documento com  de conceitos de programação orientada a objetos, utilizado para obtenção de nota bimestral para a matéria de Programação Orientada a Objetos no 2º ano de Sistemas de Informação da Universidade da Região de Joinville (Univille).


## Construtor 
Um construtor é basicamente o responsável por criar objetos de uma classe. Sempre tem o mesmo nome da classe e não tem nenhum tipo de retorno

Ex:

```java 
public class animal {
  public String raça; 
  public animal (String raça) { 
    this.raça = raça; 
  }

} 
```

## Instanciação

É a ação de criar um objeto a partir de uma classe

## Palavra reservada new

É a palavra chave utilizada para invocar o construtor

Ex:

```java
public class ex {
	
	public static void main (String[] args) {
		animal m = new animal("macaco");
		m.setraça("homo");
		System.out.println(m.getraça());
		
		
	}

}
```

## Palavra reservada instanciof

É a palavra chave utilizada para verifcar se um objeto é uma instancia de uma classe, ou seja se esse objeto foi criado a partir dessa classe

Ex:

```java
public boolean equals(Object object){
		boolean b = false;
		if(object instanceof Ponto){
			Ponto q = (Ponto) object;
			b = x == q.getX() && y == q.getY();
		}
		return b;
	}
```

## Encapsulamento

É um tipo de tecnica que possibilita "esconder" atributos auxiliando dessa forma na proteção dos dados, usando essa tecnica os atributos só podem ser alterados a partir de métodos específicos

Ex: 

``` java 		
	private String raça;
```

Só pode ser alterado por:

```java
public void setraça(String raça) {
		this.raça = raça;
	}
```

## Palavra reservada this

É utilizada para meios de diferenciação entre métodos e nome de parametros

Ex:

```java
public void setraça(String raça) {
		this.raça = raça;
	}
```

## Getters/Setters

O getter é utilizado para buscar alguma informação sem ter que invocar o atributo, normalmente é utilizado junto com o encapsulamento

Ex:

```java
public String getraça() {
		return raça;
		
	}
```

O setter é utilizado para para setar alguma informação ao atributo ou variável em questão

Ex:

```java
public void setraça(String raça) {
		this.raça = raça;
	}
```

## Palavra reservada public/private

A palavra chave public serve para identificar a visibilidade da classe, objeto ou método como publico ou seja que pode ser visualizado e alterada por todos

Ex:

```java
public double peso;
```

A palavra chave private tem como função identificar a visibilidade da classe, objeto ou método como privado, nesse caso sópodem ser visualizados ou aletrados por métodos especificos aplicando assim a técnica de encapsulamento

Ex:

```java
private String raça;
```

## Assinatura de método

Faz parte da assinatura de método a visibilidade do mesmo, nome, argumentos, quantidades de argumentos

Ex:

```java
public void setraça(String raça) {
		this.raça = raça;
	}
```

## Sobrecarga de método

É uma tecnica que permite que vários métodos coexistam com o mesmo nome

```java
public class Personagem {
    public void acelerar(Carro carro) {
    }
    public void acelerar(Motocicleta motocicleta) {
    }
    public void acelerar(Caminhonete caminhonete) {
    }
}
```

## Escopo de classe

Escopo de classe é ademarcação que você dá a classe, ou seja, aonde ela começa e aond eela termina

Ex:

```java
public class animal { //aqui a classe começa
	private String raça;
	public double peso;
	
	public animal (String raça) { 
		this.raça = raça; }

	public String getraça() {
		return raça;
		
	}
	public void setraça(String raça) {
		this.raça = raça;
	}
	
	
}  //aqui a classe termina
```

## Escopo de objeto

## Palavra reservada final

Quando usada para definir uma variável, significa que a variável não pode assumir outro valor, tornando-se assim uma constante 

Ex: 

```java
	final int pesofixo = 10;
```

Quando utilizada na definição de um método, significa que o método não poderá ser aletrado ou sobrescrito

Ex:

```java
final public String getraça() {
		return raça;
		
	}
```

Quando usada para definir uma classe, significa que a classe não vai permitir herança

Ex:

```java
final public class animal {
}
```

## Relacionamento de dependência

Relacionamento de quando uma classe depende de outra, ocorre quando uma classe usa os serviços de outra

Ex:

![alt text](https://github.com/AndreLuis117/trabalhoPOO/blob/master/Dependencia.png)

## Relacinamento de Agregação

Ocorre quando uma classe está agregando itens em outra classe (relaciomaneto todo - parte), neste caso a parte existe em o todo

Ex:

![alt text](https://github.com/AndreLuis117/trabalhoPOO/blob/master/Agrega%C3%A7%C3%A3o.png)

## Relacionamento de Composição

Ocorre quando uma classe é composta de outra classe (relacionamento todo - parte), neste caso a parte não existe sem o todo

Ex:

![alt text](https://github.com/AndreLuis117/trabalhoPOO/blob/master/Composi%C3%A7%C3%A3o.png)












	
