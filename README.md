#include <stdio.h>
#include <math.h>
{
    float valor, novoValor;
    int i;

    printf("Escreva um valor x:");
    scanf("%f", &valor);
    
    for(i = 0; valor != 1; i++)
    {
        novoValor = valor/2;
        
        if(fmod(novoValor, 2) == 0)
        {
            valor = novoValor;
        }
        else
        {
            valor = ceil(novoValor);
        }
        printf("%.0f\n", valor);
    }
    
    printf("número de vezes até chegar no número desejado: %i\n", i);
    
    return 0;
}
