# For-Loop-C.W.-2
17.08.2022 Lab Class Works

1st Problem 

Input :- 3
Output :-
***\n
***\n
***\n

\n is for new line, it will not show in output.

Solution :-

#include<stdio.h>
int main()
{

    int i, n, j, k;
    scanf("%d",&n);
    for(i=1;i<=n;i++)
    {
        {
            for(j=1;j<=n;j++)
            {
                printf("*");
            }
            printf("\n");
         }
    }
    
}

2ed Problem 

Input :- 3
Output :-
***\n
* *\n
***\

\n is for new line, it will not show in output.

Solution :-

#include<stdio.h>
int main()
{

    int i, j, k, m, n;

    scanf("%d",&n);
    for(k=1;k<=n;k++)
    {
        printf("*");
    }
    printf("\n");

    for(i=1;i<=n-2;i++)
    {
        printf("*");
        for(j=0;j<n-2;j++)
        {
            printf(" ");
        }
        printf("*");
        printf("\n");
    }
    for(m=1;m<=n;m++)
    {
        printf("*");
    }
    
}

3rd Problem

Input :- 5
Output :- 12321

Solution :-

#include<stdio.h>
int main()
{

    int i, j,n;
    scanf("%d",&n);
    for(i=1;i<=n/2;i++)
    {
        printf("%d",i);
    }
    printf("%d",n/2+1);
    for(j=n/2;j>=1;j--)
    {
        printf("%d",j);
    }
    
}

Another solution from sir.

#include<stdio.h>
int main()
{

    int i, j, n;
    scanf("%d",&n);
    j=1;
    int flag = 1;
    for(i=0;i<n;i++)
    {
        printf("%d",j);
        if(j<= n/2 && flag == 1)
        {
            j++;
        }
        else
        {
            j--;
            flag =0;
        }
    }
    
}


4th Problem

Input :- 5
Output :-
12321
12321
12321
12321
12321

Solution

#include<stdio.h>
int main()
{

    int n, i, j, k;
    scanf("%d",&n);
    for(int k =0;k<n;k++)
    {
         j=1;
         int flag = 1;
         for(i=0;i<n;i++)
        {
             printf("%d",j);
            if(j<= n/2 && flag == 1)
            {
            j++;
            }
            else
            {
              j--;
              flag =0;
            }
        }
        printf("\n");
    }
    
}

Solution from sir

#include<stdio.h>
int main()
{

    int n, i, j;
    scanf("%d",&n);
    for(int k = 0; k<n ;k++)
    {
        j = 1;
        int flag = 1;
        for(i = 0; i< n;i++)
        {
            printf("%d",j);
            if(j<= n/2 && flag == 1) j++;
            else{
                    j--;
                    flag = 0;
            }
        }
        printf("\n");
    }
    
}

5th Problem
Input :- 5
Output :-
1
12
123
1234
12345

Solution

#include<stdio.h>
int main()
{

    int n, i, j;
    scanf("%d",&n);
    {
    for(i=1;i<=n;i++)
    {
        for(j=1;j<=i;j++)
        {
            printf("%d",j);
        }
        printf("\n");
    }
    }
    
}


6th Problem 

Finding Prime numbers between 10 to 50.

Solution 

#include<stdio.h>
int main()
{

    int n,m,i,j;
    int count=0;
    scanf("%d %d",&m,&n);
    for(i=m;i<=n;i++)
    {
        int prime=0;
        for(j=2;j<i;j++)
        {
            if(i%j==0)
            {
                prime = 1;
                break;
            }
        }
        if(prime!=1)
        {
            count++;
            printf("%d\n",i);
        }
    }
    printf("\nTotal prime number are = %d",count);
    
    return 0;
    
}

7th Problem

Try to solve full Picture.

Solution

#include<stdio.h>
int main()
{

    //C.W.
    int n, i, j, k, m, x;
    scanf("%d",&n);
    for(i=1;i<=n/2;i++)
    {
        for(j=1;j<=n;j++)
        {
            if(j==n/2+1 || j== n/2+1-i+1 || j==n/2+1+i-1){

                printf("$");
            }else
                printf("-");
        }
        printf("\n");
    }
    for(k=0;k<=n-1;k++)
    {
        printf("$");
    }
    printf("\n");
    //C.W. ENDED.
    
    //H.W.
    for(m=n/2;m>=1;m--)
    {
        for(x=n;x>=1;x--)
            {
                if(x==n/2+1 || x==n/2+1-m+1 || x==n/2+1+m-1)
                {
                    printf("$");
                }
                else
                {
                    printf("-");
                }
            }
            printf("\n");
    }
    //H.W. ended. If you don't understand the process, you can ask me any time. :D
}


