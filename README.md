🔍➡️ Busca Linear (Linear Search) 💻

Tecnologia Utilizada:
(c)
Sobre o Algoritmo
A Busca Linear é um algoritmo simples de busca que percorre uma lista de elementos sequencialmente até encontrar o elemento procurado ou até o final da lista.

Como Funciona
Iteração Sequencial: O algoritmo começa no início da lista e verifica cada elemento um por um até encontrar o elemento desejado ou até chegar ao final da lista.

Comparação: Para cada elemento na lista, o algoritmo compara o valor procurado com o valor do elemento atual. Se houver uma correspondência, o elemento é retornado; caso contrário, o algoritmo continua a busca.

Simplicidade: A Busca Linear é fácil de implementar e não requer que a lista esteja ordenada. No entanto, pode ser ineficiente para listas grandes, pois o tempo de execução é proporcional ao tamanho da lista.




Implementação

#include <stdio.h>
// Função de busca linear
int buscaLinear(int arr[], int tamanho, int chave) {
    for (int i = 0; i < tamanho; i++) {
        if (arr[i] == chave) {
            return i; // Retorna o índice do elemento encontrado
        }
    }
    return -1; // Retorna -1 se o elemento não for encontrado
    }
int main() {
    int arr[] = {10, 14, 19, 26, 27, 31, 33, 35, 42, 44};
    int chave = 33;
    int tamanho = sizeof(arr) / sizeof(arr[0]);
    int resultado = buscaLinear(arr, tamanho, chave);
    if (resultado == -1) {
        printf("Elemento não encontrado\n");
    } else {
        printf("Elemento encontrado no índice %d\n", resultado);
    }
    return 0;
}
linear_search-ezgif com-webp-to-gif-converter




Como rodar na minha maquina?
Primeiro Clone o repositorio na sua maquina:

git clone https://github.com/kaychenderson/LinearSearch
Para executar você precisa navegar até o diretório onde o arquivo c se encontra, e no terminal use este comando:

gcc main.c produto.c -o caixa_supermercado
./caixa_supermercado

Complexidade
Pior Caso:
O pior caso ocorre quando o elemento procurado está no final da lista ou não está presente, obrigando o algoritmo a verificar todos os elementos da lista. 
Portanto, a complexidade para o pior caso é O(n).

c1 * 1 + c2 * 1 + c3 * 1 + ... + c_n * 1 = O(n)
Melhor Caso:
O melhor caso ocorre quando o elemento procurado está no início da lista, e o algoritmo encontra o elemento imediatamente. 
Portanto, a complexidade para o melhor caso é O(1).

c1 * 1 + c2 * 1 = O(1)

Contribuidores:
Kayc Henderson;		
Renato Bento
