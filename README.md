/******************************************************************************

Utilizando o for, desenvolva um programa para verificar se um número fornecido 
pelo usuário é primo ou não. Um número primo é aquele que é divisível apenas 
por 1 e por ele mesmo.
*******************************************************************************/
           
            #include <stdio.h>
        
            int main(){
            
            int num, i = 1, primo = 0;
            
            printf("Verifique se um número é primo!\n");
            printf("Digite um número: ");
            scanf("%d", &num);
            
            while(num < 0){
                printf("Digite um número positivo: ");
                scanf("%d", &num);
            }
            
            for(i = 1;i <= num; i = i + 1){
                
                if(num % i == 0){
                    primo = primo + 1;
                }
                
            }
            
            if(primo <= 2){
                printf("%d É primo!", num);
            }
            else{
                printf("%d Não é primo!", num);
            }
        
            return 0;
        }
