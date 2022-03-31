- 👋 Hi, I’m @Marianneguan
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Marianneguan/Marianneguan is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
/******************************************************************
 * Program 1: Conversion from binary to decimal representation
 * Programmer: Marianne Kate G. Guan
 * 
 * Class: IT 121        Instructor: 
 *        
 * Pledge: I have neither given nor received unauthorized aid
 * on this program.     (signature on file)
 *
 * Description: This program converts a binary number to decimal.
 *
 * Input: Binary number
 *
 * Output: Decimal number
 *
 ******************************************************************/

// Imported packages
   import java.util.Scanner;

    public class Binary
   {
   
   // Main method
       public static void main(String[] args)
      {
      	
  Scanner sc = new Scanner(System.in);
  long binaryNumber, decimalNumber = 0, j = 1, remainder;
  System.out.print("Input a binary number: ");
  binaryNumber = sc.nextLong();

  while (binaryNumber != 0) 
  {
   remainder = binaryNumber % 10;
   decimalNumber = decimalNumber + remainder * j;
   j = j * 2;
   binaryNumber = binaryNumber / 10;
  }
  System.out.println("Decimal Number: " + decimalNumber);
 }
}
