# 🌗 Dark Mode Toggle (Exercício 33)

Este projeto demonstra a técnica mais eficiente para alternar estados visuais em uma página web: o uso de classes CSS gerenciadas pelo JavaScript.

### ✨ O que foi implementado:
* **Alternância Inteligente**: Uso do `classList.toggle("escuro")`, que verifica automaticamente se a classe existe (removendo-a) ou não (adicionando-a).
* **Escopo Global**: Aplicação da classe diretamente no `document.documentElement` (tag `<html>`), permitindo que seletores CSS descendentes alterem todo o layout do site.
* **Separação de Preocupações**: O JavaScript cuida apenas da lógica de alternância, enquanto o CSS cuida da aparência visual no modo escuro.

### 🛠️ Por que usar toggle?
Diferente de usar `add()` e `remove()` com condicionais `if/else`, o `toggle()` reduz as linhas de código e torna a manutenção muito mais simples, tratando a classe como um interruptor (On/Off).