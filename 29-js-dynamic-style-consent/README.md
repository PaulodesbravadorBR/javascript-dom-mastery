# 🌍 Dynamic Consent UI (Exercício 29)

Este projeto simula um sistema de consentimento de dados (GDPR) que exibe mensagens específicas apenas para usuários localizados na União Europeia.

### ✨ O que foi praticado:
* **Manipulação de Style**: Uso da propriedade `element.style.display` para controlar visibilidade.
* **Lógica Condicional**: Aplicação de estilos baseada em propriedades de objetos (`ehDaUniaoEuropeia`).
* **Valores CSS Iniciais**: Uso de strings vazias `""` para redefinir o comportamento padrão do elemento no navegador.

### 🛠️ Diferença Técnica:
Embora o uso de classes (`classList`) seja recomendado para estilos estáticos, a propriedade `.style` é essencial quando precisamos de mudanças rápidas e diretas baseadas em lógica de programação ou cálculos dinâmicos.