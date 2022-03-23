# miniproject

import java.util.*;

public class my{
   
    public static void main(String[] args){
        Scanner scn = new Scanner(System.in);
      
        int myNumber = (int)(Math.random()*100);

        int UseNumber ;

        do{
            System.out.println("Guess my number : ");
            UseNumber = scn.nextInt();

            if(UseNumber == myNumber)
            {
                System.out.println("WOOHOO ... Correct Number !");
                break;
            }
            else if(UseNumber > myNumber){
                System.out.println("Your number is too large !");
            }else{
                System.out.println("Your number is too small !");
            }
        }
        while(UseNumber >= 0);

        System.out.println("My number was : ");
        System.out.println(myNumber);
    }
}
