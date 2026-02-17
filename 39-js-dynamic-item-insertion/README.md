# 🛒 Adição Incremental de Itens (Exercício 39)

Neste exercício, evoluímos a lógica de renderização. Em vez de processar um array inteiro de uma vez, criamos uma função capaz de lidar com a entrada de **um item por vez**.

### 🛠️ Funcionamento:
Cada vez que a função `adicionarItemListaDeCompras(item)` é executada:
1. Ela captura a referência da lista `<ul>`.
2. Ela "injeta" um novo elemento `<li>` no final da lista.
3. O conteúdo anterior não é afetado nem recriado.



### 💡 Por que isso é importante?
Esta é a base para criar interfaces interativas. Em um aplicativo real, você chamaria essa função quando o usuário clicasse em um botão "Adicionar" após preencher um campo de texto. Como o `insertAdjacentHTML` é eficiente, a página permanece rápida mesmo se a lista crescer consideravelmente.