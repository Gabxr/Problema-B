#include <stdio.h>
#include <stdlib.h> 

int main (){
	char resposta='s';
	
do {
	int n;
	printf("\nQuantas vezes os passos serao revezados? ");
	scanf("\n%i",&n);
	
	if (n==0){
	exit(0);
	}
	

	int i=0;
	int f[i];
	int x=0;
	int maior=0;
	

	for ( ; i<n+1; i++){
	printf("\nQuantidade de passos: ");
	scanf("\n%i",&f[i]);		
	
		
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
	
printf("\n\nDeseja testar outra vez?");
printf("\n(pressione 's' para continuar/qualquer digito para sair): ");
scanf("\n%c",&resposta);
if (resposta !='s'){
	exit (0);
}

} while (1);
	

return 0;
}
