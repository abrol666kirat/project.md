**PARKIRAT SINGH**

#**COMPUTER SCIENCE**

#***PPS COURSE***18105

#*1915057*

```c
#include <stdio.h>
int main()
{
        int m, n, c, d, first[10][10], second[10][10], sum[10][10];
        printf("Enter the number of rows and columns of matrix\n");
        scanf("%d%d", &m, &n);
        printf("Enter the elements of first matrix\n");
        for (c = 0; c < m; c++)
        for (d = 0; d < n; d++)
             scanf("%d", &first[c][d]);

        printf("Enter the elements of second matrix\n");

        for (c = 0; c < m; c++)
                for (d = 0 ; d < n; d++)
                        scanf("%d", &second[c][d]);
        printf("Sum of entered matrices:-\n");

        for (c = 0; c < m; c++)
        {
                for (d = 0 ; d < n; d++) 
                {
                        sum[c][d] = first[c][d] + second[c][d];
                        printf("%d\t", sum[c][d]);
                }
                printf("\n");
        }
       return 0;
}
```
```c
#include <stdio.h>
int main()
{
  int array[100], n, c, d, swap;
  printf("Enter number of elements\n");
  scanf("%d", &n);
  printf("Enter %d integers\n", n);
  for (c = 0; c < n; c++)
    scanf("%d", &array[c]);
  for (c = 0 ; c < n - 1; c++)
  {
    for (d = 0 ; d < n - c - 1; d++)
    {
      if (array[d] > array[d+1])
      {
        swap       = array[d];
        array[d]   = array[d+1];
        array[d+1] = swap;
      }
    }
  }
  printf("Sorted list in ascending order:\n");
  for (c = 0; c < n; c++)
     printf("%d\n", array[c]);
  return 0;
}
```
```c
#include <stdio.h>
void swap(int*, int*);
int main()
{
   int x, y;
   printf("Enter the value of x and y\n");
   scanf("%d%d",&x,&y);
   printf("Before Swapping\nx = %d\ny = %d\n", x, y);
   swap(&x, &y);
   printf("After Swapping\nx = %d\ny = %d\n", x, y);
   return 0;
}
void swap(int *a, int *b)
{
   int temp;
   temp = *b;
   *b = *a;
   *a = temp;
}
```
```c
#include<stdio.h>

void swap(int,int);        

void main( )
{
    int n1,n2;
    printf("Enter the two numbers to be swapped\n");
    scanf("%d%d",&n1,&n2);
    printf("\nThe values of n1 and n2 in the main function before calling the swap function are n1=%d n2=%d\n",n1,n2);
    swap(n1,n2);
    printf("\nThe values of n1 and n2 in the main function after calling the swap function are n1=%d n2=%d\n",n1,n2);}

void swap(int n1,int n2)
{ 
    int temp;
    temp=n1;
    n1=n2;
    n2=temp;
    printf("\nThe values of n1 and n2 in the swap function after swapping are n1=%d n2=%d\n",n1,n2);
}
```
```c
#include<stdio.h>

int main()
{
puts("Parkirat\n CSE A2\n 1915057\n\
Doraha, Distt, Ludhiana");
return 0;
}
```
```c
#include <stdio.h>
int main()
{
        int num;
        printf("Enter an integer number: ");
        scanf("%d",&num);
        if(num%2==0)
                printf("%d is an EVEN number.\n",num);
        else
                printf("%d is an ODD number.\n",num);
        return 0;
}
```
```c
#include <stdio.h>
int main()
{
    int i, n, t1 = 0, t2 = 1, nextTerm;
    printf("Enter the number of terms: ");
    scanf("%d", &n);
    printf("Fibonacci Series: ");
    for (i = 1; i <= n; ++i)
    {
        printf("%d, ", t1);
        nextTerm = t1 + t2;
        t1 = t2;
        t2 = nextTerm;
    }
    return 0;
}
```
```c
#include<stdio.h>

int main()
{
int n,a=0,b=1,c,i;
printf(" Enter the  no of fibonachi terms u want to print: ");
scanf("%d",&n);
printf("%d\t%d\t",a,b);
for(i=1;i<=n-2;i++)
{
c=a+b;
printf("%d\t",c);
a=b;
b=c;
}
return 0;
}
```
```c
#include <stdio.h>
int main()
{
    int n, i;
    int factorial = 1;
    printf("Enter an integer: ");
    scanf("%d",&n);
    if (n < 0)
        printf("Error! Factorial of a negative number doesn't exist.");
    else
    {
        for(i=1; i<=n; ++i)
        {
            factorial *= i;
        }
        printf("Factorial of %d = %d\n", n, factorial);
    }
    return 0;
}
```
```c

#include <stdio.h>
int multiplyNumbers(int n);
int main()
{
    int n;
    printf("Enter a positive integer: ");
    scanf("%d", &n);
    printf("Factorial of %d = %d\n", n, multiplyNumbers(n));
    return 0;
}
int multiplyNumbers(int n)
{
    if (n >= 1)
        return n*multiplyNumbers(n-1);
    else
        return 1;
}
```
```c
#include<stdio.h>
float square ( float x );
int main()
{   
    float m, n ;
    printf ( "\nEnter some number for finding square \n");
    scanf ( "%f", &m ) ;
    // function call
    n = square ( m ) ;
    printf ( "\nSquare of the given number %f is %f\n",m,n );
}

float square ( float x )
{
    float p ;
    p = x * x ;
    return ( p ) ;
}
```
```c
#include<stdio.h>

int main()
{
	int a,b,c;

	printf("Enter the three numbers : ");
	scanf("%d %d %d",&a,&b,&c);

{
	if(a>b&&a>c)
	printf("%d is the greatest\n",a);


	if(b>a&&b>c)
	printf("%d isthe greatest\n",b);


	if(c>a&&c>b)
	printf("%d is the greatest\n",c);
}
	return 0;
}
```
```c
#include <stdio.h>
int main()
{
    int i, space, rows, k=0;
    printf("Enter number of rows: ");
    scanf("%d",&rows);
    for(i=1; i<=rows; ++i, k=0)
    {
        for(space=1; space<=rows-i; ++space)
        {
            printf("  ");
        }
        while(k != 2*i-1)
        {
            printf("* ");
            ++k;
        }
        printf("\n");
    }
    return 0;
}
```
```c
#include<stdio.h>

int main()
{
int n; 
printf("Enter the year u want to check it for leap :");
scanf("%d",&n);
if(n%4==0)
printf("it is a leap year\n");
else
printf(" not a leap year\n");
return 0;
}
```
```c
#include<stdio.h>
int  main()
{
int i;
 int a[i],max;

 for(i=0;i<=4;i++)

  {
    scanf("%d",&a[i]);
    max = a[0];


    for(i=1;i<=4;i++)
    {
      if( max<a[i])
     max =a[i];
}
}
  printf("max of the array %d",max);
return 0;
} 
```
```c
#include<stdio.h>  
int main()    
{    
    int n,r,sum=0,temp;    
    printf("enter the number=");    
    scanf("%d",&n);    
    temp=n;    
    while(n>0)    
    {    
        r=n%10;    
        sum=(sum*10)+r;    
        n=n/10;    
    }    
    if(temp==sum)    
        printf("palindrome number \n");    
    else    
        printf("not palindrome\n");   
    return 0;  
}   
```
```c
#include <stdio.h>
    int main()
    {
        int i, j, rows;
        printf("Enter number of rows: ");
        scanf("%d",&rows);
        for(i=1;i<=rows;i++)
        {
            for(j=1;j<=i;j++)
            {
                printf("* ");
            }
            printf("\n");
        }
        return 0;

    }
    ```
    ```c
    # include<stdio.h>
int main()
{
int i,j,n,k,l;
printf("Enter the no of rows of pattern u want to print : ");
scanf("%d",&n);
for(i=1;i<=n;i++)
{for(j=1;j<=i;j++)
printf("*");
printf("\n");
}
for(k=1;k<=n;k++)
{for(l=1;l<=n-k;l++)
printf("*");
printf("\n");
}
return 0;
}
```
```c
#include<stdio.h>

int main()
{
int i,j,k,n;
printf("Enter the no of rows of pattern u want to print: ");
scanf("%d",&n);
for(i=1;i<=n;i++)
{
for(j=1;j<=n-i;j++)
printf(" ");
for(k=1;k<=i;k++)
printf("*");
printf("\n");
}
return 0;
}
```
```c
#include<stdio.h>

int main()
{
int i,j,k,n;
printf("Enter the no of rows of pattern u want to see : ");
scanf("%d",&n);
for(i=1;i<=n;i++)
{
for(j=1;j<=n-i;j++)
printf(" ");
for(k=1;k<=2*i-1;k++)
printf("*");
printf("\n");
}
return 0;
} 
```
```c
#include<stdio.h>
int main()
{   
        int n;
        int *p;
        p=&n;
        n=100;
        printf("using variable :- \n");
        printf("value of n:%d\n adress of n:%d\n",n,&n);
        printf("using pointer variable :- \n");
        printf("value of n:%d \n adress of n:%d\n",*p,p);
        return 0;
}
```
```c
#include<stdio.h>
#include<math.h>
int main()
{
 float a,b,c,d,r1,r2;
printf("\n programe to find roots ");
printf("\n enter the value of a,b,c where a*x*x+b*c+c=0");
scanf("\n%.4f,%.4f,%.4f",&a,&b,&c);
            
           d=(b*b)-(4*a*c);
    if (d==0)
{
    printf("\nthe roots are real");	
}	 

else	if(d<0)
{
	printf("\nthe roots are imagimnary");
}

else	if (d>0)
{
	printf("\nthe roots are  real and unequal");
} 
   return 0;
}
```
```c
#include<stdio.h>
int factorial(int);
int main()
{
        int i;
        printf("Enter any value :- ");
        scanf("%d",&i);
        printf("Factorial is :- %d ",factorial(i));
        return 0;
}
int factorial(int i)
{
        if(i==1)
                return 1;
        return i*factorial(i-1);
}
```
```c
#include<stdio.h>
int main()
{       
        int a,n,r;
        printf("Enter a value to find its reverse :- \n");
        scanf("%d",&n);
        while(n>=1)
        {
                a=n%10;
                r=r*10+a;
                n=n/10;
        }
        printf("the reversed value is :- %d\n",r);
        return 0;
}
```
```c
#include<stdio.h>

int main()
{
int n;
printf(" Enter m for monday t for tuesday w for wednesday h for thursday f for friday s for saturday  : ");
scanf("%c",&n);
switch(n)
{
case 'm':printf("monday\n");
break;
case 't':printf("tuesday\n");
break;
case 'w':printf("wednseday\n");
break;
case 'h':printf("thursday\n");
break;
case 'f':printf("friday\n");
break;
case 's':printf("saturday\n");
break;
}
return 0;
}
```
```c
  #include <stdio.h>
    int main()
    {
        int a[10][10], transpose[10][10], r, c, i, j;
        printf("Enter rows and columns of matrix: ");
        scanf("%d %d", &r, &c);
        // Storing elements of the matrix
        printf("\nEnter elements of matrix:\n");
        for(i=0; i<r; ++i)
            for(j=0; j<c; ++j)
            {   
                printf("Enter element a%d%d: ",i+1, j+1);
                scanf("%d", &a[i][j]);
            }
        // Displaying the matrix a[][] */
        printf("\nEntered Matrix: \n");
        for(i=0; i<r; ++i)
            for(j=0; j<c; ++j)
            {   
                printf("%d  ", a[i][j]);
                if (j == c-1)
                    printf("\n\n");
            }
        // Finding the transpose of matrix a
        for(i=0; i<r; ++i)
            for(j=0; j<c; ++j)
            {
                transpose[j][i] = a[i][j];
            }
        // Displaying the transpose of matrix a
        printf("\nTranspose of Matrix:\n");
        for(i=0; i<c; ++i)
            for(j=0; j<r; ++j)
            {
                printf("%d  ",transpose[i][j]);
                if(j==r-1)
                     printf("\n\n");
            }
        return 0;
    }
```
```c
#include<stdio.h>

int main()
{ 
float f,c;
printf(" Enter degree of farenhiet:  ");

scanf("%f",&f);
c=(f-32)*5/9;
printf("The coverted value of  %f farenhiet is : %f\n",f,c);
return 0;
}
```
```c
#include<stdio.h>
int main()
{
   printf("hello budding engineers");
 
   return 0;
}
```
