# 🗑️ DOM Element Removal (Exercício 32)

Este exercício foca na exclusão definitiva de nós do DOM em resposta a eventos do usuário.

### ✨ Conceitos Praticados:
* **Método `.remove()`**: Diferente de `display: none` (que apenas esconde), o `.remove()` deleta o elemento da árvore do documento.
* **Segurança no Código**: Implementação de uma verificação condicional (`if (mensagem)`) para garantir que a função não tente remover algo que já foi excluído.
* **Acesso Direto**: Diferença entre limpar o conteúdo (`innerHTML = ""`) e remover a tag inteira.

### 💡 Dica Técnica:
Ao usar `document.body` ou `document.documentElement`, você acessa as raízes do seu projeto. Já o `.remove()` é a ferramenta de "limpeza" cirúrgica para elementos específicos como modais, alertas ou mensagens de boas-vindas.