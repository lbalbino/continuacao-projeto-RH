# continuacao-projeto-RH

import java.util.Scanner;

```java
public class Principal {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);        
        Pessoas pessoa = new Pessoas();

        System.out.println("Qual seu Nome? ");
        String nome = sc.nextLine();
        System.out.println("Qual é a sua idade?");
        int idade = sc.nextInt();
        System.out.println("Qual é o seu cpf?");
        String cpf = sc.nextLine();
        System.out.println("Qual é o seu rg?");
        int rg = sc.nextInt();

        pessoa.Set_Nome(nome);
        pessoa.Set_Idade(idade);
        pessoa.Set_Cpf(cpf);
        pessoa.Set_rg(rg);

        System.out.println("Olá " + pessoa.Get_Nome());
        System.out.println("Sua Idade é: " + pessoa.Get_Idade() + " Anos.");
        System.out.println("Portador do CPF: " + pessoa.Get_Cpf());
        System.out.println("Portador do Rg: " + pessoa.Get_rg());
    }

}

public class Pessoas {
    private String nome;
    private int idade;
    private String cpf ;
    private int rg ;
    private String dataNacimento;
    
    
     public String Set_Nome(String nome) {
        return this.nome = nome;
    }
    public String Get_Nome() {
        return this.nome;
    }

     public String Set_Cpf(String cpf) {
        return this.cpf = cpf;
    }

    public String Get_Cpf() {
        return this.cpf;
    }

     public int Set_rg(int rg) {
        return this.rg = rg;
    }

    public int Get_rg() {
        return this.rg;
    }
    
    public int Set_Idade (int idade) {
        return this.idade = idade;
    }
     
    public int Get_Idade () {
        return this.idade;
    }
    
        
}

```
