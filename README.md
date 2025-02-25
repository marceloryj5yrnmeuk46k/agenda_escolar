<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport"
content="width=device-width, initial-scale=1.0">
<title>Página de Teste</title>
</head>
<body>
<h1>Bem-vindo ao GitHub Pages!</h1>
</body>
</html>


package aula_1;
import java.util.*;
public class teste {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		 Scanner sc = new Scanner(System.in);

		    int op, idade=0;

		 String nome = "a", curso = "a", turma = "a", data = "a", hora = "a",compromisso = "a" ;
		// iniciando o programa com while true para que o programa sempre volte ao menu principal
		    while (true){
		      // menu de opções da agenda
		      System.out.println("====== MENU ======");
		      System.out.println("1 - Cadastrar usuario");
		      System.out.println("2 - Cadastrar compromisso");
		    System.out.println("3 - mostrar agenda");
		      System.out.println("4 - fechar o progama");
		    op = sc.nextInt();

		    switch(op){
		      case 1: 
		        // case 1 serve para cadastrar um usuario
		      System.out.println("digite seu nome:");
		        nome = sc.next();
		               sc.nextLine();
		    System.out.println("digite sua idade: ");
		        idade = sc.nextInt();
		        sc.nextLine();
		      System.out.println("digite seu curso: ");
		        curso = sc.next();
		        sc.nextLine();
		      System.out.println("digite sua turma: ");
		        turma = sc.next();
		        sc.nextLine();
		      
		        break;
		      case 2: 
		        // case 2 serve para cadastrar um compromisso
		        System.out.println(" digite seu compromisso:  ");
		        compromisso = sc.next();
		        sc.nextLine();
		        System.out.println("digite a data: ");
		        data = sc.next();
		        sc.nextLine();
		        System.out.println("digite a hora: ");
		        hora = sc.next();
		        sc.nextLine();
		        
		        
		        break;
		      case 3:
		        // case 3 serve para mostrar a agenda. apenas pritando os dados que foram cadastrados
		    
		        if (idade == 0){
		        // esta condição serve para verificar se o usuario ja foi cadastrado
		        System.out.println("usuário não cadastrado");
		          }
		        else if (compromisso == "a"){
		    // esta condição serve para verificar se o usuario cacadastrou um compromisso
		          System.out.println("compromisso não cadastrado");}
		          
		       else
		          // se o usuário e o compromisso ja foram cadastrados, será mostrado a agenda
		        { System.out.println(" ========AGENDA========");
		        System.out.println("nome: " + nome);
		        System.out.println("compromisso: " + compromisso);
		        System.out.println("data: " + data);
		        System.out.println("hora: " + hora);}
		        break;
		                
		      
		   
		   }
		      if (op == 4)  {
		        // Esse if serve para fechar o programa, encerrando o laço de repetição 
		     System.out.println("progama encerrado");
		     break;
		   } 
		      
		    }
		  
		  }
		}
