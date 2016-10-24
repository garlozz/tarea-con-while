# include <stdio.h>
# include <stdlib.h>
int main ()
{
    float temperatura, promedio, sumatemperatura=0;
    int numero=0;
    printf ("\n Programa temperatura de procesadores\n");
    printf ("\n Ingrese temperatura \n\t");
    scanf ("%f", &temperatura);
    while (temperatura !=0)
    {
        if (temperatura ==0)
        {
            printf ("\n Ingrese temperatura del procesador (acabar programa con 0) \n\t");
        }
        else
        {
            numero++;
            sumatemperatura+=temperatura;
        }
      printf("\ningrese otra temperatura (finalizar con 0)\n");
      scanf("%f", & temperatura);
    }
    promedio=(float)sumatemperatura/numero;

    printf ("\n\t La suma de temperaturas es: %.2f", sumatemperatura);
    printf ("\n\t EL promedio de temperaturas es : %.2f", promedio);
    getch();
    return 0;
}
