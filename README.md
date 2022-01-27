# Exercicios



Informar todos os números de 1000 a 1999 que quando divididos por 11 obtemos resto = 5. (FOR)

import java.util.Random;

public class Exec1 {
    public static void main(String[] args) {
        int num_aleatorio;
        
       
        for(int count=1 ; count <= 20 ; count++){
            
            Random randomGenerator = new Random();
       
            num_aleatorio = randomGenerator.nextInt(1000) + 1000;
            
            if(num_aleatorio % 11 == 5)
                System.out.println(num_aleatorio);
        }
    }
}



Ler 10 números e imprimir quantos são pares e quantos são ímpares. (FOR)



package cap14;




import java.util.Scanner;







public class Exerc2 {


   public static void main(String[] argss){


       Scanner ent = new Scanner(System.in);


       int num, contPar = 0, contImpar = 0;


      


       for(int i = 1; i <= 5; i++){


           System.out.println("Digite o " + i + "º número");


           num = ent.nextInt();


          


           if(num % 2 == 0){


               contPar++;


           }










           


           if(num % 2 == 1){


               contImpar++;


           }


           


       }


      


       System.out.println("Foram digitados " + contPar + " números pares \n");


       // System.out.println("E " + contImpar + " números ímpares");


      


   }


}





Solicitar a idade de várias pessoas e imprimir: Total de pessoas com menos de 21 anos. Total de pessoas com mais de 50 anos. O programa termina quando idade for =-99. (WHILE)


import java.io.IOException;
import java.util.Scanner;
public class Exerc3 {
  public static void main(String[] args) throws IOException {
    Scanner leitor = new Scanner(System.in);
    int cont = 0;
    double soma = 0;
    double n=0;
  
    while (n >= 0) {
      n = leitor.nextInt();
      if (n >= 0) { 
       cont++;
       soma+=n;
      }
    }
    double media = soma / cont;
    System.out.println(String.format("%.2f", media));
  }
}





Uma empresa desenvolveu uma pesquisa para saber as características psicológicas dos indivíduos de uma região. Para tanto, a cada uma das pessoas era perguntado: idade, sexo (1-feminino / 2-masculino / 3-Outros), e as opções (1, se a pessoa era calma; 2, se a pessoa era nervosa e 3, se a pessoa era agressiva). Pede-se para elaborar um sistema que permita ler os dados de 150 pessoas, calcule e mostre: (WHILE)
o número de pessoas calmas; 
o número de mulheres nervosas; 
o número de homens agressivos; 
o número de outros calmos;
o número de pessoas nervosas com mais de 40 anos; 
o número de pessoas calmas com menos de 18 anos.


Crie um programa que leia um número do teclado até que encontre um número igual a zero. No final, mostre a soma dos números digitados.(DO...WHILE)


public class Exerc5 {

    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
       
        System.out.println("Digite o seu nome: ");
        String nome = in.nextLine();
         
            System.out.println("Informe a sua idade: ");
            int idade = in.nextInt();
           
            System.out.println("Informe a sua cidade de nascimento: ");
            String cidade = in.next();

            System.out.print("Ola. Meu nome é "+nome);
            System.out.print(", sou natural de "+cidade);
            System.out.print(", tenho "+idade);
            System.out.print(" anos, e estou aprendendo a programar.");
    }
}



Escrever um programa que receba vários números inteiros no teclado. E no final imprimir a média dos números múltiplos de 3. Para sair digitar 0(zero).(DO...WHILE)

public class Exerc6 {
public static void main(String[]args){
	
	for(int i=1 ; i<=100 ; i++){
		if(i % 3 ==0){
			System.out.println(i);
		}
	}
}

}
