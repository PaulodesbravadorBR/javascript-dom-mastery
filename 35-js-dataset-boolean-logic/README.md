# ⚖️ Lógica Booleana com Dataset (Exercício 35)

Este exercício resolve um dos "problemas" clássicos ao lidar com atributos HTML: a tipagem. Como o HTML só armazena strings, precisamos de lógica extra para tratar estados ativado/desativado.

### 🧩 O Desafio do "False"
No JavaScript, `Boolean("false")` retorna `true` porque a string não está vazia. 
Por isso, a técnica utilizada aqui:
* `const resultado = valor === "true"`

Garante que apenas o texto exato "true" seja convertido para o tipo booleano `true`, enquanto qualquer outra coisa (como "false", "undefined" ou vazio) resulte em `false`.

### 💡 Aplicação Prática:
Esta técnica é amplamente usada para verificar se um usuário está logado, se um modal deve estar aberto ou se um botão de "DarkMode" foi previamente ativado, tudo lendo metadados injetados no HTML pelo servidor.