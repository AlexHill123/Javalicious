# Javalicious
import java.util.Scanner;
/**
 * Birth year finder:
 * 
 * @author Alex Hill
 * @version May 1st 2018
 */


public class java {

public static void main(String[] args) {
    
 // this is the current year   
 int year = 2018;   
    
 // variable for later
 int age = 0;
 
 // string for later
 String yesOrNo = "";
 
     // next two lines ask for your age and save it
     System.out.println("How old are you");
     age = yourAge();
     
     // prints your age
     System.out.println("You are " + age + " years old");
     
     // asks if you would like to know when you were born
     System.out.println("Would you like to know what year you were born?");
     
     // user inputs yes or no
     Scanner keyboard = new Scanner(System.in);
    yesOrNo = keyboard.nextLine();
     
    // validating if statment
    if(  yesOrNo.equals("yes")) {
     
        System.out.println("This was the year you were born: " 
                          + year(age) + " give or take a year.");
     // what happens if you say anything but yes                       
    } else {
        
        System.out.println("Have a nice day");
    }
        
        
}


/*
 * Obtaining the users age
 * 
 * @return a which is the users age
 */
public static int yourAge (){
 
    int a = 0;
    
    Scanner in = new Scanner(System.in);
    
    a = in.nextInt();
    return a;
}

/*
 * Obtaining the users age
 * 
 * @param age what age the user is
 * @return year which is when you were born
 */
        public static int year(int age) {
            
          int  theYear = 0;
           
           theYear = 2018 - age;
           
           return theYear;
}
}
