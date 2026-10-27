# Tutorial 03 - Answers

## Question 1
1. Write statements for each of the followingS

    a.Determine whether 3x8=27.

    ```java
        void main(){
            if(3 * 8 == 27)
                System.out.println("3 x 8 is equal to 27");
            else
                System.out.println("3 x 8 is not equal to 27");
        } 
    ```
    b.Determine whether an input integer is an odd number or even number.

    ```java
        import java.util.Scanner;
        void main(){
            Scanner input = new Scanner(System.in);
            System.out.print("Enter a number: ");
            int num = input.nextInt();

            if(num % 2 == 0)
                System.out.println(num + " is an even number");
            else
                System.out.println(num + " is an odd number");
        }
    ```

    c.Determine whether a character is a capital letter.

    ```java
        void main(){
            char character = 'a';

            if(Character.isUpperCase(character) == true)
                System.out.println(character + " is in capital letter");
            else
                System.out.println(character + " is not in capital letter");
        }
    ```

    d.Display two strings in alphabetical order ignoring their case.
    
    ```java
        void main(){
            String word1 = "Hello"
            String word2 = "World"

            if(word1.compareToIgnoreCase(word2) <= 0);
                System.out.println(word1);
                System.out.println(word2);
            else
                System.out.println(word2);
                System.out.println(word1);
        }
    ```

    e.A switch statement that display Sunday, Monday, .., Satudary if the input is 0,1, …, 6.

    ```java
        void main(){
            int day = 1;
            switch(day){
                case 0:
                    System.out.println("It is Sunday");
                    break;
                case 1:
                    System.out.println("It is Monday");
                    break;
                case 2:
                    System.out.println("It is Tuesday");
                    break;
                case 3:
                    System.out.println("It is Wednesday");
                    break;
                case 4:
                    System.out.println("It is Thursday");
                    break;
                case 5:
                    System.out.println("It is Friday");
                    break;
                case 6:
                    System.out.println("It is Saturday");
                    break;
            }
        }
    ```

## Question 2
2. Correct the error for the following statements.

    a.if (num1 = num2)<br>
        System.out.println("Number 1 is equal to number 2.");
    
    ```java
        if (num1 == num2)
        System.out.println("Number 1 is equal to number 2.");
    ```

    b.if (x > y > z)<br>
        System.out.println("x is the largest number");
    
    ```java
        if (x > y && x > z)
            System.out.println("x is the largest number");
    ```

    c.String s1, s2;<br>
      if (s1==s2)<br>
        System.out.println("They are equal strings.");<br>
      else (s1!=s2)<br>
        System.out.println("They are not equal strings.");
    
    ```java
        String s1, s2;
        if (s1.equals(s2))
            System.out.println("They are equal strings.");
        else
            System.out.println("They are not equal strings.");
    ```

    d.if x>0 or y>0;<br>
        System.out.println("Either x or y is positive");
    
    ```java
        if (x>0 || y>0)
            System.out.println("Either x or y is positive");
    ```

## Question 3
3. Write the output for the following statements when x=9 and y=10
    a.if (x < 10)<br>
        if (y > 10)<br>
            System.out.println("*****");<br>
      else<br>
        System.out.println("#####");<br>
        System.out.println("$$$$$");
    
    Output

        #####
        $$$$$
    
    b.if (x < 10) {<br>
        if (y < 10)<br>
            System.out.println("*****");<br>
      else{<br>
        System.out.println("#####");<br>
        System.out.println("$$$$$"); <br>
      }}
    
    Output

        #####
        $$$$$
    
    c.if (x < 10) {<br>
        if (y < 10)<br>
            System.out.println("*****");<br>
            System.out.println("#####");<br>
      }<br>
      else {<br>
        System.out.println("$$$$$");<br>
      }
    
    Output
    
        *****
        #####
    
    d.if (x > 10) {<br>
        if (y > 10) {<br>
            System.out.println("*****");<br>
            System.out.println("#####"); }<Br>
      else<br>
        System.out.println("$$$$$");<br>
      }
    
    Output

        no output
    
## Question 4
4. Write the java statements that used the if statement to find the biggest number among
three given integers.

    ```java
        void main(){
            int num1 = 20, num2 = 35, num3 = 43;
            int biggest;

            if (num1 > num2 && num1 >  num3)
                biggest = num1;
            else if (num2 > num1 && num2 >  num3)
                biggest = num2;
            else
                biggest = num3;
            System.out.println(biggest + " is the biggest number");
        }
    ```

## Question 5
5. Write the java statements that determine whether the Leap year. A Leap year is
divisible by 4 but not by 100. However, a Leap year is also divisible by 400.

    ```java
        void main(){
            int year = 2026;
            
            if (year % 4 == 0 && year % 100 != 0 || year % 400 == 0)
                System.out.println(year + " is a leap year.");
            else
                System.out.println(year + " is not a leap year.");
        }
    ```