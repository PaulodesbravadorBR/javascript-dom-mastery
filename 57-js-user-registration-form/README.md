# 📝 Formulário de Registro de Usuário

Este projeto simula o fluxo de captura de dados para um sistema de cadastro, utilizando manipulação de DOM e eventos de formulário.

## 🚀 Tecnologias Utilizadas
* HTML5
* CSS3 (Custom Variables/Themes)
* JavaScript (ES6)

## 🧠 Conceitos Aplicados

### Manipulação de Eventos
A captura de dados é feita através do evento `submit` disparado pelo formulário. Isso permite uma experiência de usuário melhor, pois aceita tanto o clique no botão quanto a tecla "Enter".

### Prevenção de Comportamento Padrão
O uso de `event.preventDefault()` é fundamental para que o processamento dos dados ocorra no lado do cliente (front-end) sem a necessidade de atualizar a página, permitindo integrações futuras com APIs.

### Funções de Callback
Os dados coletados (`value`) são organizados e passados como argumentos para uma função de processamento (`registroCompleto`), simulando o envio de um objeto para um banco de dados.

## 🛠️ Como usar
1. Preencha os campos Nome, E-mail e Senha.
2. Clique em 'Register'.
3. Abra o console do navegador para ver o objeto de dados capturado.