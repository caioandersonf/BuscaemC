#include<stdio.h>
#include<stdlib.h>
#include<time.h>

#define tam 11
//buscar numeros pares
void gerarvalores(int v[tam]){
	for(int i=0; i<tam; i++){
		v[i] = rand() % 100;
	}
//	for(int cont=0; cont<tam; cont++){
//		printf("%d ", v[cont]);
//	}
}

void BubbleSort(int v[tam]){
	int i, j, aux;
	
	for(i=0; i<tam; i++){
		for(j=i + 1; j<tam; j++){
			
			if(v[j]<v[i]){
				aux = v[i];
				v[i] = v[j];
				v[j] = aux;
			}
		}
	}
	for(int i= 0; i<tam; i++){
		printf("%d ", v[i]);
	}
}

void buscaBinaria(int v[tam]){
	int meio = tam/2;
	int pivo = v[meio];
	int dado;
	
	printf("insira um numero: ");
	scanf("%d", &dado);
	
	for(int i = 0; i<tam; i++){
		if(pivo <= dado){
			for(int j = tam/2; j<tam; j++){
				if(v[j]==dado){
					printf("Seu dado existe no vetor\n");
					i = tam -1;
				}
			}
		}
		else if(pivo>=dado){
				if(v[tam/2]>dado){
					for(int j=0; j<tam/2; j++){
						if(v[j]==dado){
							printf("O dado existe no vetor\n");
				   	   	}
			   	   	}
	   	   	   	}
	   	   	   	i=tam-1;
		}
	
	}
}

void buscaLinear(int v[tam]){
	int contador = 0;
	
	for(int i = 0; i<tam; i++){
		if(v[i] % 2 == 0){
			contador++;
		}
	}
	printf("\n\nSeu vetor possui %d numeros pares\n", contador);
}
int main(){
	int vetor[tam];
	
	gerarvalores(vetor);
	BubbleSort(vetor);
	buscaBinaria(vetor);
}
