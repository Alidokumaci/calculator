import java.util.Scanner;

public class Test{
    public static void main(String[] args){
        Scanner scan = new Scanner(System.in);
        System.out.print("birinci sayiyi giriniz : ");
        double num1 = scan.nextDouble(); 

        System.out.print("ikinci sayiyi giriniz : ");
        double num2 = scan.nextDouble(); 

        System.out.print("bir islem seciniz (+ - / * ) : ");
        char operator = scan.next().charAt(0);

        double result = 0;

        if (operator=='+'){
            result=num1+num2;
        }else if (operator=='-'){
            result=num1-num2;
        }else if (operator=='*'){
            result=num1*num2;
        }else if (operator=='/'){
           if(num2==0){
            System.out.println("0 a bolme yapamam");
           }else{
            result=num1/num2;
           }
        } else{
            System.out.println("kullanilmayan operator girdiniz");
        }
           
        System.out.println("islemin sonucu : " + result);
           

    }
}
