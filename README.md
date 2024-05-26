# Pilha - Implementação em C++

Este projeto consiste em uma implementação simples de uma pilha em C++. Uma pilha é uma estrutura de dados que segue o princípio "último a entrar, primeiro a sair" (LIFO - Last In, First Out), onde o último elemento adicionado é o primeiro a ser removido.

## Funcionalidades

- **Push:** Adiciona um item ao topo da pilha.
- **Pop:** Remove o item do topo da pilha, se houver algum.
- **Top:** Retorna o item do topo da pilha, sem removê-lo.
- **Empty:** Permite verificar se a pilha está vazia.

## Como Usar

1. Instancie um objeto da classe `Pilha`.
2. Adicione elementos à pilha usando o método `push(item)`.
3. Remova elementos da pilha usando o método `pop()`.
4. Consulte o elemento do topo da pilha sem removê-lo usando o método `top()`.
5. Verifique se a pilha está vazia usando o método `empty()`.

## Exemplo de Uso

```Cpp
int main(){
    // Declare of the class
    Stack stack;

    // Fills the list with 100 numbers
    for (int i = 0; i < 101; i++) {
        stack.push(i);
        stack.printList();
        stack.sleepForOneSecond();
    }
    cout << endl;

    stack.printList();
    cout << "Aguarde..." << endl;
    stack.sleepForOneSecond();

    // Emptying the entire list
    while (not stack.empty()){
        int last_item_list = stack.top();
        stack.pop();
        cout << "Item removido da lista com sucesso: " << last_item_list << endl;
        stack.printList();
        stack.sleepForOneSecond();
    }

    return 0;
}
```

Este exemplo demonstra como preencher uma pilha com números de 0 a 100, imprimir a pilha, aguardar por alguns segundos e então remover cada elemento da pilha e imprimir a pilha resultante.

## Autor

Este código foi desenvolvido por Ageu Felipe Nunes Moraes(eu) como parte de um projeto pessoal dedicado ao fortalecimento e amadurecimento da codificação. Para quaisquer dúvidas ou sugestões, por favor, entre em contato pelo e-mail [ageumoraes67@gmail.com].

## Aviso Legal

Este é um projeto de software desenvolvido por um indivíduo e não tem afiliação com outrem.
