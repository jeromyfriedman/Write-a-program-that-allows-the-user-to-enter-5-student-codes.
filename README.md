# Write-a-program-that-allows-the-user-to-enter-5-student-codes.
Write a program that allows the user to enter 5 student codes.
import java.util.Scanner;
 
public class BaiTapJavaCoBan10
{
    public static void main(String[] args)
    {
       String[] MSSV = new String[5];
       Scanner sc = new Scanner(System.in);
       for (int i = 0; i < 5; i++)
       {
          System.out.println("Enter the MSSV th " + (i+1) + ":");
          MSSV[i] = sc.nextLine();
       }

       for (int i = 0; i < 5; i++)
       {
          if (!MSSV[i].matches("B170[1-9]{4}"))
             System.out.println("The MSSV th " + (i+1) + " is wrong format!");
       }
    }
}
