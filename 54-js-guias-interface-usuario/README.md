# 📑 Interface de Guias (Tabs UI) - Exercício 54

Este projeto faz parte da trilha de desenvolvimento JavaScript e foca na criação de componentes de interface reutilizáveis e lógicos.

### 🛠️ Tecnologias e Conceitos:
* **Seletores de Escopo**: Uso de `.guias .guia` para isolar a lógica do componente e evitar conflitos com outros botões da página.
* **Manipulação de Classes**: Alternância dinâmica entre as classes `active` (para destaque visual da aba) e `show` (para controle de visibilidade do conteúdo).
* **Atributos de Dados (Dataset)**: Utilização de `data-content` no HTML para armazenar seletores CSS, permitindo um código JavaScript mais limpo e independente de IDs fixos.

### ⚙️ Como funciona a lógica:
1. O script monitora o clique em qualquer elemento `.guia` dentro do container `.guias`.
2. Ao clicar, um loop limpa o estado ativo de todas as abas e conteúdos.
3. O `this.dataset.content` identifica qual parágrafo deve ser exibido.
4. As classes são aplicadas para atualizar a interface instantaneamente.

---
*Projeto desenvolvido como parte do desafio técnico SENAI Dev.*