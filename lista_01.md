# Instruções

- Faça uma cópia deste arquivo .md para um repositório próprio
- Resolva as 6 questões objetivas assinalando a alternativa correta
- Resolva as 4 questões dissertativas escrevendo no próprio arquivo .md
  - lembre-se de utilizar as estruturas de código como ``esta aqui com ` `` ou
```javascript
//esta aqui com ```
let a = "olá"
let b = 10
print(a)
```
- Resolva as questões com uso do Visual Studio Code ou ambiente similar.
- Teste seus códigos antes de trazer a resposta para cá.
- Cuidado com ChatGPT e afins: entregar algo só para ganhar nota não faz você aprender e ficar mais inteligente. Não seja dependente da máquina!
- ao final, publique seu arquivo lista_01.md com as respostas em seu repositório, e envie o link pela Adalove. 

# Questões objetivas

**1)** O que o código a seguir faz?

![Uma imagem](assets/ex01.PNG)

Escolha a opção que responde corretamente:

**a) Imprime os números pares de 1 a 10.**

b) 

c) 

d) 

______

**2)** Identificar a linha que falta no código para criar uma classe Veiculo com atributo marca, e uma classe Carro que herda de Veiculo com um método ligar(). 

![Uma imagem](assets/ex02.PNG)

No lugar onde está escrito “// linha” qual das opções abaixo deve estar para funcionar corretamente o código?

**A) let carro = new Carro("Toyota");**

B) 

C) 

D) 

______

**3)** Qual é o valor de resultado após a execução deste código?

![Uma imagem](assets/ex03.PNG)

Escolha a opção que responde corretamente:

**A) 18**

B)

C) 

D) 

______

**4)** Como você criaria um método `acelerar()` em uma classe `Carro`, que recebe um parâmetro `velocidade` e o adiciona a um atributo `velocidadeAtual`?

**A) ![Uma imagem](assets/ex04_1.PNG)**

B) 

C) 

D) 

______

**5)** Qual a forma correta de definir uma classe Carro em JavaScript, com um método ligar() e um atributo marca?

**A) ![Uma imagem](assets/ex05_1.PNG)**

B) 

C) 

D) 

______

**6)** Observe o código abaixo:

![Uma imagem](assets/ex06.PNG)

Qual será a saída do código acima?

**A) "Olá, meu nome é João. Olá, meu nome é Maria."**

B) 

C) 

D)

______

# Questões dissertativas

**7)** Vamos criar um programa em JavaScript para entender classes, métodos e atributos!
Classe Animal:
- Crie uma classe chamada Animal.
- Adicione dois atributos: nome e idade.
- Adicione um método chamado descrever() na classe Animal.
  - Este método deve exibir no console uma descrição do animal com seu nome e idade.

Criando e manipulando Animais:
- Crie dois objetos da classe Animal: um chamado "cachorro" e outro "gato", com idades distintas.
- Para cada animal, chame o método descrever() para ver a descrição no console.

Dica: Utilize `console.log()` para exibir as informações!

```
class Animal { //Criando a classe Animal
    constructor(nome, idade) { // Definindo os atributos da classe
        this.nome = nome;
        this.idade = idade;
    }

    descrever() { // Criando o método
        console.log('O animal ' + this.nome + ' tem ' + this.idade + ' anos.');
    }
}

// Criando os objetos da classe animal
let cachorro = new Animal('Cachorro', 5); 
let gato = new Animal('Gato', 3);

cachorro.descrever(); // Chamando o console.log do objeto cachorro 
gato.descrever(); // Chamando o console.log do objeto gato 
```
______

**8)** Nos últimos dias tivemos a oportunidade de ter contato com Programação Orientada a Objetos, e tivemos contato com o tema "herança". Herança é um princípio de orientação a objetos, que permite que classes compartilhem atributos e métodos. Ela é usada na intenção de reaproveitar código ou comportamento generalizado ou especializar operações ou atributos. Então vamos praticar esse conteúdo nessa questão.
Vamos criar um programa em JavaScript para entender classes, métodos, atributos e herança!

Classe Animal:
- Crie uma classe chamada Animal.
- Adicione dois atributos: nome e idade.
- Adicione um método descrever() que exiba no console uma descrição do animal com seu nome e idade.

Classe Gato (Herda de Animal):
- Crie uma classe chamada Gato que herda da classe Animal.
- Adicione um atributo extra cor específico para gatos.
- Adicione um método miar() que exiba no console o som que um gato faz.

Criando Animais:
- Crie dois objetos da classe Animal: um chamado cachorro e outro gato, com idades distintas.
- Para o gato, também defina a cor.

Chamando os Métodos:
- Para cada animal, chame o método descrever() para ver a descrição no console.
- Para o gato, chame o método miar() para "ouvir" o som que ele faz (é também para ver o som no console).

Dica: Utilize console.log() para exibir as informações!

```
// Criando a Classe Animal
class Animal {
    constructor(nome, idade) { // Adicionando os atributos solicitados
        this.nome = nome;
        this.idade = idade;
    }

    descrever() { // Criando o método
        console.log('O animal ' + this.nome + ' tem ' + this.idade + ' anos.');
    }
}
// Criando a classe Gato que herda da classe Animal
class Gato extends Animal {
    constructor(nome, idade, cor) { // Adicionando atributo extra
        super(nome, idade);
        this.cor = cor;
    }

    miar() { // Criando método do som
        console.log("Miau!");
    }

    descrever() { // Método descrever com o atributo cor
        console.log('O animal ' + this.nome + ' de cor ' + this.cor + ' tem ' + this.idade + ' anos.');
    }
}

// Criando os objetos da classe Animal 
let cachorro = new Animal("Cachorro", 5);
let gato = new Gato("Gato", 3, "Preto");

// Chamando os Métodos
cachorro.descrever();
gato.descrever(); 
gato.miar(); // Saída: Miau!
```

______

**9)** Vamos criar um programa em JavaScript para somar notas!

Classe SomadorDeNotas:
- Crie uma classe chamada SomadorDeNotas.
- Adicione um atributo total inicializado com 0 para armazenar a soma das notas.

Método adicionarNota:
- Adicione um método chamado adicionarNota(nota) na classe SomadorDeNotas.
- Este método deve receber um parâmetro nota e somá-lo ao atributo total.

Criando o Somador e Adicionando Notas:
- Crie um objeto da classe SomadorDeNotas, chamado somador.
- Utilize o método adicionarNota(nota) para adicionar algumas notas ao somador.

Chamando o Método para Ver o Total:
- Após adicionar todas as notas, chame um método verTotal() para exibir o total das notas adicionadas.

Dica: Utilize console.log() para exibir as informações!

```
// Criando a classe SomadorDeNotas
class SomadorDeNotas {
    constructor() {
        this.total = 0;
    }

    adicionarNota(nota) { // Criando o método na classe 
        this.total += nota;
    }

    verTotal() {
        console.log('A soma total das notas é: ' + this.total);
    }
}
// Criando o Somador usando a classe 

let somador = new SomadorDeNotas();
somador.adicionarNota(8); //Usando o método pra incluir as notas
somador.adicionarNota(9.5);
somador.adicionarNota(7.2);

// Chamando o Método 
somador.verTotal(); 
```
______

**10)** Imagine que você está criando um programa em JavaScript para uma escola. Neste programa, existem diferentes tipos de funcionários, cada um com suas próprias características. Considere as seguintes classes:

Funcionário:
- atributo: Nome
- atributo: Idade
- atributo: Salário base
- método: calcularSalario() - Este método calcula o salário total do funcionário. Para cada tipo de funcionário, o cálculo será diferente.

Professor (herança de Funcionário):
- atributo: Disciplina
- atributo: Horas de aula por semana
- método: calcularSalario() - Para calcular o salário do professor, multiplicamos suas horas de aula pelo valor da hora/aula.

Agora, sua tarefa é escrever um código em JavaScript que crie as classes Funcionário e Professor, com suas características e métodos descritos acima. Depois de criar as classes, crie:
- Dois objetos do tipo Professor com informações fictícias.
- Para cada objeto, chame o método calcularSalario() e mostre o salário calculado no console.

```
// Criando a classe Funcionário
class Funcionario {
    constructor(nome, idade, salarioBase) { // Definindo atributos pra classe
        this.nome = nome; 
        this.idade = idade;
        this.salarioBase = salarioBase;
    }

    calcularSalario() { // Criando método
        return this.salarioBase;
    }
}

// Classe Professor, que herda da classe Funcionário
class Professor extends Funcionario {
    constructor(nome, idade, salarioBase, disciplina, horasAula) { // Adicionando atributos da classe mãe e também extras
        super(nome, idade, salarioBase);
        this.disciplina = disciplina;
        this.horasAula = horasAula;
    }
 
    calcularSalario() { //Método pra calcular salário
        return this.salarioBase * this.horasAula;
    }
}

// Criando objetos do tipo Professor
let professor1 = new Professor("João", 40, 3000, "Matemática", 20);
let professor2 = new Professor("Maria", 35, 3500, "História", 15);

// Chamando o método calcularSalario() para calcular o salário de cada objeto da classe Professor
console.log('O salário do professor ' + professor1.nome + ' é R$ ' + professor1.calcularSalario());
console.log('O salário do professor ' + professor2.nome + ' é R$ ' + professor2.calcularSalario());
```

Certifique-se de explicar cada parte do código utilizando comentários, explicando para que serve cada atributo e método, bem como a lógica por trás do cálculo de salário para o tipo de funcionário Professor.