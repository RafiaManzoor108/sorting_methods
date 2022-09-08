# Sorting Methods

## Sorting Method 1

```
using System;


public class HelloWorld

{
    public static void Main(string[] args)
    {
        
        int[] list1 = {2,7,4,1,9,2};    
        Console.WriteLine("Unsorted array");       
        foreach (int i in list1)       
        {
            
            Console.Write(i + " ");
        
        }
               
        Array.Sort(list1);        
        Console.WriteLine("\nSorted list");      
        for (int i=0;i<list1.Length;i++)
        
        {
            
            Console.WriteLine(list1[i] + " ");
        
        }    
    }
}

```
