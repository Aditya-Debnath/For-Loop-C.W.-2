# For-Loop-C.W.-2
17.08.2022 Lab Class Works

1st Problem 

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



5th Problem 

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
    printf("\nTotal prime number are=%d",count);
    
    return 0;
    
}

6th Problem

Solution

#include<stdio.h>
int main()
{

    int n, i, j, k;
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
    for(k=0;k<=n;k++)
    {
        printf("$");
    }
    printf("\n");
    
}












