# alimento-e-bebida
Fastfood

#include<stdio.h>
float acum=0,valor,vf;
int cod,qtd,qde;
char resp;

int main(){
	printf("**********welcome fast food fmu*********");
	do{
	printf("\n o que voce deseja? ");
	printf("\ncachorro quente - cod 100");
	printf("\nrefrigerante - cod 101\n");
	scanf("%d",&cod);
	printf("\nqual a quantidade desejada: ");
	scanf("%d",&qde);
	if(cod==100){
		printf("\ncachorro quente");
		valor=qde*10.00;
	}
	else if(cod==101){
		printf("\nrefrigerante");
		valor=qde*5.00;
	}
	acum+=valor;
	printf("\no valor atual e RS%.2f",valor);
	printf("\ndeseja mais algum produto? S-sim N-nao ");
	scanf(" %c",&resp);
	}
	
while(resp=='s'||resp=='S');
printf("\nTotal a pagar RS%.2f",acum);
	
return 0;
}
