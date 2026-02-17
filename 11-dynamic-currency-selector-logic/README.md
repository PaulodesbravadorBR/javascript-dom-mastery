# 💱 Dynamic Currency Selector

Este projeto simula a lógica de seleção de preferências do usuário em uma plataforma financeira. O foco principal é a transformação de elementos de interface (DOM) em dados estruturados (Arrays).

## 🛠️ Tecnologias e Conceitos
- **Spread Operator (`...`)**: Utilizado para converter coleções de nós do DOM (NodeList) em Arrays funcionais.
- **Array.map()**: Aplicado para extrair metadados específicos (`textContent`) de uma coleção de elementos.
- **Dynamic CSS Classes**: Interação com estados ativos/inativos para filtragem de dados.

## 💻 Como funciona
A função `obterMoedasSelecionadas` identifica quais "cards" o usuário clicou (marcados com a classe `.active`), converte essa lista e retorna um array simplificado com as siglas das moedas, pronto para ser enviado a uma API ou banco de dados.

```javascript
const obterMoedasSelecionadas = () => {
    const cardsAtivos = document.querySelectorAll(".card.active");
    return [...cardsAtivos].map(card => card.textContent);
}
