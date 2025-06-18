#include <stdio.h>

int main() {
    // Definição das variáveis para os dados da Carta 1
    char estado;
    char codigo[100];
    char nome_da_cidade[100];
    int populacao;
    float area;
    float pib;
    int pontos_turisticos;

    // Entrada dos dados da Carta 1
    printf("Digite a letra do Estado: ");
    scanf(" %c", &estado);

    printf("Digite o código da cidade: ");
    scanf("%s", codigo);

    printf("Digite o nome da cidade: ");
    scanf(" %[^\n]", nome_da_cidade); // Permite leitura de espaços

    printf("Digite a população da cidade: ");
    scanf("%d", &populacao);

    printf("Digite a área da cidade (em km²): ");
    scanf("%f", &area);

    printf("Digite o PIB da cidade (em bilhões de reais): ");
    scanf("%f", &pib);

    printf("Digite o número de pontos turísticos: ");
    scanf("%d", &pontos_turisticos);

    // Exibição dos Dados da Carta
    printf("\n--- Dados da Carta de Cidade ---\n");
    printf("Estado: %c\n", estado);
    printf("Código: %s\n", codigo);
    printf("Nome da cidade: %s\n", nome_da_cidade);
    printf("População: %d habitantes\n", populacao);
    printf("Área: %.2f km²\n", area);
    printf("PIB: R$ %.2f bilhões\n", pib);
    printf("Número de pontos turísticos: %d\n", pontos_turisticos);

    return 0;
}
