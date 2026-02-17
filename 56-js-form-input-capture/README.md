# 📥 Projeto: Captura de Dados de Login com JavaScript

Este projeto pratica a manipulação de dados de entrada (inputs) do usuário em formulários HTML utilizando JavaScript.

## 🚀 Tecnologias Utilizadas
* HTML5 (Estrutura de formulários)
* CSS3 (Estilização de componentes)
* JavaScript (Manipulação de DOM e Eventos)

## 🧠 Conceitos Praticados

### 1. Captura de Valores (`element.value`)
Aprendi que para obter o texto digitado pelo usuário, devemos acessar a propriedade `.value` do elemento de input.
> **Ponto Crucial:** O valor deve ser lido **dentro** do evento de envio, caso contrário, obteremos apenas uma string vazia do carregamento inicial da página.

### 2. Evento de Submit e Fluxo de Dados
* **`event.preventDefault()`**: Utilizado para gerenciar o envio via JavaScript sem que a página recarregue.
* **Passagem de Argumentos**: Prática de coletar múltiplos valores (e-mail e senha) e enviá-los como argumentos para uma função de processamento (`processaLogin`).

## 🛠️ Como Funciona
Ao preencher os campos de e-mail e senha e clicar no botão de Login:
1. O evento `submit` é disparado.
2. O comportamento padrão do navegador é interrompido.
3. Os valores atuais dos campos são capturados e enviados para a lógica de autenticação.