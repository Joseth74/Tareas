
package tarea;


public class Persona {
    private String nombre;
    private int edad;
    private String cedula;
    private char sexo;
    private double peso;
    private double altura;


    public Persona(String nombre, int edad,String cedula,char sexo) {
        this.nombre = nombre;
        this.edad = edad;
        this.cedula = cedula;
        this.sexo = sexo;
    }
    
     
    public Persona(double peso, double altura ){
    this.peso = peso;
    this.altura = altura;
    
    }

   
     
public void Datos(){
System.out.println("El nombre es: "+nombre);    
System.out.println("La edad es: "+edad);
System.out.println("La cedula es: "+cedula);
System.out.println("El sexo es: "+sexo);
}

}


package tarea;
import java.util.Scanner;
public class Main {
    public static void main(String [] args){ 
    
        
        Persona persona1 = new Persona("Andres",25,"401-190865-0008x",'H');
      
    persona1.Datos();
   
  
        

    Scanner sc=new Scanner (System.in);
        float kg,mts,imc,x;
        System.out.print("Cual es tu peso? (Kg) ");
        kg=sc.nextFloat();
        System.out.print("Cual es tu altura? (mts) ");
        mts=sc.nextFloat();
        imc=mts*mts;
        x=kg/imc;
        System.out.println("Tu indice de masa corporal es: "+x);
        if(x<=18){
            System.out.println("-1");
        }else if(x>=18 && x<=24.9){
            System.out.println("0");
        }else if(x>=25 && x<=26.9){
            System.out.println("+1");
            
     
           
    
  }

 }
}


