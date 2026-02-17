# 📊 Dataset & Data Attributes (Exercício 34)

Este exercício explora a forma padrão de armazenar e recuperar metadados diretamente em elementos HTML, uma técnica essencial para integrar dados do servidor com a lógica do Front-end.

### 🧠 O que aprendemos:
* **Ponte HTML/JS**: O prefixo `data-` no HTML mapeia diretamente para o objeto `.dataset` no JavaScript.
* **CamelCase Transformation**: Atributos como `data-id-usuario` tornam-se propriedades amigáveis como `idUsuario`.
* **Tipagem**: Lembre-se que o DOM trata tudo como texto. Para cálculos ou IDs numéricos, a conversão manual (`Number()`) é obrigatória.



### 🛠️ Por que usar Dataset?
É a maneira mais segura de "anexar" informações a um elemento (como o ID de um banco de dados) sem poluir os atributos padrão do navegador ou as classes de estilo.