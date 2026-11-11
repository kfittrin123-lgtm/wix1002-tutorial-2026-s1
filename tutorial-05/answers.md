# Tutorial 05 - answers

## Question 1
1. Write statements for each of the following

    a.Declare an array that used to store 12 floating point numbers.

    ```java
        float[] numbers = new float[12];
    ```

    b.Initialize an array that used to store the value of A to E.

    ```java
        char[] letters = {'A','B','C','D','E'};
    ```

    c.Declare an array that used to store 100 students name.

    ```java
        String[] StudentName = new String[100];
    ```

    d.Declare an array for a table with 6 rows 2 columns that used to store integer value.

    ```java
        int[][] Integers = new int[6][2];
    ```

    e.Initialize an array with the following value:<br>
    (6,9)<br>
    (2,5)<br>
    (4,6)<br>

    ```java
        int[][] numbers = {
            {6,9},
            {2,5},
            {4,6}
        };
    ```

    f.After initialize the array, modify the value of the above array to:<br>
    (6,9)<br>
    (2,4)<br>
    (3,7)<br>

    ```java
        numbers[1][1] = 4;
        numbers[2][0] = 3;
        numbers[2][1] = 7;
    ```

    g.Display all the values of an array name contact in separate lines.

    ```java
        for(int i = 0; i < contact.length; i++){
            System.out.println(contact[i]);
        }
    ```

## Question 2
2. Correct the error for the following statements.

    a.String[] code = {'AAA', 'AAB', 'AAC', 'AAD'};

    ```java
        String[] code = {"AAA", "AAB", "AAC", "AAD"};
    ```

    b.int[] num = new num[10];<br>
    for(int k=0; k<=num.length(); k++)<br>
    sum+=num;<br>

    ```java
        int[num] = new int[10];
        int sum = 0;
        for(int k = 0; k<=num.length; k++){
            sum += num;
        }
    ```

    c.int [][]t = new int[3][];<br>
    t[1][2] = 5;<br>
    
    ```java
        int[][] t = new int[3][3];
        t[1][2] = 5;
    ```

    d.int i=4;<br>
    int []score = new int[5];<br>
    score [1] = 78;<br>
    score[++i] = 100;<br>

    ```java
        int i = 4;
        int[] score = new int[5];
        score[1] = 78;
        score[i] = 100;
    ```

## Question 3
3. Determine the values of each element of array marks. Assume the array was declared as:<br>
    
    int[] marks = new int[5];<br>
    int i = 0, j = 1;<br>
    marks[i] = 12;<br>
    marks[j] = marks[i] + 19;<br>
    marks[j-1] = marks[j] * marks [j];<br>
    marks[j*3] = marks[i+1];<br>
    marks[++j] = marks[i]%5;<br>
    marks[2*j] = marks[j-1];<br>

    Answers
    
        marks[0] = 961
        marks[1] = 31
        marks[2] = 1
        marks[3] = 31
        marks[4] = 31

## Question 4 
4. Write the statements that display the number of occurrence of the word "the" (case sensitive) in a string array name sentence. 

    ```java
        int count = 0;
        for(int i = 0; i<Sentence.length; i++){
            if (Sentence.equals("the")){
                count++;
            }
        }
    ```

## Question 5
5. Write the statements that display the string array name sentence in reverse order. Each string element must be displayed in reverse order as well.

    ```java
        for(int i = sentence.length - 1; i>=0; i--){
            for(int n = sentence[i].length - 1; n>=0; n--){
                System.out.print(sentence[i].charAt(n));
            }
            System.out.print(", ");
        }
    ```

## Question 6
6. Write the statements that generate 1 random integer within 0 – 255. Convert the number to binary and store the bit into an 8 bit array. Then, display the binary number.

    ```java
        Random rand = new Random();
        int RandNum = rand.nextInt(256);
        int temp = RandNum;
        int[] binary = new int[8];
        for(int i = 7; i>=0; i--){
            binary[i] = temp%2;
            temp /= 2;
        }

        for(int n = 0; n<binary.length; n++){
            System.out.print(binary[n]);
        }
    ```
