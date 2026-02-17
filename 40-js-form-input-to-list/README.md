# ✍️ Do Input para a Tela (Exercício 40)

Este exercício é a união de tudo o que vimos até agora: seleção de elementos, manipulação de texto e inserção eficiente no DOM.

### 🕹️ Como testar:
1. Abra o arquivo no navegador.
2. Digite algo no campo "Item name".
3. Clique em **Add** ou aperte **Enter**.
4. Veja a mágica acontecer: o item aparece na lista e o valor é registrado no Console (`F12`).

### 🛠️ O que está acontecendo por baixo dos panos?
O navegador está usando um **Event Listener** (ouvintes de eventos). Quando o formulário é enviado (`submit`), ele captura o `value` do seu input e o envia para a nossa função `adicionarItemDaComprasDeLista`.



### 💡 Por que `insertAdjacentHTML` brilha aqui?
Se tivéssemos 100 itens na lista e usássemos `innerHTML`, o navegador teria que reconstruir os 100 itens toda vez que você adicionasse um novo. Com `insertAdjacentHTML`, ele apenas adiciona o 101º item, mantendo a performance impecável!