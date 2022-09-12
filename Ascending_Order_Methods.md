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

#Sorting Method 2

```
using System;

public class HelloWorld
{
    public static void Main(string[] args)
    {
        int[] list = new int [10];
        int n, i, j, temp;
         
        Console.Write("Input size of the array.");
        n = Convert.ToInt32(Console.ReadLine());
         
        Console.Write("Write {0} number in the array \n", n);
        
        for(i=0;i<n;i++)
        {
            Console.Write("Number - {0}:",i);
            list[i] = Convert.ToInt32(Console.ReadLine());
        }
         
        for(i=0;i<n;i++)
        {
            for(j=i+1;j<n;j++)
            {
                if(list[j]<list[i])
                {
                    temp = list[i];
                    list[i] = list[j];
                    list[j] = temp;
                     
                }
            }
        }
         
        Console.WriteLine("Sorted list in ascending order.");
        for(i=0;i<n;i++)
        {
            Console.Write("{0} ", list[i]);
             
        }
        Console.Write("\n\n");	
    }
}
```
