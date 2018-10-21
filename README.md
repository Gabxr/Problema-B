#include <stdio.h>
#include <stdlib.h>

int main (){
	
	int n;
	printf("Quantas vezes os passos serao revezados? ");
	scanf("%i",&n);
	
	int cont =0;
	int i=0;
	int f[i];
	int x=0;
	int maior=0;
	
	for ( ; i<n+1; i++){
	printf("\nQuantidade de passos: ");
	scanf("\n%i",&f[i]);		
	cont++;
		
			if (i%2==0){
			       if (x==0){
			       	x=f[i];
			       }
			       else {
			x=x+f[i];	
			       }
			}
			else{
				x=x-f[i];
			}
			if (x>maior)
			maior=x;
	}
printf("\n------------------------------------------------");
printf("\nA maior distancia que Joaozinho andou foi de: %i",maior);
printf(" passos.");
	
return 0;
}
