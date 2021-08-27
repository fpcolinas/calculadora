#include <stdio.h>
#include <stdlib.h>
#define j 3
void menu()
{
system("cls");
system("color 0b");

 printf("\n>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>\n\n");
printf(" \n\n\t\t CALCULADORA\n\n");
printf(" \n1 - SOMAR\n");
printf(" \n2 - SUBTRAIR\n");
printf(" \n3 - MULTIPLICAR\n");
printf(" \n4 - DIVIDIR\n");
printf(">>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>\n\n\n\n\n");

}

void calcula(int opc,float n1,float n2)
{
float resultado;

 if (opc==1)
{
resultado=n1+n2;
}
if (opc==2)
{
resultado=n1-n2;
}
if (opc==3)
{
resultado=n1*n2;
}
if (opc==4)
{
resultado=n1/n2;
}
 system("pause");
 system("cls");
 system("color 0f");
printf("============================================================\n\n");
printf(" \n\n\t\t RESULTADO >>>> %.2f\n",resultado);
printf("============================================================\n\n");

 getch();

}

int main()
{
float v1,v2,resposta;
int op,i;

 for (i=0;i<j;i++)
{
menu();

 printf("\n Informe o numero da opcao desejada>>> ");
scanf("%d",&op);

 printf("\n Informe o primeiro valor>>> ");
scanf("%f",&v1);

 printf("\n Informe o segundo valor>>> ");
scanf("%f",&v2);

 calcula(op,v1,v2);

 }
return 0;
}
