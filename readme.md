**SOLID:**
1. [x] Single Responsibility Principle
2. [x] Open Closed Principle
3. [x] Liskov Substitution Principle
4. [x] Interface Segregation Principle
5. [x] Dependency Inversion Principle

**1- Orientação a Objetos:**

_Coesão:_
* Uma classe coesa faz bem uma única coisa
* Classes coesas não devem ter várias responsabilidades

_Encapsulamento:_

* Getters e setters não são formas eficientes de aplicar encapsulamento
* É interessante fornecer acesso apenas ao que é necessário em nossas classes
* O encapsulamento torna o uso das nossas classes mais fácil e intuitivo

_Acoplamento:_

* Acoplamento é a dependência entre classes
* Acoplamento nem sempre é ruim, e que é impossível criar um sistema sem nenhum acoplamento
* Devemos controlar o nível de acoplamento na nossa aplicação

**2- Melhorando a coesão**

* Classes/métodos/funções/módulos devem ter uma única responsabilidade bem definida;
* Segundo o Princípio de Responsabilidade Única (SRP), uma classe deve ter um e apenas um motivo para ser alterada;

**3- Reduzindo o acoplamento**

_Open Closed Principle_

* Embora complexo em sua definição, é muito útil e pertinente.
* Garantir que o sistema seja extensivel.
* Para garantir que nosso sistema seja extensivel da forma correta, devemos garantir que cada ação/responsabilidade esteja na classe correta.
* Cada classe deve conhecer e ser responsável por suas próprias regras de negócio;
* O princípio Aberto/Fechado (OCP) diz que um sistema deve ser aberto para a extensão, mas fechado para a modificação
  Isso significa que devemos poder criar novas funcionalidades e estender o sistema sem precisar modificar muitas classes já existentes
* Uma classe que tende a crescer "para sempre" é uma forte candidata a sofrer alguma espécie de refatoração.

**04- Liskov Substitution Principle**

* Embora a herança favoreça o reaproveitamento de código, ela pode trazer efeitos colaterais quando não utilizada da maneira correta;
* O princípio de Substituição de Liskov (LSP) diz que devemos poder substituir classes base por suas classes derivadas em qualquer lugar, sem problema.

**05- Dependency Inversion Principle.**

_Vantagem ao criar dependências com interfaces_

* Se um método muda a forma como realiza sua tarefa, desde que a interface se mantenha, não vamos precisar nos preocupar nem em editar o nosso códig.

_Interface Segregation Principle_

* Uma classe não deve ser obrigada a implementar um método de determinada interface, se ele não será útil. Para isso, uma interface deverá ser extraída apenas com os métodos necessários.

**Resumo**

* É mais interessante e mais seguro para o nosso código depender de interfaces (classes abstratas, assinaturas de métodos e interfaces em si) do que das implementações de uma classe;
* As interfaces são menos propensas a sofrer mudanças enquanto implementações podem mudar a qualquer momento;
* O Princípio de Inversão de Dependência (DIP) diz que implementações devem depender de abstrações e abstrações não devem depender de implementações;
* As interfaces devem definir apenas os métodos que fazem sentido para seu contexto;
* O Princípio de Segregação de Interfaces (ISP) diz que uma classe não deve ser obrigada a implementar um método que ela não precisa;