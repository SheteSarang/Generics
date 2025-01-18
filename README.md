# Generics
using System;
 
namespace Generics
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int[] a = new int[] { 1, 2, 3 };
            string[] b = new string[] { "q", "s", "d" };
 
            // Call the generic method for both int and string arrays
            PrintArray<int>(a);
            PrintArray<string>(b);
 
            Console.ReadLine(); // To keep the console open
        }
 
        
        public static void PrintArray<T>(T[] values)
        {
            foreach (var i in values)
            {
                Console.Write(i);
            }
        }
    }
}
