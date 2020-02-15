# Calculator
import java.util.*;
import java.lang.*;
import java.io.*;
class Calculator
{
    public static void main(String[] args) {
      Scanner sc=new Scanner(System.in);
      System.out.println("Enter numbers to perform operation on them");
      int num1=sc.nextInt();
      int num2=sc.nextInt();
      Calculator c=new Calculator();
c.getResult(num1,num2);
}
void getResult(int number1,number2){
      System.out.println("Choose operation to be formed ");
      System.out.println("1.Addition");
      System.out.println("2.Multiplication");
      System.out.println("3.Subtraction");
      System.out.println("4.Division");
      int select=sc.nextInt();
      switch(select)
      {
          case 1: int k1=number1+number2;
                   System.out.println("Sum of given numbers "+number1+" and "+number2+" is "+k1);
                   break;
          case 2: int k2=number1-number2;
                   if(k2>0)
                   {
                   System.out.println("Difference of given numbers "+number1+" and "+number2+" is "+k2);
                   }
                   else
                   {
                   System.out.println(" Subtraction cannot be performed ");
                   }
                   break;
          case 3: int k3=number1*number2;
                   System.out.println("Product of given numbers "+number1+" and "+number2+" is "+k3); 
                   break; 
          case 4: 
                if(number2!=0)
                {
                   int k4=number1/number2;
                   System.out.println("Division of given numbers "+number1+" and "+number2+" is "+k4); 
                }
                else
                {
                      System.out.println("Division cannot be performed");
                }     
                   break;
          default:  System.out.println("No operation to perform");
                     break;                           
      }
    }
}
