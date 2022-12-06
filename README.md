#include <stdio.h>
#include <stdlib.h>

int main()
{
   int number,digit,sum=0;
   printf("Enter a 3 digit number: ");
   scanf("%d",&number);
   dnz:
   digit=number%10;
   sum=sum+digit^3;
   number=number/10;
       if(number<10)
        {sum=sum+number^3;
        goto dnz;}
       if(sum==number)
        printf("Equal");
       else
        printf("Not equal");

       getch();
}
