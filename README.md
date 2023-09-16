# Condicionais-If-Else-no-java

Anotações de Condicionais If Else no java

                                                                      Condicionais If-Else
Agenda
.O que é controle de decisão
.IF(se)
.IF - ELSE(se-senão)
.Múltiplos if-else

                                                                           Comando IF

.Comandos dentro de um bloco IF somente são executados se a condição for verdadeira.
.Se a condição for falsa, os comandos não são executados.

A dente vai fazer o programa assim.


public class IfQuadrinho {

	public static void main(String[] args) {

		boolean temBatata = true;
		int ovos = 6;

		if (temBatata){
		    ovos = 9;
                }

		System.out.println("Compre" + ovos + " ovos.");
	}

}


Nesse código nós iremos comprar 6 ovos e se tiver batatas vamos comprar 9 ovos.
então é justamente isso o que o IF quer dizer, se uma condicional for verdadeira a gente executa a lógica de programação o código que está dentro do IF se
não for verdadeira aquilo não é eecutado.

if (idade >= 18){
    System.out.println("É maior de idade");

-

package CondicionaisIfElseTeste;

import java.util.Scanner;

public class IfElse {

	public static void main(String[] args) {
		
		Scanner scan = new Scanner(System.in);
		
		System.out.println("Entre com sua idade");
		
		int idade = scan.nextInt();
		
		if (idade >= 18) {
			System.out.println("É maior de idade.");
		}
	}

}

Console:
Entre com sua idade
20

É maior de idade.


                                                                        Comando If-Else

.Comandos dentro de um bloco ELSE somente são executados se a condição do IF for falsa.

package CondicionaisIfElseTeste;

import java.util.Scanner;

public class IfElse {

	public static void main(String[] args) {
		
		Scanner scan = new Scanner(System.in);
		
		System.out.println("Entre com sua idade");
		
		int idade = scan.nextInt();
		
		if (idade >= 18) {
			System.out.println("É maior de idade.");
		} else {
			System.out.println("Não é maior de idade.");
		}
	}

}

Console:
Entre com sua idade
10
Não é maior de idade.


                                                                        Múltiplos IF-ELSE
.É possível ter vários if-else aninhados!


package CondicionaisIfElseTeste;

import java.util.Scanner;

public class IfElse {

	public static void main(String[] args) {
		
		Scanner scan = new Scanner(System.in);
		
		System.out.println("Entre com sua idade");
		
		int idade = scan.nextInt();
		
		if (idade >= 18) {
			System.out.println("É maior de idade.");
		} else {
			System.out.println("Não é maior de idade.");
		}
		
		//barato <= 10
		//10 < valor < 15 - pedir desconto
		//15 <= valor 17 - pesquisar mais
		//>= 17 - muito caro
		
		System.out.println("Entre com o preço do item");
		double valor = scan.nextDouble();
		
		if (valor <= 10) {
			System.out.println("Está barato, pode comprar");
		} else if (valor > 10 && valor < 15) {
			System.out.println("Você pode pedir um desconto");
		} else if (valor >= 15 && valor < 17) {
			System.out.println("Pode pesquisar mais");
		} else {// valor >=17
			System.out.println("Muito caro");
		}
	}

}
