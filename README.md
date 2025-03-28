# Entregável 1 - Java
<sup>Isabela R. de Souza - Ciência da Computação - 3° semestre</sup>

## Parte 1 - Histórico e Evolução do Java


Java foi criado em 1991 por uma equipe da Sun Microsystems, composta por James Golsing, Mike Sheridan e Patrick Naughton. Em 2009, a Oracle Corporation adquiriu a empresa, assumindo a responsabilidade pelo desenvolvimento e manutenção do Java a partir de 2010.

Principal objetivo do Java é:

### WORA -> Write Once, Read Anywhere!

Essa caracerística impactou bastante a programação moderna, facilitando o desenvolvimento de aplicações de multiplataforma.

Java passou por muitas atualizações importantes, essas incluem:

* Java 1.0 (1996) _JVM e Bibliotteca de Classes_
* Java 2 (1998) _Edições: Standard, Enterprise e Micro_
* Java SE 5 (2004) _Produtividade e Segurança do código_
* Java SE 8 (2014) _Lambda e API de Streams_
* Java SE 9 (2017) _Sistema de Módulos (Projec Jigsaw)_
* Java SE 17 (2021) _Versão de suporte de longo prazo (LTS)_

Essa constante evolução da linguagem, mantém o Java como uma das mais relevantes e amplamente usadas no cenário atual da tecnologia.

## Parte 2 - Ambientes de Desenvolvimento (IDEs)

### Eclipse 

...é uma IDE de código aberto, conhecido por sua extensibilidade, permite a adição de diversos plugins para suportar diferentes ferramentas e tecnologias.

**Vantagens**

* Extensa biblioteca de plugins que possibilita a personalização conforme as necessidades do desenvolvedor.
* Grande comunidade de usuários, oferecendo ampla documentação e suporte.
* Integração com sistemas de controle de versão, como Git e SVN.

**Desvantagens**

* Pode ser pesado e consumir considerável quantidade de memória, afetando o desempenho em máquinas menos potentes.
* A curva de aprendizado pode ser íngreme para iniciantes devido à sua complexidade e variedade de funcionalidades.

### IntelliJ

...é reconhecido por sua inteligência e recursos avançados que aumentam a produtividade no desenvolvimento Java.

**Vantagens**

* Interface intuitiva e recursos de autocompletar inteligentes que facilitam a codificação.
* Suporte nativo a diversos frameworks populares, como Spring e Hibernate.
* Ferramentas integradas para desenvolvimento web, mobile e empresarial.

**Desvantagens**

* A versão completa (Ultimate) é paga, o que pode ser um impeditivo para alguns desenvolvedores.
* Consome uma quantidade significativa de recursos do sistema, podendo impactar o desempenho em computadores com hardware limitado.

### NetBeans

...é conhecido por sua simplicidade e facilidade de uso, sendo uma boa opção para iniciantes.

**Vantagens**

* Interface amigável e fácil de navegar, ideal para quem está começando no desenvolvimento Java.
* Suporte integrado para criação de interfaces gráficas com o recurso "drag-and-drop".
* Atualizações regulares e suporte ativo da comunidade.

**Desvantagens**

* Menor quantidade de plugins e extensões em comparação com o Eclipse.
* Pode ser menos eficiente em projetos de grande escala devido a limitações de desempenho.

## Parte 3 - Paradigma de Programação Orientado a Objetos

### Classe

Uma classe é um modelo para criar objetos. Ela define atributos e métodos que os objetos instanciados dela poderão ter.

```java
class Gato {
    String raca;
    int anoNascimento;

    void mostrarFicha() {
        System.out.println("Raça: " + raca + ", Ano: " + anoNascimento);
    }
}
```

### Objeto

Um objeto é uma instância de uma classe. Ele possui valores próprios para seus atributos e pode executar os métodos definidos na classe.

```java
public class Main {
    public static void main(String[] args) {
        Gato meuGato = new Gato(); // Criando um objeto da classe Gato
        meuCarro.raca = "Balinês";
        meuCarro.anoNascimento = 2022;
        meuCarro.mostrarFicha();
    }
}
```

### Encapsulamento

O encapsulamento é o conceito de proteger os atributos de uma classe, permitindo o acesso a eles apenas através de métodos específicos (getters e setters).

```java
class Gato {
    String raca;
    int anoNascimento;

    public String getAnoNascimento() {
        return anoNascimento;
    }
}

public class Main {
    public static void main(String[] args) {
        Gato meuGato = new Gato();
        System.out.println("Nome: " + meuGato.getAnoNascimento()); // Obtém o nome usando o getter
    }
}
```

### Herança

A herança permite que uma classe filha herde atributos e métodos de outra classe pai, promovendo reutilização de código.

```java
class Animal {
    String nome;

    void fazerSom() {
        System.out.println("O animal faz um som.");
    }
}

class Gato extends Animal {
    void miar() {
        System.out.println(nome + " está miando!");
    }
}

public class Main {
    public static void main(String[] args) {
        Gato meuGato = new Gato();
        meuGato.nome = "Larry";
        meuGato.fazerSom(); // Método herdado da classe Animal
        meuGato.miar();    // Método específico da classe Gato
    }
}
```

### Polimorfismo

O polimorfismo permite que um método tenha diferentes comportamentos, dependendo do objeto que o chama. Pode ocorrer por sobrescrita (override) ou sobrecarga (overload).

```java
class Animal {
    void fazerSom() {
        System.out.println("O animal faz um som.");
    }
}

class Gato extends Animal {
    @Override
    void fazerSom() {
        System.out.println("O gato mia.");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal meuAnimal = new Animal();
        meuAnimal.fazerSom(); // Chama o método da classe Animal

        Animal meuGato = new Gato();
        meuGato.fazerSom(); // Chama o método da classe Gato
    }
}
```

## Parte 4 - Mercado de Trabalho para Desenvolvedores Java

### Áreas de Atuação do Java

O Java é uma linguagem versátil, utilizada em diversas áreas, incluindo:

* Desenvolvimento Web
* Aplicações Empresariais
* Big Data e Análise de Dados​
* Aplicações Móveis
* Sistemas Embarcados

### Tecnologias e Frameworks Populares em Java

Entre as tecnologias e frameworks frequentemente requisitados por empresas que buscam programadores Java, destacam-se:

* Spring Framework
* Hibernate
* JavaServer Faces (JSF)
* Apache Struts
* Maven

### Salário Médio de Desenvolvedores Java no Brasil

Os salários para desenvolvedores Java no Brasil variam conforme o nível de experiência:

* Júnior: A média salarial é de aproximadamente R$ 2.800 por mês
* Pleno: O salário médio é de cerca de R$ 5.733 mensais
* Sênior: A média salarial é de aproximadamente R$ 9.358 por mês
