# ⚡ Inserção Eficiente: insertAdjacentHTML (Exercício 38)

Este exercício foca na performance e nas boas práticas de manipulação do DOM ao lidar com listas dinâmicas.

### 🚀 Por que não usar `innerHTML +=`?
Quando usamos `innerHTML +=`, o navegador:
1. Converte todo o conteúdo atual em string.
2. Adiciona a nova string.
3. **Destrói** todos os elementos antigos.
4. **Recria** tudo do zero.
Isso apaga eventos (listeners) e consome muito processamento.

### ✅ A Solução: `insertAdjacentHTML`
Com `insertAdjacentHTML("beforeend", ...)`, o navegador apenas anexa o novo pedaço de HTML no lugar certo, mantendo o restante do DOM intacto.



### 🛠️ Explicação Técnica:
* **`beforeend`**: Adiciona o conteúdo logo antes do fechamento da tag pai (ou seja, como o último filho).
* **Template Strings**: O uso de crases (`` ` ``) permite interpolar as variáveis `${item}` de forma limpa e legível.