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

Q5 

#include <stdio.h>
 
int primeno(int, int);
 
int main()
{
    int num, check;
    printf("Enter a number: ");
    scanf("%d", &num);
    check=primenum(num,num/2)
    if (check == 1)
    {
        printf("%d is a prime number\n", num);
    }
    else
    {
        printf("%d is not a prime number\n", num);
    }
    return 0;
}
int primenum(int num, int i)
{
    if (i == 1)
    {
        return 1;
    }
    else
    {
  if (num % i == 0)
  {
  return 0;
 }
 else
 {
 return primenum(num, i - 1);
}
 }
}


Q6

#include <stdio.h>
int lcm(int, int);
int main()
{
    int a, b, result;
    int prime[100];
    printf("Enter two numbers: ");
    scanf("%d%d", &a, &b);
    result = lcm(a, b);
    printf("The LCM of %d and %d is %d\n", a, b, result);
    return 0;
}
int lcm(int a, int b)
{ 
 static int common = 1;
 if (common % a == 0 && common % b == 0)
 }
return common;
}
common++;
lcm(a, b);
return common;
}


Q7

#include <stdio.h>
#include <stdlib.h>
 
typedef struct{
 
    char name[10];
    int age;
    int salary;
    int phone number;
 
} Employee;
 
int main()
{
    int i, n=3;
 
    Employee employees[n];
    printf("Enter %d Employee Details \n \n",n);
    for(i=0; i<n; i++)
{
        printf("Name: ");
        scanf("%s",employees[i].name);
        printf("Age: ");
        scanf("%d",&employees[i].age);
        printf("Salary: ");
        scanf("%d",&employees[i].salary);
        printf("Phone number: ");
        scanf("%d",&employees[i].phone number);
 
        printf("\n");
    }
 
    printf("All Employees Details\n");
 
    for(i=0; i<n; i++)
{
 
        printf("Name \t: ");
        printf("%s \n",employees[i].name);
 
        printf("Age \t: ");
        printf("%d \n",employees[i].Age);
 
        printf("Salary \t: ");
        printf("%d \n",employees[i].Salary);
        
        printf("%d \t: ");
        printf("%d \n",employees[i].Phone number);
 
        printf("\n");
    }
 
    return 0;
}



Q8

print("Program for Student Information")
D = dict()
n = int(input('How many student record you want to store?? '))
for i in range(0,n):

    x, y = input("Enter the complete name (First and last name) of student: ").split()

    z = input("Enter contact number: ")

    m = input('Enter Marks: ')

    D[x, y] = (z, m)

def sort():

    ls = list()
    for sname,details in D.items(): 

        tup = (sname[0],sname[1]) 

        ls.append(tup)    

    ls = sorted(ls)    
    for i in ls:
   print(i[0],i[1]) 
    return
def minmarks():
   ls = list()
    for sname,details in D.items(): 

  ls.append(details[1])      
    ls = sorted(ls)    

    print("Minimum marks: ", min(ls))

    return

def searchdetail(fname):

    ls = list()

    for sname,details in D.items():

        tup=(sname,details)

        ls.append(tup)

    for i in ls: 

        if i[0][0] == fname:

 print(i[1][0])

    return

def option():
    choice = int(input('Enter the operation detail: \n \

    1: Sorting using first name \n \

    2: Finding Minimum marks \n \

    3: Search contact number using first name: \n \

    4: Exit\n \

    Option: '))

    if choice == 1:

        # function call

        sort()

        print('Want to perform some other operation??? Y or N: ')

        inp = input()

        if inp == 'Y':

            option()  

        # exit function call    

        exit()

    elif choice == 2:

        minmarks()

        print('Want to perform some other operation??? Y or N: ')

        inp = input()

        if inp == 'Y':
 option()

        exit() 

    elif choice == 3:

        first = input('Enter first name of student: ')

        searchdetail(first)

        print('Want to perform some other operation??? Y or N: ')

        inp = input()

        if inp == 'Y':

option()
 exit()
  else:

 print('Thanks for executing me!!!!')

 exit()

option()
