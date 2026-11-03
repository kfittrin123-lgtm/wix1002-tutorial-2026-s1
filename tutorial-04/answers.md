# Tutorial 04 - answers

## Question 1
1. Write statements for each of the following

    a.Find the largest integer n so that n3 is less than 2000.

    ```java
        int n = 0;
        while(Math.pow(n,3)<2000){
            n++;
        }
        n--;
        System.out.println(n);
    ```

    b.Display the square number of the first twelve integers starting from 1.

    ```java
        for(int n = 1; n < 12 ; n++){
            System.out.print("Squared number of " + n + " : " + n*n);
        }
    ```

    c.Display a 4-by-5 matrix using random number within 0 to 100.

    ```java
        import java.util.Random;
        void main(){
            Random rand = new Random();
            for(int row = 0; row < 4; row++){
                for(int collumn = 0; collumn < 5; collumn++){
                    System.out.print(rand.nextInt(101) + " ");
                }
                System.out.println("");
            }
        }
    ```

    d.Compute the sum of numbers from 1 to a given number. 

    ```java
        import java.util.Scanner;
        void main(){
            Scanner input = new Scanner(System.in);
            System.out.print("Enter a number: ");
            int num = input.nextInt();
            int sum = 0;

            for(int n = 1; n <= num; n++){
                sum += n;
            }
            System.out.print("Sum of number 1 till " + num + " : " + sum);
        }
    ```

    e.Compute the sum of the series: 1/25+2/24+3/23 … + 25/1 in two decimal places.

    ```java
        double sum = 0;
        for(double i = 1,j = 25; i <= 25 && j>= 1; i++, j--){
            sum += i/j;
        }
        System.out.println("The sum is : " + sum)
    ```

## Question 2
2. Correct the error for the following statements

    a.for (x = 10; x > 0; x++)<br>
      sum += x;<br>

    ```java
        int sum = 0;
        for (int x = 10; x > 0;x--){
            sum += x;
        }
    ```

    b.do
        x += 2;<br>
        y += x;<br>
        System.out.println(x + " and " + y);<br>
      while (x < 100)<br>

    ```java
        int x = 0,y = 0;
        do{
            x += 2;
            y += x;
            System.out.println(x + " and " + y);
        }while(x<100);
    ```

    c.for ( x==1, y==20; x < y, x++, y-=2);<br>
        System.out.println(x & " " & y);<br>

    ```java
        for (int x = 1, y = 20; x < y; x++, y -= 2){
            System.out.println(x + " " + y);
        }
    ```

    d.i =1;<br>
      while(i<10) {<br>
        if (i==10)<br>
        System.out.println("Program End");<br>
      }<br>
    
    ```java
        int i = 1;
        while (i <= 10){
            if (i == 10){
                System.out.println("Program End");
                break;
            }
            i++;
        }
    ```

## Question 3
3. Write the statements that display the first ten values of the Fibonacci sequence. Given the formula f1 = 1, f2 =1, fn = fn-1 + fn-2.

    ```java
        int f1 = 1,f2 = 1, fn;
        System.out.print(f1 + " " + f2 + " ");
        for(int i = 3; i <= 10; i++){
            fn = f1 + f2;
            f1 = f2;
            f2 = fn;
            System.out.print(fn + " ");
        }

    ```

## Question 4
4. Write the statements that display the string in reverse order. (use String.length() to get the length of the string)

    ```java
        String sentence = "Sentence";
        String reversedSentence = "";
        for(int i = sentence.length() - 1; i >= 0; i--){
            reversedSentence += sentence.charAt(i);
        }
        System.out.println(reversedSentence);
    ```

