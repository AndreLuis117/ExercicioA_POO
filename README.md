# trabalhoPOO

## Construtor 
Um construtor é basicamente o responsável por criar objetos de uma classe. Sempre tem o mesmo nome da classe e não tem nenhum tipo de retorno.

Ex:

```java 
public class animal {
  public String raça; 
  public animal (String raça) { 
    this.raça = raça; 
  }

} 
```

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

É a palavra chave utilizada para verifcar se um objeto é uma instancia de uma classe, ou seja se esse objeto foi criado a partit dessa classe

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

É um tipo de tecnica que possibilita "esconder" atributos auxiliando dessa forma na proteção dos

Ex: 

``` java 		
m.setraça("homo");
```

## Palavra reservada this

É utilizada para meios de diferenciação entre métodos e nome de parametros

Ex:

```java
public void setraça(String raça) {
		this.raça = raça;
	}
```




