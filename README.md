# DotNetAssignment1
```C#
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine("Enter the height of the triangle:");
    
        if (int.TryParse(Console.ReadLine(), out int height))
        {
            PrintTriangle(height);
        }
        else
        {
            Console.WriteLine("Invalid input. Please enter a valid integer.");
        }
    }

    static void PrintTriangle(int height)
    {
        for (int i = 1; i <= height; i++)
        {
            // Print spaces before the stars
            for (int j = 1; j <= height - i; j++)
            {
                Console.Write(" ");
            }

            // Print stars
            for (int k = 1; k <= 2 * i - 1; k++)
            {
                Console.Write("*");
            }

            Console.WriteLine(); // Move to the next line
        }
    }
}
```
![assignment_outputscreen1](https://github.com/chaithanya08-kashyap/DotNetAssignment1/assets/155832480/906beeef-28f4-4d21-94dc-aac3c93a7461)





