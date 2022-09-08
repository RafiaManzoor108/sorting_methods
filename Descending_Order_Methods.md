# Descending Order

```
using System;

public class descending order
{
    public static void Main(string[] args)
    {
        int[] list = new int[] {5,2,7,1,0,4};
        int point;
        
        for(int i=0;i<list.Length-1;i++)
        {
            for(int j=i;j<list.Length;j++)
            {
                if(list[i] < list[j])
                {
                    point=list[i];
                    list[i]=list[j];
                    list[j]=point;
                }
            }
        }
        
        foreach (int digit in list)
        {
            Console.WriteLine (digit+" ");
        }
        
    }
}
```
