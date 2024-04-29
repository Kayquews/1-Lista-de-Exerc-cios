# 1-Lista-de-Exerc-cios
Listas de exercício 

1- Faça um Programa que peça dois números e imprima o maior deles.
#include <stdio.h>

int main() {
    // Declaração das variáveis
    float numero1, numero2;

    // Solicita dois números ao usuário
    printf("Digite o primeiro número: ");
    scanf("%f", &numero1);
    printf("Digite o segundo número: ");
    scanf("%f", &numero2);

    // Verifica qual é o maior número
    float maior_numero;
    if (numero1 > numero2) {
        maior_numero = numero1;
    } else {
        maior_numero = numero2;
    }

    // Imprime o maior número
    printf("O maior número é: %.2f\n", maior_numero);

    return 0;
}

2- Faça um Programa que peça um valor e mostre na tela se o valor é positivo ou negativo.

#include <stdio.h>

int main() {
    // Declaração da variável
    float valor;

    // Solicita um valor ao usuário
    printf("Digite um valor: ");
    scanf("%f", &valor);

    // Verifica se o valor é positivo, negativo ou zero
    if (valor > 0) {
        printf("O valor %.2f é positivo.\n", valor);
    } else if (valor < 0) {
        printf("O valor %.2f é negativo.\n", valor);
    } else {
        printf("O valor é zero.\n");
    }

    return 0;
}

3- Faça um Programa que verifique se uma letra digitada é "F" ou "M". Conforme a letra escrever: F
- Feminino, M - Masculino, Sexo Inválido.
 
#include <stdio.h>

int main() {
    // Declaração da variável para armazenar a letra
    char letra;

    // Solicita uma letra ao usuário
    printf("Digite uma letra (F/M): ");
    scanf(" %c", &letra); // Note o espaço antes de %c para consumir qualquer espaço em branco ou quebra de linha pendente

    // Verifica se a letra é "F" ou "M" e imprime a mensagem correspondente
    if (letra == 'F' || letra == 'f') {
        printf("F - Feminino\n");
    } else if (letra == 'M' || letra == 'm') {
        printf("M - Masculino\n");
    } else {
        printf("Sexo Inválido\n");
    }

    return 0;
}

4- Faça um Programa que verifique se uma letra digitada é vogal ou consoante.
#include <stdio.h>

#include <stdio.h>

int main() {
    // Declaração da variável para armazenar a letra
    char letra;

    // Solicita uma letra ao usuário
    printf("Digite uma letra: ");
    scanf(" %c", &letra);

    // Verifica se a letra é uma vogal minúscula
    if (letra == 'a' || letra == 'e' || letra == 'i' || letra == 'o' || letra == 'u' ||
        letra == 'A' || letra == 'E' || letra == 'I' || letra == 'O' || letra == 'U') {
        printf("A letra digitada '%c' é uma vogal.\n", letra);
    } else if ((letra >= 'a' && letra <= 'z') || (letra >= 'A' && letra <= 'Z')) {
        printf("A letra digitada '%c' é uma consoante.\n", letra);
    } else {
        printf("Caracter inválido.\n");
    }

    return 0;
}

5- Faça um Programa que leia três números e mostre o maior deles.

#include <stdio.h>

int main() {
    // Declaração das variáveis
    float numero1, numero2, numero3;

    // Solicita os três números ao usuário
    printf("Digite o primeiro número: ");
    scanf("%f", &numero1);
    printf("Digite o segundo número: ");
    scanf("%f", &numero2);
    printf("Digite o terceiro número: ");
    scanf("%f", &numero3);

    // Verifica qual é o maior número
    float maior_numero = numero1;
    if (numero2 > maior_numero) {
        maior_numero = numero2;
    }
    if (numero3 > maior_numero) {
        maior_numero = numero3;
    }

    // Imprime o maior número
    printf("O maior número é: %.2f\n", maior_numero);

    return 0;
}

6- Faça um Programa que leia três números e mostre o maior e o menor deles

#include <stdio.h>

int main() {
    // Declaração das variáveis
    float numero1, numero2, numero3;

    // Solicita os três números ao usuário
    printf("Digite o primeiro número: ");
    scanf("%f", &numero1);
    printf("Digite o segundo número: ");
    scanf("%f", &numero2);
    printf("Digite o terceiro número: ");
    scanf("%f", &numero3);

    // Inicializa as variáveis de maior e menor número
    float maior_numero = numero1;
    float menor_numero = numero1;

    // Verifica qual é o maior número
    if (numero2 > maior_numero) {
        maior_numero = numero2;
    }
    if (numero3 > maior_numero) {
        maior_numero = numero3;
    }

    // Verifica qual é o menor número
    if (numero2 < menor_numero) {
        menor_numero = numero2;
    }
    if (numero3 < menor_numero) {
        menor_numero = numero3;
    }

    // Imprime o maior e o menor número
    printf("O maior número é: %.2f\n", maior_numero);
    printf("O menor número é: %.2f\n", menor_numero);

    return 0;
}

7- Faça um programa que pergunte o preço de três produtos e informe qual produto você deve
comprar, sabendo que a decisão é sempre pelo mais barato.

#include <stdio.h>

int main() {
    // Declaração das variáveis para armazenar os preços
    float preco_produto1, preco_produto2, preco_produto3;

    // Solicita ao usuário os preços dos três produtos
    printf("Digite o preço do primeiro produto: ");
    scanf("%f", &preco_produto1);
    printf("Digite o preço do segundo produto: ");
    scanf("%f", &preco_produto2);
    printf("Digite o preço do terceiro produto: ");
    scanf("%f", &preco_produto3);

    // Verifica qual produto tem o menor preço
    if (preco_produto1 <= preco_produto2 && preco_produto1 <= preco_produto3) {
        printf("Você deve comprar o primeiro produto, que custa %.2f.\n", preco_produto1);
    } else if (preco_produto2 <= preco_produto1 && preco_produto2 <= preco_produto3) {
        printf("Você deve comprar o segundo produto, que custa %.2f.\n", preco_produto2);
    } else {
        printf("Você deve comprar o terceiro produto, que custa %.2f.\n", preco_produto3);
    }

    return 0;
}

8- Faça um Programa que leia três números e mostre-os em ordem decrescente

#include <stdio.h>

int main() {
    // Declaração das variáveis
    float numero1, numero2, numero3;

    // Solicita os três números ao usuário
    printf("Digite o primeiro número: ");
    scanf("%f", &numero1);
    printf("Digite o segundo número: ");
    scanf("%f", &numero2);
    printf("Digite o terceiro número: ");
    scanf("%f", &numero3);

    // Verifica e troca a ordem dos números, se necessário, para colocá-los em ordem decrescente
    if (numero1 < numero2) {
        float temp = numero1;
        numero1 = numero2;
        numero2 = temp;
    }
    if (numero2 < numero3) {
        float temp = numero2;
        numero2 = numero3;
        numero3 = temp;
    }
    if (numero1 < numero2) {
        float temp = numero1;
        numero1 = numero2;
        numero2 = temp;
    }

    // Imprime os números em ordem decrescente
    printf("Os números em ordem decrescente são: %.2f, %.2f, %.2f\n", numero1, numero2, numero3);

    return 0;
}

9- Faça um Programa que pergunte em que turno você estuda. Peça para digitar M-matutino ou VVespertino ou N- Noturno. Imprima a mensagem "Bom Dia!", "Boa Tarde!" ou "Boa Noite!" ou
"Valor Inválido!", conforme o caso.

#include <stdio.h>

int main() {
    // Declaração da variável para armazenar o turno
    char turno;

    // Solicita ao usuário o turno em que estuda
    printf("Em que turno você estuda?\n");
    printf("Digite M para Matutino, V para Vespertino ou N para Noturno: ");
    scanf(" %c", &turno);

    // Verifica o turno e imprime a mensagem correspondente
    switch (turno) {
        case 'M':
        case 'm':
            printf("Bom Dia!\n");
            break;
        case 'V':
        case 'v':
            printf("Boa Tarde!\n");
            break;
        case 'N':
        case 'n':
            printf("Boa Noite!\n");
            break;
        default:
            printf("Valor Inválido!\n");
    }

    return 0;
}

10- As Organizações Tabajara resolveram dar um aumento de salário aos seus colaboradores e lhe
contraram para desenvolver o programa que calculará os reajustes.
1. Faça um programa que recebe o salário de um colaborador e o reajuste segundo o
seguinte critério, baseado no salário atual:
2. salários até R$ 280,00 (incluindo) : aumento de 20%
3. salários entre R$ 280,00 e R$ 700,00 : aumento de 15%
4. salários entre R$ 700,00 e R$ 1500,00 : aumento de 10%
5. salários de R$ 1500,00 em diante : aumento de 5% Após o aumento ser realizado,
informe na tela:
6. o salário antes do reajuste;
7. o percentual de aumento aplicado;
8. o valor do aumento;
9. o novo salário, após o aumento.

#include <stdio.h>

int main() {
    // Declaração da variável para armazenar o salário
    float salario;

    // Solicita ao usuário o salário do colaborador
    printf("Digite o salário do colaborador: R$ ");
    scanf("%f", &salario);

    // Declaração de variáveis para armazenar o percentual de aumento e o valor do aumento
    float percentual_aumento;
    float valor_aumento;

    // Calcula o aumento de acordo com o salário atual
    if (salario <= 280.00) {
        percentual_aumento = 20.0;
    } else if (salario <= 700.00) {
        percentual_aumento = 15.0;
    } else if (salario <= 1500.00) {
        percentual_aumento = 10.0;
    } else {
        percentual_aumento = 5.0;
    }

    // Calcula o valor do aumento
    valor_aumento = salario * (percentual_aumento / 100.0);

    // Calcula o novo salário após o aumento
    float novo_salario = salario + valor_aumento;

    // Imprime as informações na tela
    printf("Salário antes do reajuste: R$ %.2f\n", salario);
    printf("Percentual de aumento aplicado: %.2f%%\n", percentual_aumento);
    printf("Valor do aumento: R$ %.2f\n", valor_aumento);
    printf("Novo salário após o aumento: R$ %.2f\n", novo_salario);

    return 0;
}

11- Faça um Programa que leia um número e exiba o dia correspondente da semana. (1-Domingo, 2-
Segunda, etc.), se digitar outro valor deve aparecer valor inválido.

#include <stdio.h>

int main() {
    // Declaração da variável para armazenar o número do dia
    int numero_dia;

    // Solicita ao usuário o número do dia
    printf("Digite um número de 1 a 7 para representar um dia da semana: ");
    scanf("%d", &numero_dia);

    // Verifica o número do dia e imprime o dia correspondente
    switch (numero_dia) {
        case 1:
            printf("Domingo\n");
            break;
        case 2:
            printf("Segunda-feira\n");
            break;
        case 3:
            printf("Terça-feira\n");
            break;
        case 4:
            printf("Quarta-feira\n");
            break;
        case 5:
            printf("Quinta-feira\n");
            break;
        case 6:
            printf("Sexta-feira\n");
            break;
        case 7:
            printf("Sábado\n");
            break;
        default:
            printf("Valor inválido\n");
    }

    return 0;
}





