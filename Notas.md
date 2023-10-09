# JAVA (POO)
  - [Conceitos](#conceitos)
  - [Encapsulamento](#encapsulamento)
  - [Agregação](#agregação)
  - [Associação](#associação)
  - [Interface gráfica](#interface-grafica)


Aula do dia 17/08/2023

# Conceitos

A Programação Orientada a Objetos é formada por alguns itens: Classes, Objetos, Atributos, Métodos, Construtores (já visto em Engenharia de Software II)

# Encapsulamento

O	que	começamos	a	ver	nesse	capítulo	é	a	ideia	de	encapsular,	isto	é,	esconder	todos	os	membros	de
uma	 classe	,	 além	 de	 esconder	 como	funcionam	 as	 rotinas	 (no	 caso	métodos)	 do
nosso	sistema.

* Quando se insere uma variável, o java procura primeiro localmente e depois globalmente
* É interessante o getters/setters serem públicos
* Alt + insert ->  Criação dos getters e setters

# Agregação

Num relacionamento de Agregação, podemos entender que classes que são agregadas por outras não precisam destas para “viver”, para “existir”. Por exemplo, a classe Unha agrega a classe Corpo Humano. Sem a unha o corpo humano vive sem grandes dificuldades.

````
Obs: Não deixa de ser uma associação
````


Pilha = variáveis
Heap = conteúdo

| Pilha          | Heap |
| -------------  | ------------- |
| F1             | Classe Func  |
| Filho          | Classe Filho  |


# Associação

A associação entre dois objetos ocorre quando eles são completamente independentes entre si mas eventualmente estão relacionados.

# Construtores

Quando	usamos	a	palavra	chave		new	,	estamos	construindo	um	objeto.	Sempre	quando	o		new		 é
chamado,	ele	executa	o	construtor	da	classe.	O	construtor	da	classe	é	um	bloco	declarado	com	o mesmo
nome	que	a	classe

    class Conta	{
				String	titular;
				int	numero;
				double	saldo;
				//	construtor
				Conta()	{
						System.out.println("Construindo	uma conta.");
				}
    }
Então,	quando	fizermos:
Conta	c	=	new	Conta();
A	mensagem	"construindo	uma	conta"	aparecerá.	É	como	uma	rotina	de	inicialização	que	é	chamada
sempre	que	um	novo	objeto	é	criado.	Um	construtor	pode	parecer,	mas	não	é	um	método.

# Collections

Estrutura de dados = armazena dados correlatos

A API de Collections traz a interface java.util.List , que especifica o que uma classe deve ser
capaz de fazer para ser uma lista

- List:
  - Acesso via índice
  - Ordem de entrada é igual a ordem de saída
  - Pode ter itens duplicados

Para criar uma lista, chame o construtor:  `ArrayList lista = new ArrayList();`

Para saber quantos elementos há na lista, usamos o método `size()` e o `get(int)` que recebe como argumento o índice do elemento que se quer
recuperar :
```
for(int i = 0; i < lista.size(); i++){
            System.out.println("Nome:[" + i + "]:" + lista.get(i));
        }
```

* *ForEach*

"for-each" (ou "enhanced for loop" em inglês) e é uma maneira simplificada de percorrer coleções de objetos em Java, como arrays e listas.

# Interface gráfica

*Criar projeto em FXML JavaFX Maven Archtype (Gluon)*

- FXML - tela
- CSS - estilos
- Controller - Gerenciamento
	- Os eventos que ocorrem dentro da tela (FXML) é gerenciado pelo controller

 Para renomear a classe App mude a linha 39 do pom.xml em project files
