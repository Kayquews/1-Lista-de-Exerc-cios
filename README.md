# Lista-git
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

12- Faça um programa que lê as duas notas parciais obtidas por um aluno numa disciplina ao longo
de um semestre, e calcule a sua média. A atribuição de conceitos obedece à tabela abaixo:
1. Média de Aproveitamento Conceito
2. Entre 9.0 e 10.0 A
3. Entre 7.5 e 9.0 B
4. Entre 6.0 e 7.5 C
5. Entre 4.0 e 6.0 D
6. Entre 4.0 e zero E
O algoritmo deve mostrar na tela as notas, a média, o conceito correspondente e a mensagem
“APROVADO” se o conceito for A, B ou C ou “REPROVADO” se o conceito for D ou E.

#include <stdio.h>

int main() {
    // Declaração das variáveis
    float nota1, nota2, media;
    char conceito;

    // Solicita as notas ao usuário
    printf("Digite a primeira nota: ");
    scanf("%f", &nota1);
    printf("Digite a segunda nota: ");
    scanf("%f", &nota2);

    // Calcula a média
    media = (nota1 + nota2) / 2.0;

    // Determina o conceito com base na média
    if (media >= 9.0) {
        conceito = 'A';
    } else if (media >= 7.5) {
        conceito = 'B';
    } else if (media >= 6.0) {
        conceito = 'C';
    } else if (media >= 4.0) {
        conceito = 'D';
    } else {
        conceito = 'E';
    }

    // Imprime as notas, a média, o conceito correspondente e a situação do aluno
    printf("\nNotas: %.2f e %.2f\n", nota1, nota2);
    printf("Média: %.2f\n", media);
    printf("Conceito: %c\n", conceito);
    if (conceito == 'A' || conceito == 'B' || conceito == 'C') {
        printf("APROVADO\n");
    } else {
        printf("REPROVADO\n");
    }

    return 0;
}

13- Faça um programa que calcule as raízes de uma equação do segundo grau, na forma ax2 + bx +
c. O programa deverá pedir os valores de a, b e c e fazer as consistências, informando ao usuário
nas seguintes situações:
1. Se o usuário informar o valor de A igual a zero, a equação não é do segundo grau e o
programa não deve fazer pedir os demais valores, sendo encerrado;
2. Se o delta calculado for negativo, a equação não possui raizes reais. Informe ao usuário
e encerre o programa;
3. Se o delta calculado for igual a zero a equação possui apenas uma raiz real; informe-a
ao usuário;
4. Se o delta for positivo, a equação possui duas raiz reais; informe-as ao usuário;

#include <stdio.h>
#include <math.h>

int main() {
    // Declaração das variáveis
    float a, b, c, delta, raiz1, raiz2;

    // Solicita os valores de a, b e c ao usuário
    printf("Digite o valor de a: ");
    scanf("%f", &a);

    // Verifica se a equação é do segundo grau
    if (a == 0) {
        printf("A equação não é do segundo grau.\n");
        return 0; // Encerra o programa
    }

    printf("Digite o valor de b: ");
    scanf("%f", &b);
    printf("Digite o valor de c: ");
    scanf("%f", &c);

    // Calcula o delta
    delta = b * b - 4 * a * c;

    // Verifica o valor do delta e calcula as raízes
    if (delta < 0) {
        printf("A equação não possui raízes reais.\n");
    } else if (delta == 0) {
        raiz1 = -b / (2 * a);
        printf("A equação possui uma raiz real: %.2f\n", raiz1);
    } else {
        raiz1 = (-b + sqrt(delta)) / (2 * a);
        raiz2 = (-b - sqrt(delta)) / (2 * a);
        printf("A equação possui duas raízes reais: %.2f e %.2f\n", raiz1, raiz2);
    }

    return 0;
}
14- Faça um Programa que peça um número correspondente a um determinado ano e em seguida
informe se este ano é ou não bissexto.

#include <stdio.h>

int main() {
    // Declaração da variável para armazenar o ano
    int ano;

    // Solicita ao usuário o ano
    printf("Digite um ano: ");
    scanf("%d", &ano);

    // Verifica se o ano é bissexto
    if ((ano % 4 == 0 && ano % 100 != 0) || (ano % 400 == 0)) {
        printf("%d é um ano bissexto.\n", ano);
    } else {
        printf("%d não é um ano bissexto.\n", ano);
    }

    return 0;
}

15- Faça um Programa para um caixa eletrônico. O programa deverá perguntar ao usuário a valor do
saque e depois informar quantas notas de cada valor serão fornecidas. As notas disponíveis serão
as de 1, 5, 10, 50 e 100 reais. O valor mínimo é de 10 reais e o máximo de 600 reais. O programa
não deve se preocupar com a quantidade de notas existentes na máquina.
1. Exemplo 1: Para sacar a quantia de 256 reais, o programa fornece duas notas de 100,
uma nota de 50, uma nota de 5 e uma nota de 1;
2. Exemplo 2: Para sacar a quantia de 399 reais, o programa fornece três notas de 100,
uma nota de 50, quatro notas de 10, uma nota de 5 e quatro notas de 1.

#include <stdio.h>

int main() {
    // Declaração das variáveis
    int valor_saque, notas_100, notas_50, notas_10, notas_5, notas_1;

    // Solicita ao usuário o valor do saque
    printf("Digite o valor do saque (entre 10 e 600 reais): ");
    scanf("%d", &valor_saque);

    // Verifica se o valor do saque está dentro do intervalo permitido
    if (valor_saque < 10 || valor_saque > 600) {
        printf("Valor inválido para saque.\n");
        return 0; // Encerra o programa
    }

    // Calcula o número de notas de cada valor
    notas_100 = valor_saque / 100;
    valor_saque = valor_saque % 100;

    notas_50 = valor_saque / 50;
    valor_saque = valor_saque % 50;

    notas_10 = valor_saque / 10;
    valor_saque = valor_saque % 10;

    notas_5 = valor_saque / 5;
    valor_saque = valor_saque % 5;

    notas_1 = valor_saque;

    // Imprime as notas fornecidas ao usuário
    printf("\nNotas fornecidas para o saque:\n");
    printf("Notas de 100 reais: %d\n", notas_100);
    printf("Notas de 50 reais: %d\n", notas_50);
    printf("Notas de 10 reais: %d\n", notas_10);
    printf("Notas de 5 reais: %d\n", notas_5);
    printf("Notas de 1 real: %d\n", notas_1);

    return 0;
}

16- Faça um Programa que leia 2 números e em seguida pergunte ao usuário qual operação ele deseja
realizar. O resultado da operação deve ser acompanhado de uma frase que diga se o número é:
1. par ou ímpar;
2. positivo ou negativo;
3. inteiro ou decimal.

#include <stdio.h>

int main() {
    // Declaração das variáveis
    float num1, num2, resultado;
    char operacao;

    // Solicita os dois números ao usuário
    printf("Digite o primeiro número: ");
    scanf("%f", &num1);
    printf("Digite o segundo número: ");
    scanf("%f", &num2);

    // Solicita ao usuário a operação desejada
    printf("Escolha a operação desejada:\n");
    printf("1. Soma (+)\n");
    printf("2. Subtração (-)\n");
    printf("3. Multiplicação (*)\n");
    printf("4. Divisão (/)\n");
    printf("Operação: ");
    scanf(" %c", &operacao);

    // Realiza a operação escolhida
    switch (operacao) {
        case '+':
            resultado = num1 + num2;
            printf("Resultado da soma: %.2f\n", resultado);
            break;
        case '-':
            resultado = num1 - num2;
            printf("Resultado da subtração: %.2f\n", resultado);
            break;
        case '*':
            resultado = num1 * num2;
            printf("Resultado da multiplicação: %.2f\n", resultado);
            break;
        case '/':
            // Verifica se o segundo número é zero para evitar divisão por zero
            if (num2 == 0) {
                printf("Erro: divisão por zero!\n");
                break;
            }
            resultado = num1 / num2;
            printf("Resultado da divisão: %.2f\n", resultado);
            break;
        default:
            printf("Operação inválida!\n");
            return 0; // Encerra o programa
    }

    // Verifica se o resultado é par ou ímpar
    if ((int)resultado % 2 == 0) {
        printf("O resultado é par.\n");
    } else {
        printf("O resultado é ímpar.\n");
    }

    // Verifica se o resultado é positivo ou negativo
    if (resultado > 0) {
        printf("O resultado é positivo.\n");
    } else if (resultado < 0) {
        printf("O resultado é negativo.\n");
    } else {
        printf("O resultado é zero.\n");
    }

    // Verifica se o resultado é inteiro ou decimal
    if (resultado == (int)resultado) {
        printf("O resultado é um número inteiro.\n");
    } else {
        printf("O resultado é um número decimal.\n");
    }

    return 0;
}
17- Faça um programa que faça 5 perguntas para uma pessoa sobre um crime. As perguntas são:
1. "Telefonou para a vítima?"
2. "Esteve no local do crime?"
3. "Mora perto da vítima?"
4. "Devia para a vítima?"
5. "Já trabalhou com a vítima?" O programa deve no final emitir uma classificação sobre a
participação da pessoa no crime. Se a pessoa responder positivamente a 2 questões ela
deve ser classificada como "Suspeita", entre 3 e 4 como "Cúmplice" e 5 como
"Assassino". Caso contrário, ele será classificado como "Inocente".

#include <stdio.h>

int main() {
    // Declaração das variáveis para armazenar as respostas
    char resposta1, resposta2, resposta3, resposta4, resposta5;

    // Pergunta ao usuário sobre o crime
    printf("Responda com 'S' para Sim ou 'N' para Não.\n");
    printf("1. Telefonou para a vítima? ");
    scanf(" %c", &resposta1);
    printf("2. Esteve no local do crime? ");
    scanf(" %c", &resposta2);
    printf("3. Mora perto da vítima? ");
    scanf(" %c", &resposta3);
    printf("4. Devia para a vítima? ");
    scanf(" %c", &resposta4);
    printf("5. Já trabalhou com a vítima? ");
    scanf(" %c", &resposta5);

    // Conta o número de respostas positivas
    int num_respostas_positivas = 0;
    if (resposta1 == 'S' || resposta1 == 's') {
        num_respostas_positivas++;
    }
    if (resposta2 == 'S' || resposta2 == 's') {
        num_respostas_positivas++;
    }
    if (resposta3 == 'S' || resposta3 == 's') {
        num_respostas_positivas++;
    }
    if (resposta4 == 'S' || resposta4 == 's') {
        num_respostas_positivas++;
    }
    if (resposta5 == 'S' || resposta5 == 's') {
        num_respostas_positivas++;
    }

    // Classifica a participação da pessoa no crime
    if (num_respostas_positivas == 2) {
        printf("Você é suspeito.\n");
    } else if (num_respostas_positivas >= 3 && num_respostas_positivas <= 4) {
        printf("Você é cúmplice.\n");
    } else if (num_respostas_positivas == 5) {
        printf("Você é o assassino.\n");
    } else {
        printf("Você é inocente.\n");
    }

    return 0;
}

18- Uma fruteira está vendendo frutas com a seguinte tabela de preços:
1. Até 5 Kg Acima de 5 Kg
2. Morango R$ 2,50 por Kg R$ 2,20 por Kg
3. Maçã R$ 1,80 por Kg R$ 1,50 por Kg
Se o cliente comprar mais de 8 Kg em frutas ou o valor total da compra ultrapassar R$
25,00, receberá ainda um desconto de 10% sobre este total. Escreva um algoritmo para
ler a quantidade (em Kg) de morangos e a quantidade (em Kg) de maças adquiridas e
escreva o valor a ser pago pelo cliente.

#include <stdio.h>

int main() {
    // Declaração das variáveis
    float kg_morangos, kg_macas, valor_total;

    // Solicita ao usuário a quantidade de morangos e maçãs adquiridas
    printf("Digite a quantidade de morangos (em Kg): ");
    scanf("%f", &kg_morangos);
    printf("Digite a quantidade de maçãs (em Kg): ");
    scanf("%f", &kg_macas);

    // Calcula o valor total da compra
    float preco_morangos, preco_macas;
    if (kg_morangos <= 5) {
        preco_morangos = 2.50 * kg_morangos;
    } else {
        preco_morangos = 2.20 * kg_morangos;
    }
    if (kg_macas <= 5) {
        preco_macas = 1.80 * kg_macas;
    } else {
        preco_macas = 1.50 * kg_macas;
    }
    valor_total = preco_morangos + preco_macas;

    // Aplica o desconto, se necessário
    if (kg_morangos + kg_macas > 8 || valor_total > 25.00) {
        valor_total *= 0.90; // Aplica o desconto de 10%
    }

    // Imprime o valor a ser pago pelo cliente
    printf("Valor a ser pago pelo cliente: R$ %.2f\n", valor_total);

    return 0;
}

19- O Hipermercado Tabajara está com uma promoção de carnes que é imperdível. Confira:
1. Até 5 Kg Acima de 5 Kg
2. File Duplo R$ 4,90 por Kg R$ 5,80 por Kg
3. Alcatra R$ 5,90 por Kg R$ 6,80 por Kg
4. Picanha R$ 6,90 por Kg R$ 7,80 por Kg
Para atender a todos os clientes, cada cliente poderá levar apenas um dos tipos de carne
da promoção, porém não há limites para a quantidade de carne por cliente. Se compra
for feita no cartão Tabajara o cliente receberá ainda um desconto de 5% sobre o total da
compra. Escreva um programa que peça o tipo e a quantidade de carne comprada pelo
usuário e gere um cupom fiscal, contendo as informações da compra: tipo e quantidade
de carne, preço total, tipo de pagamento, valor do desconto e valor a pagar.

#include <stdio.h>

int main() {
    // Declaração das variáveis
    char tipo_carne;
    float kg_carne, preco_kg, preco_total, desconto, valor_final;

    // Solicita ao usuário o tipo e a quantidade de carne comprada
    printf("Digite o tipo de carne (F - Filé Duplo, A - Alcatra, P - Picanha): ");
    scanf(" %c", &tipo_carne);
    printf("Digite a quantidade de carne (em Kg): ");
    scanf("%f", &kg_carne);

    // Determina o preço por Kg de acordo com o tipo de carne
    switch (tipo_carne) {
        case 'F':
        case 'f':
            if (kg_carne <= 5) {
                preco_kg = 4.90;
            } else {
                preco_kg = 5.80;
            }
            break;
        case 'A':
        case 'a':
            if (kg_carne <= 5) {
                preco_kg = 5.90;
            } else {
                preco_kg = 6.80;
            }
            break;
        case 'P':
        case 'p':
            if (kg_carne <= 5) {
                preco_kg = 6.90;
            } else {
                preco_kg = 7.80;
            }
            break;
        default:
            printf("Tipo de carne inválido.\n");
            return 0; // Encerra o programa
    }

    // Calcula o preço total da compra
    preco_total = kg_carne * preco_kg;

    // Verifica se o cliente pagará com cartão Tabajara e aplica o desconto, se necessário
    char tipo_pagamento;
    printf("Pagamento com cartão Tabajara? (S - Sim, N - Não): ");
    scanf(" %c", &tipo_pagamento);
    if (tipo_pagamento == 'S' || tipo_pagamento == 's') {
        desconto = preco_total * 0.05; // Desconto de 5%
    } else {
        desconto = 0;
    }

    // Calcula o valor final a ser pago pelo cliente
    valor_final = preco_total - desconto;

    // Imprime o cupom fiscal
    printf("\nCUPOM FISCAL\n");
    printf("Tipo de carne: ");
    switch (tipo_carne) {
        case 'F':
        case 'f':
            printf("Filé Duplo\n");
            break;
        case 'A':
        case 'a':
            printf("Alcatra\n");
            break;
        case 'P':
        case 'p':
            printf("Picanha\n");
            break;
    }
    printf("Quantidade de carne: %.2f Kg\n", kg_carne);
    printf("Preço total: R$ %.2f\n", preco_total);
    if (desconto > 0) {
        printf("Tipo de pagamento: Cartão Tabajara\n");
        printf("Valor do desconto: R$ %.2f\n", desconto);
    } else {
        printf("Tipo de pagamento: Dinheiro ou outro cartão\n");
    }
    printf("Valor a pagar: R$ %.2f\n", valor_final);

    return 0;
}

20- Faça um Programa que leia um número inteiro menor que 1000 e imprima a quantidade de
centenas, dezenas e unidades dele. Observando os termos no plural a colocação do "e", da vírgula
entre outros. Exemplo:
326 = 3 centenas, 2 dezenas e 6 unidades
12 = 1 dezena e 2 unidades
Testar com: 326, 300, 100, 320, 310,305, 301, 101, 311, 111, 25, 20, 10, 21, 11, 1, 7 e 16

#include <stdio.h>

int main() {
    // Declaração da variável para armazenar o número
    int num;

    // Solicita ao usuário um número inteiro menor que 1000
    printf("Digite um número inteiro menor que 1000: ");
    scanf("%d", &num);

    // Verifica se o número está dentro do intervalo permitido
    if (num < 1 || num >= 1000) {
        printf("Número inválido.\n");
        return 0; // Encerra o programa
    }

    // Calcula a quantidade de centenas, dezenas e unidades
    int centenas = num / 100;
    int dezenas = (num % 100) / 10;
    int unidades = num % 10;

    // Imprime a quantidade de centenas, dezenas e unidades
    printf("%d = ", num);

    // Imprime a quantidade de centenas
    if (centenas > 0) {
        printf("%d centena%s", centenas, (centenas > 1) ? "s" : "");
        if (dezenas > 0 || unidades > 0) {
            printf(", ");
        }
    }

    // Imprime a quantidade de dezenas
    if (dezenas > 0) {
        printf("%d dezena%s", dezenas, (dezenas > 1) ? "s" : "");
        if (unidades > 0) {
            printf(" e ");
        }
    }

    // Imprime a quantidade de unidades
    if (unidades > 0 || (centenas == 0 && dezenas == 0)) {
        printf("%d unidade%s", unidades, (unidades > 1) ? "s" : "");
    }

    printf("\n");

    return 0;
}






