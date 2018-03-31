package train3;

public class Max 
{
   public static int maxsum(int[] a)
   {  
	int firstsum;
	int secondsum = 0;
	int i,j,k;
   for( i=0;i<a.length;i++)
   {
     for( j=i ; j < a.length;j++)
      {  
        firstsum=0;  
        for ( k=i; k <= j; k++)
           {  
             firstsum=firstsum+ a[k];  
             if(firstsum > secondsum)
             {  
               secondsum = firstsum;  
             }  
           }  
      } 
   }
         if (secondsum < 0) 
         {
             return 0;
         }
         else 
         {
             return secondsum;
         }
   }
}

