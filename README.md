# Calculator
import java.util.*;
import java.lang.*;
import java.io.*;
class Calculator
{
    public static void main(String[] args)
    {
      Scanner sc=new Scanner(System.in);
      System.out.println("Enter numbers to perform operation on them");
      int n1=sc.nextInt();
      int n2=sc.nextInt();
      Calculator c=new Calculator();
      c.getResult(n1,n2);  
     }
    void getResult(int number1,number2)
    {
      System.out.println("Choose operation to be formed ");
      System.out.println("1.Addition");
      System.out.println("2.Multiplication");
      System.out.println("3.Subtraction");
      System.out.println("4.Division");
      int select=sc.nextInt();
      switch(select)
      {
          case 1: int ResultOfAdd=Addition(number1,number2);
                   System.out.println("Sum of given numbers "+number1+" and "+number2+" is "+ResultOfAdd);
                   break;
          case 2: 
                   if(number1>number2)
                   {
                   int ResultOfSub=Subtraction(number1,number2);
                   System.out.println("Difference of given numbers "+number1+" and "+number2+" is "+ResultOfSub);
                   }
                   else
                   {
                   System.out.println(" Subtraction cannot be performed ");
                   }
                   break;
          case 3: int ResultOfMul=Multiplication(number1,number2);
                   System.out.println("Product of given numbers "+number1+" and "+number2+" is "+ResultOfMul); 
                   break; 
          case 4: 
                if((number2)!=0)
                {
                   int ResultOfDiv=Division(number1,number2);
                   System.out.println("Division of given numbers "+number1+" and "+number2+" is "+ResultOfDiv); 
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
    int Addition(int num1,int num2)
    {
    return num1+num2;
    }
    int Subtraction(int num1,int num2)
    {
    return num1-num2;
    }
    int Multiplication(int num1,int num2)
    {
    return num1*num2;
    }
    int Division(int num1,int num2)
    {
    return num1/num2;
    }
}
