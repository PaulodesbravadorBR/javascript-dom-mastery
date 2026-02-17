# 🎯 Advanced DOM Selectors Mastery

Este projeto demonstra a aplicação de seletores CSS avançados dentro do JavaScript para filtrar elementos de forma precisa. O foco aqui não é apenas "pegar elementos", mas sim aplicar **especificidade e hierarquia**.

## 🚀 O que este projeto cobre?
Diferente de seletores simples, aqui explorei três níveis de busca no DOM:
1. **Seleção Global**: Capturar todos os elementos de um tipo (`div`).
2. **Seleção por Descendência**: Filtrar links específicos dentro de um container (`#footer-wrapper a`).
3. **Seleção por Classe**: Agrupar elementos relacionados espalhados pela página (`a.about`).

## 🧠 Conceitos Técnicos
- **Descendant Combinators**: Entender como o espaço entre seletores permite navegar na hierarquia do HTML.
- **Tag + Class Specificity**: Combinar o nome da tag com a classe para uma busca mais performática e segura.
- **NodeList Management**: Lidar com coleções de elementos retornadas pelo `querySelectorAll`.

## 💻 Exemplo de Implementação
```javascript
// Busca refinada: Apenas links que estão dentro do rodapé
const obterFooterLinks = () => {
    return document.querySelectorAll("#footer-wrapper a");
}
