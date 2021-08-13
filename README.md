#include<stdio.h>
#include<string.h>

main(){
	char palabra[3]="escuela"; //declaramos variables
	char letras[3];
	char respuesta[3]={};
	char letra, opcion;
	char letra2="s";
	int i=0, intentos=3, contador=0;
	
	
	for( i=0; i<strlen(escuela); i++){
		letras[i]='_';
	}
    do {
    	fflush(stdin);
    	printf("\nInserta una letra: ");
    	scanf("%c",&letra);
    	
    	for( i=0; i<strlen(palabra); i++){
    		if(letra==palabra[i]){
    			letras[i]=letra;
			}
		}
		
		for(i=0; i<strlen(letras); i++){
			printf("%c", letras[i]);
			
		}
		printf("\n¿Ya sabes la respuesta?: s/n: ");
		scanf("%c",&opcion);
		contador++;
		
		if (opcion==letra2){
			printf("\nEscribe la respuesta aqui: ");
			scanf("%s",&respuesta[3]);
			palabra[3]=respuesta[3];
			
			printf("\nADIVINASTE");
		} break;
		
		
	
	} while(intentos==3);
      printf("\nLa palabra secreta es: escuela");
      printf("\n\n¡SUERTE PARA LA PROXIMA!");
