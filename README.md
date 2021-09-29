import java.util.Scanner;
public class Main
{
   static Scanner sc = new Scanner(System.in);
   public static void main(String args[])
   {  

   int marks;
   while(true)
   {
   System.out.print("\nThis Is a Grade Checker Program");
   System.out.print("\nEnter The Marks Between 0 To 100:");
   
   System.out.print("\nEnter The Mark: ");
   marks = sc.nextInt();
   
   if(marks>100)
   {
    /* Marks greater than 100 */
    System.out.print("\ngrade not found\n");
   }
   else
   {
   switch(marks/10)
   {
       case 10 :
       case 9 :
           /* Marks between 90-100 */
           System.out.print("\nYour Grade Is: A or Excellent");
           break;
       case 8 :
       case 7 :
           /* Marks between 70-89*/
           System.out.print("\nYour Grade Is: B or Very Good" );
           break;
       case 6 :
           /* Marks between 60-69 */
           System.out.print("\nYour Grade Is: C or Fair" );
           break;
       case 5 :
       case 4 :
           /* Marks between 40-59 */
           System.out.print("\nYour Grade Is: D or Pass");
           break;
       default :
           /* Marks less than 40 */
           System.out.print("\nYou Grade Is: F or Fail\n");
           
   }
 }
}   
   }
}

