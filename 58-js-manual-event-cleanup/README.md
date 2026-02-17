# 🧨 Remoção Manual de Event Listeners

Este projeto demonstra a técnica clássica de controle de eventos no DOM, garantindo que uma ação seja disparada apenas uma vez através da remoção manual do ouvinte.

## 🚀 Conceitos Aplicados

### 1. Funções Nomeadas como Callback
Diferente das funções anônimas, definir uma função com nome (como `handleClick`) é obrigatório para que o `removeEventListener` funcione, pois o JavaScript precisa de uma referência exata da função que deve ser removida da memória.

### 2. Limpeza de Recursos (`Cleanup`)
A remoção de ouvintes de eventos é uma prática essencial para:
* **Performance**: Evita que o navegador continue "ouvindo" algo que não é mais necessário.
* **Lógica de Negócio**: Garante que ações de clique único (como finalização de compra ou logs de auditoria) não sejam repetidas por engano.

### 3. Acesso Dinâmico (Anti-Hardcode)
O uso de `event.target.textContent` garante que o log reflita exatamente o que está escrito no botão no momento da interação, tornando o código flexível e reutilizável.

## 🛠️ Como o código funciona
1. O evento é registrado vinculando o clique à função `handleClick`.
2. No primeiro clique, a função executa o `console.log`.
3. Logo após o log, a função executa `removeEventListener`, "desligando" o botão para cliques futuros.