# Ex17 Reversing a String Using Stack Data Structure
## DATE:
## AIM:
To write a Java program that reverses an input string using a stack, without using built-in reverse functions.

## Algorithm
Start the program.

Read the input string from the user.

Create an empty stack of characters.

Traverse the string and push each character onto the stack.

Pop each character from the stack and append it to a new string — this gives the reversed string.

Display the reversed string.

Stop the program. 

## Program:
```
/*
Program to reverses an input string using a stack
Developed by:  Praveen K
RegisterNumber:  212223040152
*/

import java.util.Scanner;
import java.util.Stack;

public class ReverseStringWithStack {

    public static String reverseString(String input) {
         Stack<Character> stack=new Stack<>();
        for(char ch:input.toCharArray())
        {
            stack.push(ch);
        }
        StringBuilder rev=new StringBuilder();
        while(!stack.isEmpty())
        {
            rev.append(stack.pop());
        }
        return rev.toString();
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String input = scanner.nextLine();
        String reversed = reverseString(input);
        System.out.println(reversed);

        scanner.close();
    }
}
```

## Output:
<img width="467" height="339" alt="image" src="https://github.com/user-attachments/assets/aad99d95-fa31-41a7-bb1c-dc1c001dbea1" />



## Result:
Thus, the program successfully reverses the given string using a stack without relying on built-in reverse functions.
