
#include <stdio.h>

// Desafio Super Trunfo - Países
// Tema 2 - Comparação das Cartas
// Este código inicial serve como base para o desenvolvimento do sistema de comparação de cartas de cidades. 
// Siga os comentários para implementar cada parte do desafio.

int main() {
    // Definição das variáveis para armazenar as propriedades das cidades

    //Cadastro da Carta numero 1
    char codigo1[5];                //variavel string "codigo1" com tamanho maximo de caracteres
    char estado1[50];               //variavel string "estado1" com tamanho maximo de caracteres
    char cidade1[50];               //variavel string "cidade1" com tamanho maximo de caracteres
    int populacao1;                 //variavel int (numero inteiro) "populacao1"
    float area1;                     //variavel float (Numeros com casas decimais) area em km2
    float pib1;                     //variavel float (numeros com casas decimais) "pib1"
    int pontosturisticos1;          //variavel int (numeros inteiro) pontosturisticos1
    float densidade1, pibpercapta1; //variavel float (numeros com casas decimais) "densidade1 e pibpercapta1"

    //Cadastro da carta número 2
    char codigo2[5];               //variavel string "codigo2" com tamanho maximo de caracteres
    char estado2[50];               //variavel string "estado2" com tamanho maximo de caracteres
    char cidade2[50];                //variavel string "cidade2" com tamanho maximo de caracteres
    float area2;                    //variavel float (Numeros com casas decimais) area em km2
    int populacao2;                 //variavel int (numero inteiro) "populacao2"
    float pib2;                     //variavel float (numeros com casas decimais) "pib2"
    int pontosturisticos2;           //variavel int (numeros inteiro) "pontosturisticos2"
    float densidade2, pibpercapta2;  //variavel float (numeros com casas decimais) "densidade2 e pibpercapta2"

    // Você pode utilizar o código do primeiro desafio
    // Implemente a lógica para solicitar ao usuário que insira os dados das cidades
    // utilizando a função scanf para capturar as entradas.
    // utilize o código do primeiro desafio
    // Exemplo:
    // printf("Digite o código da cidade: ");
    // scanf("%s", codigo);
    // (Repita para cada propriedade)

    //Inserção de dados carta 1
    printf("****CARTA NUMERO 1****\n\n");
    printf("Insira o codigo da carta: \n");      //Mensagem para o usuario realizar a inserção do codigo da carta
    scanf("%s", codigo1);                        //Captura da inserção (codigo1) informado pelo usuario

    printf("Insira o nome do Estado: \n");       //Mensagem para o usuario realizar a inserção do codigo da carta
    scanf("%s", estado1);                        //Captura da inserção (estado1) informado pelo usuario

    printf("Insira a cidade: \n");               //Mensagem para o usuario realizar a inserção do codigo da carta
    scanf("%s", cidade1);                        //Captura da inserção (cidade1) informado pelo usuario
 
    printf("Insira o numero populacional: \n");  //Mensagem para o usuario realizar a inserção do codigo da carta
    scanf("%d", &populacao1);                     //Captura da inserção (populacao1) informado pelo usuario

    printf("Insira a area total em km2: \n");    //Mensagem para o usuario realizar a inserção do codigo da carta
    scanf("%f", &area1);                          //Captura da inserção (area1) informado pelo usuario

    printf("Insira o PIB: \n");                  //Mensagem para o usuario realizar a inserção do codigo da carta  
    scanf ("%f", &pib1);                          //Captura da inserção (pib1) informado pelo usuario

    printf("insira a quantidade de pontos turisticos: \n"); //Mensagem para o usuario realizar a inserção do codigo da carta
    scanf("%d", &pontosturisticos1);   

     //INSERÇÃO DE DADOS PELO USUARIO
    printf("\n****CARTA NUMERO 2****\n\n");
    printf("Insira o codigo da carta: \n");      //Mensagem para o usuario realizar a inserção do codigo da carta
    scanf("%s", codigo2);                        //Captura da inserção (codigo2) informado pelo usuario

    printf("Insira o nome do Estado: \n");       //Mensagem para o usuario realizar a inserção do codigo da carta
    scanf("%s", estado2);                        //Captura da inserção (estado2) informado pelo usuario

    printf("Insira a cidade: \n");               //Mensagem para o usuario realizar a inserção do codigo da carta
    scanf("%s", cidade2);                        //Captura da inserção (cidade2) informado pelo usuario
 
    printf("Insira o numero populacional: \n");  //Mensagem para o usuario realizar a inserção do codigo da carta
    scanf("%d", &populacao2);                     //Captura da inserção (populacao2) informado pelo usuario

    printf("Insira a area total em km2: \n");    //Mensagem para o usuario realizar a inserção do codigo da carta
    scanf("%f", &area2);                          //Captura da inserção (area2) informado pelo usuario

    printf("Insira o PIB: \n");                  //Mensagem para o usuario realizar a inserção do codigo da carta  
    scanf ("%f", &pib2);                          //Captura da inserção (pib2) informado pelo usuario

    printf("insira a quantidade de pontos turisticos: \n"); //Mensagem para o usuario realizar a inserção do codigo da carta
    scanf("%d", &pontosturisticos2);                        //Captura da inserção (pontosturisticos2) informado pelo usuario

    // Cálculos de densidade e pib percapta
    densidade1 = populacao1 / area1;
    pibpercapta1 = pib1 / populacao1;

    densidade2 = populacao2 / area2;
    pibpercapta2 = pib2 / populacao2; 

    //IMPRESSÃO DE RESULTADOS
    //DADOS INFORMADOS DA CARTA 1
    printf("\n****RESULTADOS****\n");
    printf("\n****CARTA 1****\n");
    printf("Codigo da Carta 1: %s \n", codigo1);
    printf("O Estado carta 1: %s\n", estado1);
    printf("A cidade carta 1: %s\n", cidade1);
    printf("Área territorial (km²): %.2f\n", area1);
    printf("A população carta 1: %d\n", populacao1);
    printf("O PIB da carta 1: %.2f\n", pib1);
    printf("Pontos Turisticos carta 1: %d\n", pontosturisticos1);
    printf("Densidade Populacional: %.2f hab/km²\n", densidade1);
    printf("PIB per capita: %.2f\n", pibpercapta1);

    //DADOS INFORMADOS DA CARTA 2
    printf("\n****CARTA 2****\n");
    printf("Codigo da Carta 2: %s\n", codigo2);
    printf("O Estado carta 2: %s\n", estado2);
    printf("A cidade carta 2: %s\n", cidade2);
    printf("Área territorial (km²): %.2f\n", area2);
    printf("A população carta 2: %d\n", populacao2);
    printf("O PIB da carta 2: %.2f\n", pib2);
    printf("Pontos Turisticos carta 2: %d\n", pontosturisticos2);
    printf("Densidade Populacional: %.2f hab/km²\n", densidade2);
    printf("PIB per capita: %.2f\n", pibpercapta2);



    return 0;
}
