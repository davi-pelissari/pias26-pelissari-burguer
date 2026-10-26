# pias26-pelissari-burguer
#include <stdio.h>
#include <stdlib.h>

int main() {
    // 1. Declarar um ponteiro para o arquivo
    FILE *arquivo;

    // 2. Abrir/criar o arquivo no modo de escrita ("w")
    arquivo = fopen("exemplo.txt", "w");

    // 3. Verificar se o arquivo foi criado com sucesso
    if (arquivo == NULL) {
        printf("Erro ao tentar criar o arquivo!\n");
        return 1;
    }

    // 4. Escrever conteúdo no arquivo
    fprintf(arquivo, "Olá! Este arquivo foi criado em C.\n");

    // 5. Fechar o arquivo
    fclose(arquivo);

    printf("Arquivo criado com sucesso!\n");
    return 0;
}
