using System;

namespace HelloWorld
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello World!");
        }
    }
}


Replace the contents of the Main method in Program.cs, which is the line that calls Console.WriteLine, with the following code:

C#


Console.WriteLine("What is your name?");
var name = Console.ReadLine();
var currentDate = DateTime.Now;
Console.WriteLine($"{Environment.NewLine}Hello, {name}, on {currentDate:d} at {currentDate:t}!");
Console.Write($"{Environment.NewLine}Press any key to exit...");
Console.ReadKey(true);

Run the program again:

.NET CLI


dotnet run
