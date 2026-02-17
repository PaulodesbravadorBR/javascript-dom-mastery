# 🎯 Busca Inteligente: Closest + Dataset (Exercício 37)

Este exercício demonstra uma das técnicas mais poderosas para lidar com interfaces dinâmicas, como listas de cards ou tabelas.

### 💡 O Problema:
Imagine que você tem um botão de "Excluir" dentro de um card. O ID do usuário está no card (o pai), mas o clique acontece no botão (o filho). Como o botão sabe qual ID deletar?

### 🛠️ A Solução:
Usamos o `closest(".classe")`. Diferente do `parentElement`, que sobe apenas um nível, o `closest` sobe quantos níveis forem necessários até encontrar o seletor especificado.

1. **Subida**: `elemento.closest(".cartao-usuario")` localiza o container principal.
2. **Extração**: `.dataset.userId` lê o valor armazenado no HTML.
3. **Conversão**: `Number()` transforma o texto em um número utilizável.



### ✅ Vantagem:
Essa abordagem é extremamente resiliente. Se você adicionar uma `<div>` extra ao redor do texto ou do botão, o código continua funcionando perfeitamente, pois ele não depende de uma estrutura rígida, mas sim da presença da classe no ancestral.