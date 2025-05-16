<!-- 
import java.util.Scanner;

public class palindrome {

    public static void main(String[] args) {
        
        Scanner input=new Scanner(System.in);
        System.out.println("Enter the string: ");
        String s = input.nextLine();
           
     String rev="";
     for(int i=s.length()-1;i>=0;--i){
         rev=rev+s.charAt(i);
     }
     System.out.println(rev);
     if(rev.equalsIgnoreCase(s)){
         System.out.println("Palindrome");
     }else{
         System.out.println("Not palindrome");
     }
    input.close();
    }
} -->



import java.util.Scanner;

/**
 *
 * @author Vidhikara
 */
public class checkPrime {

    public static void main(String[] args) {
        Scanner scn=new Scanner(System.in);
        int n=scn.nextInt();
        if(n<2){
            System.out.println("Not a prime!! ");
            scn.close();
                return;
        }
        for(int i=2;i<=n/2;i++){
            if(n%i==0){
                System.out.println("Not a prime!! ");
                scn.close();
                return;
            }
        }
        
       System.out.println("Number is Prime!! ");
       scn.close();
    }
    
}