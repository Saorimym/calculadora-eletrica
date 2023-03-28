# calculadora-eletrica
 #include <stdio.h>
#include <math.h>

int main() {
    int opcao;
    float v, i, p,corrente,resistencia, tensao;

    printf("Escolha a opcao desejada:\n");
    printf("1 - Conversao de potencia e corrente para tensao\n");
    printf("1 - Conversao de potencia e corrente para resistencia\n");
    printf("====================================================\n");
    printf("3 - Conversao de tensao e potencia para corrente\n");
    printf("4 - Conversao de tensao e potencia para resistencia\n");
    printf("====================================================\n");
    printf("5 - Conversao de corrente e resistencia para tensao\n");
    printf("6 - Conversao de corrente e resistencia para tensao\n");
    printf("====================================================\n");
    printf("7 - Conversao de corrente e tensao para potencia\n");
    printf("8 - Conversao de corrente e tensao para resistencia\n");
    printf("====================================================\n");
    printf("9 - Conversao de resistencia e tensao para corrente\n");
    printf("10 - Conversao de resistencia e tensao para potencia\n");

    scanf("%d", &opcao);

    switch (opcao) {
        case 1:
            printf("Digite a potencia em watts: ");
            scanf("%f", &p);

            printf("Digite a corrente em amperes: ");
            scanf("%f", &i);

            v = p / i;

            printf("A tensao em volts eh: %.2f V\n", v);
            break;

        case 2:
            printf("Digite a potencia em watts: ");
            scanf("%f", &p);

            printf("Digite a corrente em amperes: ");
            scanf("%f", &i);

            r = (p / i) / i;

            printf("A tensao em volts eh: %.2f V\n", r);
            break;
          
        case 3:
            printf("Digite a tensao em volts: ");
            scanf("%f", &v);

            printf("Digite a potencia em watts: ");
            scanf("%f", &p);

            i = p / v;

            printf("A corrente em amperes eh: %.2f A\n", i);
            break;
            
       case 4:
           printf("Digite a tensao em volts: ");
           scanf("%f", &v);

           printf("Digite a potencia em watts: ");
           scanf("%f", &p);

           r = v² / p;

           printf("A corrente em amperes eh: %.2f A\n", r);
           break;
           
        case 5:
            printf("Digite a corrente em amperes: ");
			scanf("%f", &corrente);
			   
			printf("Digite a resistencia em ohms: ");
			   scanf("%f", &resistencia);
			  
			tensao = corrente * resistencia;
			   
			printf("A tensao resultante e: %f volts", tensao);
			break;

        case 6:
            printf("Digite a corrente em amperes: ");
            scanf("%f", &i);

            printf("Digite a resistencia em ohms: ");
            scanf("%f", &r);

            p = (r x i²);

            printf("A tensao resultante e: %f volts", p);
            break;

        case 7:
            printf("Digite a tensao em volts: ");
            scanf("%f", &v);

            printf("Digite a corrente em amperes: ");
            scanf("%f", &i);

            p = v * i;

            printf("A potencia em watts eh: %.2f W\n", p);
            break;

        case 8:
            printf("Digite a corrente em amperes: ");
            scanf("%f", &corrente);

            printf("Digite a resistencia em ohms: ");
            scanf("%f", &resistencia);

            tensao = corrente * resistencia;

            printf("A tensao resultante e: %f volts", tensao);
            break;

        case 9:
            printf("Digite a resistencia em ohms: ");
            scanf("%f", &resistencia);

            printf("Digite a tensao em volts: ");
            scanf("%f", &tensao);

            corrente = tensao / resistencia;

            printf("A corrente resultante e: %f amperes", corrente);
            break;
            
        case 10:
            printf("Digite a resistencia em ohms: ");
            scanf("%f", &r);

            printf("Digite a tensao em volts: ");
            scanf("%f", &v);

            
            p= (v² / r);

            printf("A corrente resultante e: %f amperes", p);
            break;

          
        default:
            printf("Opcao invalida!\n");
            break;
    }

    return 0;
}


