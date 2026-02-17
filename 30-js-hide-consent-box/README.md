# 🙈 Interactive UI Hiding (Exercício 30)

Este exercício demonstra como remover visualmente elementos da interface em resposta a interações do usuário, simulando um fluxo de aceitação de termos ou cookies.

### 💡 Conceitos Aplicados:
* **Manipulação de Style**: Uso de `element.style.display = "none"` para remover o elemento do layout.
* **Escopo de Função**: Criação de uma função dedicada à alteração estética de um componente específico.
* **Event Listening**: Integração com disparadores de clique para acionar mudanças de estado no DOM.

### 🛠️ Diferença de Abordagem:
Ao contrário de apenas mudar a opacidade (`opacity: 0`), o uso de `display: none` garante que o elemento não ocupe mais espaço na tela, permitindo que o conteúdo abaixo suba e preencha o vazio deixado pelo banner de consentimento.