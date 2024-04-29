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

5- 
