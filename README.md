# Recursive-function

## Aim: 
To write a C# program to reverse a number using recursive function.

## Algorithm:
### Step1:
Create a function for reversing.

### Step2:
Get the number from the user.

### Step3:
In the function find reminder of the number and multiply it by 10 and add the reverse number.

### Step4:
Recusively call this function to get the reversed number.

### Step5:

Print the reversed number.

## Program:
~~~
Name : Thirugnanamoorthi G
Reg no : 212221230117
~~~
~~~
using System;
namespace reverse
{
    class program
    {
        int rem, rev = 0;
        public int numRev(int num)
        {
            rem = num % 10;
            if (rem == 0)
            {
                return rev;
            }
            else
            {
                rem = num % 10;
                rev = rev * 10 + rem;
                return numRev(num / 10);

            }

        }
        static void Main(string[] args)
        {
            int n;
            Console.WriteLine("Enter a Number to reverse: ");
            n = Convert.ToInt32(Console.ReadLine());

            program p1 = new program();
            Console.WriteLine("Reversed Number is " + p1.numRev(n));
        }
    }
}

~~~


## Output:
![1](https://github.com/Thiru-AI/Recursive-function/assets/94980741/2a049468-9f51-46c8-8e91-6d175f0b8ccd)


## Result:
C# program to reverse a number using recursive function is executed successfully.

