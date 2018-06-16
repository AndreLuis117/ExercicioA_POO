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

É a palavra utilizada para invocar o construtor

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


