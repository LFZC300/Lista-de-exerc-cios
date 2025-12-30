# Lista-de-exerc-cios
Primeiro uso do Git


#include <stdio.h>
#define tam 5

int main()
{
	float mata[tam][tam], matb[tam][tam];
	int i, j;

	for(i=0; i<tam; i++) {
		for(j=0; j<tam; j++) {
			printf("Insira os valores da matriz A [%d] [%d]: ", i+1, j+1);
			scanf("%f", &mata[i][j]);

		}
	}

	for(i=0; i<tam; i++) {
		for(j=0; j<tam; j++) {
			matb[i][j] = mata[i][j] * 3;
		}

	}

	printf("\n--- Valores da matriz B (triplo da matriz A) ---\n");
	for(i=0; i<5; i++) {
		for(j=0; j<5; j++) {
			printf("%.1f\t", matb[i][j]);
		}
		printf("\n");
	}

	return 0;
}
