# 📝 Exercício: Manipulação de Formulários e Operadores Modernos

Este projeto foi desenvolvido para praticar conceitos fundamentais de JavaScript moderno (ES6+), focando na manipulação de eventos de formulário e no uso de novos operadores para segurança de dados.

## 🚀 Tecnologias Utilizadas
* HTML5
* CSS3
* JavaScript (ES6+)

## 🧠 Conceitos Praticados

### 1. Coalescência Nula (`??`)
Utilizado para definir valores padrão de forma segura. Diferente do operador `||`, o `??` só age quando o valor é `null` ou `undefined`, preservando valores válidos como `0` ou `""`.
> **Exemplo:** `usuario.idade ?? "desconhecido"`

### 2. Encadeamento Opcional (`?.`)
Utilizado para acessar propriedades de objetos profundamente aninhados sem causar erros caso uma das propriedades no caminho não exista.

### 3. Manipulação de Formulários (`submit`)
* **`event.preventDefault()`**: Essencial para evitar o recarregamento da página durante o envio, permitindo que o JavaScript processe os dados de forma assíncrona.
* **Event Listeners**: Captura do evento de envio diretamente no elemento `<form>`.

## 🛠️ Como rodar o projeto
1. Clone este repositório.
2. Abra o arquivo `index.html` em seu navegador.
3. Abra o console do desenvolvedor (F12) para visualizar os logs de envio.