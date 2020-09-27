# prime.c
created by swathi
#include<stdio.h>
int primenumber(int,int);
void main()
{
  int num,check;
  printf("enter a number:");
  scanf("%d",&num);
  check=primenumber(num,num/2);
  if(check==1)
  {
  printf("%d is a prime number\n");
  }
  else
  {
  printf("%d is not a prime number\n");
  }
  getch();
}
int primenumber(int num,int i)
{
 if(i==1)
 {
 return 1;
 }
 else
 {
  if(num % i==0)
  {
  return 0;
  }
  else
  {
   return primenumber(num,i-1);
   }
  }
 }
