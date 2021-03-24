Q1

#include<stdio.h>  
 int main()    
{    
int a=8 b=5;      
printf("Before swap a=%d b=%d",a,b);      
a=a+b;  // value is 13 
b=a-b; //value is 8
a=a-b; //value is 5
printf("After swap a=%d b=%d",a,b);    
return 0;  
}   
 

Q2

#include<stdio.h>
int main()
{
int num,a;
printf("Enter the number",a);
Scanf("%d",&a);
switch(num)
{
case1:
if(a==0)
printf("you entered the correct value");
case2:
if(a==1)
printf ("your entry is correct");
default:
printf("invalid entry");
break;
}
}



Q3


include <stdio.h>
int main() 
{
  int Rows, i, j;	
  printf("Please Enter the Number of Rows:  ");
  scanf("%d", &Rows);	
  printf("\nPrinting Right Angled Triangle \n \n");
  for ( i = 1 ; i <= Rows; i++ ) 
  {
 for ( j = 1 ; j <= i; j++ ) 
  {
  printf("01 ");
 }
 printf("\n");
}
return 0;
}
 
Q4

#include <stdio.h>
 
int sum (int a);
 
int main()
{
    int num, result;
 
    printf("Enter the number: ");
    scanf("%d", &num);
    result = sum(num);
    printf("Sum of digits in %d is %d\n", num, result);
    return 0;
}
 
int sum (int num)
{
    if (num != 0)
    {
        return (num % 10 + sum (num / 10));
    }
    else
    {
       return 0;
    }
}
