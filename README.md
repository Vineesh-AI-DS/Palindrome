# Palindrome

## Aim:
To write a C# program to find whether the given string is a Palindrome or not.
## Algorithm:
### Step 1:
Create a new Class named palindrom.

### Step 2:
Declare three variables of string data type.

1.input - Store the input from user.
2.str - Convert user input to lower case and store it.
3.pal - Reverse the string str and store it.
### Step 3:
Get input from the user and store it. Then convert it to lower case.

### Step 4:
Using for loop, iterate through the each character from the end to begining and add it to the new variable called pal

### Step 5:
Using If-else statement check whether the input string & reversed string are same.

### Step 6:
Print the input and reversed string along with the whether palindrom or not.

### Step 7:
End of the Program.

## Program:
```
Developed By: Vineesh.M
Register Number: 212221230122
```
```cs
using System;
namespace Palindrome
{
    public class palindrome
    {
        public static void Main(string[] args)
        {
            string input, str, pal = "";
            Console.Write("Enter String: ");
            input = Console.ReadLine();
            str = input.ToLower();
            for (int i = str.Length - 1; i >= 0; i--)
            {
                pal += str[i];
            }
            if (str == pal)
            {
                Console.Write("{0} is a palindrome\n", input);
            }
            else
            {
                Console.Write("{0} is not a palindrome\n", input);
            }
        }
    }
}
```

## Output:
![npal](https://user-images.githubusercontent.com/93427254/226117533-0a8a90b6-73b9-4826-b1d5-45f9d462c0c3.png)

![pal](https://user-images.githubusercontent.com/93427254/226117534-4c10cb25-d27c-4a7a-a6f4-f948e59dfef6.png)



## Result:
Thus the C# program to display whether the given string is Palindrome or not is executed successfully.
