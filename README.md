#include <stdio.h>
#include <stdlib.h>

int main()
{
   int sayi,bas,top=0;
   printf("Sayi Girin: ");
   scanf("%d",&sayi);
   dnz:
   bas=sayi%10;
   top=top+bas^3;
   sayi=sayi/10;
       if(sayi<10)
        {top=top+sayi^3;
        goto dnz;}
       if(top==sayi)
        printf("Esittir");
       else
        printf("Esit degildir");

       getch();
}
