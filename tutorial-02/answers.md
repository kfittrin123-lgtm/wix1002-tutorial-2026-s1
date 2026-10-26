# Tutorial 02 - Answers

## Question 1
1. Display the sentence Faculty of Computer Science and Information Technology.

    a. In one line using multiple Java statements

    ```java
    void main(){
       IO.print("Faculty ");
       IO.print("of ");
       IO.print("Computer ");
       IO.print("Science ");
       IO.print("and ");
       IO.print("Information ");
       IO.print("Technology");
    }
    ```

    b. In multiple lines using one Java statement

    ```java
    void main(){
       IO.print("Faculty \nof \nComputer \nScience \nand \nInformation \nTechnology");
    }
    ```

## Question 2
2. Write a Java statement that print "SDN" - Software-defined networking

    ```java
    void main(){
        IO.print("\"SDN\" - Software-defined networking");
    }
    ```

## Question 3
3. Correct the error for the following statements.

    a. System.Println("Java Programming");

    ```java
    void main(){
        System.out.println("Java Programming");
    }
    ```
    b. System.in.println("Introduction to Java!")

    ```java
    void main(){
        System.out.println("Introduction to Java!");
    }
    ```

    c. System.out.println("\t is the horizontal tab character");

    ```java
    void main(){
        System.out.println("\\t is the horizontal tab character");
    }
    ```

    d. system.out.println("Java is case sensitive!" );

    ```java
    void main(){
        System.out.println("Java is case sensitive!");
    }
    ```

## Question 4
4. Write statements for each of the following

    a. Declare a variable that used to store the value of a matric number.

    ```java
    void main(){
        String MatricNumber;
    }
    ```

    b. Declare a variable that used to store the value of π.

    ```java
    void main(){
        double PI = Math.PI;
    }
    ```

    c. Initialize a variable named M with the value set to false.

    ```java
    void main(){
        boolean M = false;
    }
    ```

    d. Initialize a variable named P with the value set to 8800000000.

    ```java
    void main(){
        long P = 8800000000L;
    }
    ```

    e. Initialize a variable named letter with the value set to U.

    ```java
    void main(){
        char letter = 'U';
    }
    ```

    f. Declare a constant variable named PRO. The value of the constant variable is
Java. 

    ```java
    void main(){
        final String PRO = "Java";
    }
    ```

## Question 5
5. Correct the error for the following statements.
    a.
        final double AMOUNT = "32.5";<br>
        AMOUNT += 10;<br>
        System.out.println("The amount is " + AMOUNT);
    
    ```java
    void main(){
        double AMOUNT = 32.5;
        AMOUNT += 10;
        System.out.println("The amount is " + AMOUNT);
    }
    ```

    b.
    string chapter = 'Summary';<br>
    System.out.println(chapter)

    ```java
    void main(){
        String chapter = "Summary";
        System.out.println(chapter);
    }
    ```

    c.
    int num;<br>
    ++num++;<br>
    num1 = num

    ```java
    void main(){
        int num = 0;
        num++;
        int num1 = num;
    }
    ```

    d.
    int num = 3000;<br>
    System.out.printf("%4.2f\n", num);

    ```java
    void main(){
        int num = 3000;
        System.out.printf("%d",num);
    }
    ```

    e.
    String contact;<br>
    Scanner keyboard = new Scanner(System.out);<br>
    contact = keyboard.nextLine();

    ```java
    void main(){
        String contact;
        Scanner keyboard = new Scanner(System.in);
        contact = keyboard.nextLine();
    }
    ```

## Question 6
6. Write a java program that print the circumference of a circle. The input of the
program is diameter. Display the result in three decimal places. (Note pi = Math.PI)<br>
    Enter Diameter: 11.8<br>
    The circumference of the circle is : 37.071

    ```java
    void main(){
        Scanner input = new Scanner(System.in);
        System.out.print("Enter Diameter: ");
        double diameter = input.nextDouble();
        double pi = Math.pi;
        double circumference = 2 * diameter * pi;
        System.out.printf("\n%.3f",circumference)
    }
    ```

## Question 7
7. Write a java program that converts inches to meters. (Given 1 inch equals to 2.54
centimeters). Print the output in two decimal places.<br>
    Enter value in inch: 20.17<br>
    20.17 inches in meters: 0.51 meters

    ```java
    void main(){
        Scanner input = new Scanner(System.in);
        System.out.print("Enter value in inch: ");
        double inches = input.nextDouble();
        double meters = (inches * 2.54)/100;
        System.out.printf("\n %.2f inches in meters: %.2f meters",inches,meters);
    }
    ```