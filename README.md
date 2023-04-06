# atividade-de-PAM-Livia-Cremonez-e-Matheus-Garcia

Tipos de Dados por valor e por referência em Java.

Em desenvolvimento de programas nós sempre precisamos guardar na memória os valores, que pode ser sempre um nome, uma data, ou pode ser qualquer outro tipo de informação, assim podem ser declaradas que nós conhecemos como variáveis que atribuem estes valores em tempo de execução do sistemas.

Variáveis 

As variáveis são as posições na memótia do computador que podemos armazenar dados. 
As variáveis são formadas por quatro elementos:
Nome, tipo, tamanho e valor.
Dependendo da programação, o básico de uma declaraçao de variável pode ter somente um tipo, um nome ou um valor.

LISTAGEM 1: Exemplo de declaração de variável.

 public class Imprime_Variaveis {

	public static void main(String[] args) {
		
		int valorA = 33;
		int valorB = 25;
		
		int total = valorA + valorB;		
		
		System.out.printf("A soma total = %d",total);
	}

}


O java possui dois tipos de dados que são divididos em POR VALOR (tipos primitivos) e POR REFERÊNCIA (tipos por referência). 
Os tipos primitivos são:
Boolean, Byte, Char, Short, Int, Long, Float e Double.

Os tipos por referência são classes que especificam os tipos de objeto STRINGS, ARRAYS PRIMITIVOS e OBJETOS.

Uma variável do tipo primitivo elas podem armazenar exatamente um valor de seu tipo declarado por sua vez, quando outro valor for atribuido a essa variável, seu valor inicial será substituido.

Variáveis de instância de tipo primitivo elas são inicializadas por padrão, as variáveis dos tipos byte, char, short, int, long, float e double essas são inicializadas como 0, e as variáveis do tipo boolean são inicializadas como False., esses tipos eles podem especificar o seu próprio valor inicia para uma vriável do tipo primitivo atribuindo á variável um valor na sua declaração.

A linguagem Java fornece dois tipos primitivos para armazenar números de ponto flutuante na memória, o tipo float e double.

FLOAT: essa variável números com pontos flutuantes (reais) com precisão simples.
DOUBLE: essa variável números com ponto flutuante, com precisão dupla, ou seja normalmente possui o dobro da capacidade d euma variãvel de tipo float.


  LISTAGEM 2: Exemplo dos tamanhos de tipos primitivos.



public class Tipos_de_Dados {


	public static void main(String[] args) {
		System.out.println("Tipos de dados em Java: \n" +
	            "\nMenor Byte: " + Byte.MIN_VALUE +
	            "\nMaior Byte: " + Byte.MAX_VALUE +
	            "\nMenor Short Int: " + Short.MIN_VALUE +
	            "\nMaior Short Int: " + Short.MAX_VALUE +
	            "\nMenor Int: " + Integer.MIN_VALUE +
	            "\nMaior Int: " + Integer.MAX_VALUE +
	            "\nMenor Long: " + Long.MIN_VALUE +
	            "\nMaior Long:" + Long.MAX_VALUE +
	            "\nMenor Float: " + Float.MIN_VALUE +
	            "\nMaior Float: " + Float.MAX_VALUE +
	            "\nMenor Double: " + Double.MIN_VALUE +
	            "\nMaior Double: " + Double.MAX_VALUE);

	}

}


LISTAGEM 3: Declaração dos tipos primitivos.

public class Tipos_Primitivos {
	public static void main(String[] args) {
	      byte tipoByte = 127;
	      short tipoShort = 32767;
	      char tipoChar = 'C';
	      float tipoFloat = 2.6f;
	      double tipoDouble = 3.59;
	      int tipoInt = 2147483647;
	      long tipoLong = 9223372036854775807L;
	      boolean tipoBooleano = true;
	      System.out.println("Valor do tipoByte = " + tipoByte);
	      System.out.println("Valor do tipoShort = " + tipoShort);
	      System.out.println("Valor do tipoChar = " + tipoChar); 
	      System.out.println("Valor do tipoFloat = " + tipoFloat);
	      System.out.println("Valor do tipoDouble = " + tipoDouble);
	      System.out.println("Valor do tipoInt = " + tipoInt);
	      System.out.println("Valor do tipoLong = " + tipoLong);
	      System.out.println("Valor do tipoBooleano = " + tipoBooleano);
	}

}


Na listagem 3 o tipo declarado como Char é sempre declaradocom aspas simples porque o tamanho é só de um 1 caractere, os tipos Float sempreirão possuir o caractere “ F ” no final do valor para sua identificação, sendo a mesma coisa com o tipo long só que é inserido o caractere “ L ”.

Tipos po referência.

Os programas utilizam as variáveis de tipos por referência para armazenar as localizações de objetos na memória do computador.

Os objetos que são referência podem conter várias variáveis de instância e métodos dentro do objeto apontado.

Para trazer em um objeto os seus métodos de instância, é preciso ter referência a algum objeto, as variáveis de referência são inicializadas com o valor “ null ”(nulo).

Um exemplo é, ClasseConta acao = new ClasseConta(), cria um objeto de classe ClasseConta e a variavel acao contém uma referência a esse objeto ClasseConta, onde podemos invocar todos os seus métodos e atributos da classe. A palavra chave new ela solicita a memó do sistema para armazenar um objeto e inicializa o objeto.





LISTAGEM 4: Exemplo acessando um método do objeto.
 

 public class AcessaMetodo {

	public void imprime(){
		System.out.println("Bem Vindo ao Java!");
	}

	public static void main(String[] args) {
		AcessaMetodo acessa = new AcessaMetodo ();
		acessa.imprime();

	}

}

A saida  desse código acima irá ser reproduzida através da ação acessa.imprime(), porque está sendo acessado o método do objeto que foi inicializado com a variavel definida com “ acessa ”.


Componentes visuais da plataforma Android.

A platafoma Android, como muitos dizem é um verdadiro paraiso falando de interface grafica, com contem dezenas de componntes visuais sofisticados com efitos que contem muitas caracteristicas disponiveis para serem personalizadas, essa plataforma está se tornando uma referência na quantidade e na qualidade dos componentes visuais existentes.

Os componentes visuais no Android são definidos a partir de tags no arquivo XMLde loyout, e possuem classes correspondentes para que possa ser usada no código Java (Activity).

Para um melhor entendimento, pode-se dividir os componentes visuiais em seis grupos:

VIEWS básicas: composto de componentes básicos, como caixa de texto e botões; 
PICKERS Views: componentes especiais que permitem ao usuário selecionar os dados a partir de uma fonte de dados específica;
VIEWS de listas: componentes que mostram uma lista deinformações;
VIEWS para imagens: componentes utilizados para tratamento e apresentação de
 imagens;
MENUS: formados por opções de menu;
EXTRAS: componentes especiais com funções muito especificas.



Estrutura condicional
 Dão a possibilidade do programa tomar decisões e fazer mudanças em sua execução, possibilitando o controle dos códigos executados conforme as determinadas situações, como analise de expressões booleanas, valores variáveis. Conforme tais funções forem verdadeiras, uma parte é executada, caso seja falsa outro trecho será executado.

If else 
Estrutura de condição mais conhecida, tem a função de analisar a expressão booleana (verdadeiro ou falso). O else define a execução quando a condição for falsa, já o if analisa a condição mostrando se é verdadeira. Caso a condição dentro do if  seja verdadeira ela será executada, sendo assim o else não será executado. Caso if seja falso o else definirá o que vai ser executado. 

public class Exemplo {
	
    public static void main(String[] args) {
        int resposta = 10;
        if (resposta == 10) { 
            System.out.println(“A resposta é exatamente 10!”);
        } else if (resposta > 10) {
            System.out.println(“A resposta é maior que 10!”);
        } else {
            System.out.println(“A resposta é menor que 10!”);
        }
    }
	
}

Switch Case	 
Funciona como opção quando precisamos utilizar diversos ifs durante o código, o que acaba fazendo dele uma estrutura condicional importante, uma vez que if repetidos deixa o código não legível e grande. Testa o valor de uma variável e compara com as opções. Essas opções são determinadas pela instrução case que também deve ter seu final determinado, para isso utilizamos a palavra break.

ublic class Exemplo {
	
    public static void main(String[] args) {
        int mes = 2;
        switch (mes) {
            case 1:
                System.out.println(“O mês é janeiro”);
                break;
            case 2:
                System.out.println(“O mês é fevereiro”);
                break;
            case 3:
                System.out.println(“O mês é março”);
                break;
            case 4:
                System.out.println(“O mês é abril”);
                break;
            case 5:
                System.out.println(“O mês é maio”);
                break;
            case 6:
                System.out.println(“O mês é junho”);
                break;
            case 7:
                System.out.println(“O mês é julho”);
                break;
            case 8:
                System.out.println(“O mês é agosto”);
                break;
            case 9:
                System.out.println(“O mês é setembro”);
                break;
            case 10:
                System.out.println(“O mês é outubro”);
                break;
            case 11:
                System.out.println(“O mês é novembro”);
                break;
            case 12:
                System.out.println(“O mês é dezembro”);
                break;
            default:
                System.out.println(“Mês inválido”);
                break;
        }
    }
	
}

Estrutura de repetição 
Mais conhecidas como loops, as estruturas de repetição tem a funcionalidade de execução repetidamente de instruções enquanto uma condição estiver sendo feita. 
For 
Executa um ciclo do programa por determinado tempo ou por determinada condição pré-estabelecida, e na quantidade de vezes determinada. 

public class Exemplo {
	
    public static void main(String[] args) {
        for (int i = 0; i <= 10; i++) {
            System.out.println(“A variável i agora vale “ + i);
        }
    }
	
}

While 
É uma estrutura de repetição que utilizamos quando não se tem um número de repetições do código determinado, para que esse processo pare utilizamos uma condição booleana.

while (<condição>) {
    // Trecho de código a ser repetido
}
 
While utilizando boolean
package br.com.treinaweb;

import java.util.Scanner;

public class Exemplo {
	
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        int numero = -1;
        while (numero != 10) { 
// enquanto a variável não for 10, o trecho de código será repetido
            System.out.println(“Digite um número: “);
            numero = in.nextInt();
            if (numero == 10) {
                System.out.println(“Você acertou!“);
            } else {
                System.out.println(“Você errou :(“);
            }
        }
    }
								   
}





