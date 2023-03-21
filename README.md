# Ex No.:2 Palindrome


## Aim:
To write a C# program to find whether the given string is a Palindrome or not.
## Algorithm:
### Step 1:
Create new class
### Step 2: 
Get the string from the user and convert all to lower case.
### Step 3:
Using for loop check whether the first and last letter are same and decrement it.
### Step 4:
Display that the string is palindrome when it clears the palindrome conditions. 

## Program:
Developed by: Shankar Saradha
<br/>
RegisterNumber:  212221240052
```c#
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Exp2
{
    internal class Program
    {
        static void Main(string[] args)
        {
            string array;
            Console.Write("Enter the String:");
            array = Console.ReadLine();
            int palindrome = 1;
            int len = array.Length;
            array=array.ToLower(); 
            for(int i=0,j=len-1;i<j;i++,j--)
            {
                if (array[i] != array[j])
                {
                    palindrome = 0;
                    break;
                }
            }
            if (palindrome == 1)
            {
                Console.WriteLine("The given string is Palindrome.");
            }
            else
            {
                Console.WriteLine("The given string is not Palindrome.");
            }
        }
    }
}
```


## Output:
![image](https://user-images.githubusercontent.com/93978702/226600291-3b21d58b-fd05-489d-88cf-d05d9235b5d8.png)
![image](https://user-images.githubusercontent.com/93978702/226600469-c4d12686-2412-4c70-9bc9-2519810b61f0.png)

## Result:
Thus the C# program to display whether the given string is Palindrome or not is executed successfully.
