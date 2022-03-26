	#include<stdio.h>
	
	int find_lcm(int, int,int);   // function prototype declaration
	
	int main()
	{
	    int a, b, lcm, max;
	    printf("\nEnter 2 numbers to find LCM of:");
	    scanf("%d%d", &a, &b);
	    max = (a > b) ? a : b;
	    lcm = find_lcm(a,b,max);    // function call
	    return 0;
	}
	
	int find_lcm(int a, int b,int max)  // function definition
	{
	    
	   while (1) 
	    {
	        if (max % a == 0 && max % b == 0) 
			{
	            printf("The LCM of %d and %d is %d.", a, b, max);
	            break;
	        }
	        ++max;
	    }
	    return 0;
	}
