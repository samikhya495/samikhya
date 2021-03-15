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
