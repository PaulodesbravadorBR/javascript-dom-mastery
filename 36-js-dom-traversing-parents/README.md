# 🪜 Percorrendo o DOM: Navegação Ascendente (Exercício 36)

Neste módulo, aprendemos como "viajar" pela estrutura do HTML a partir de um elemento filho.

### 🔍 Métodos Estudados:
* **`parentElement`**: Retorna o pai imediato. É útil quando você conhece a estrutura exata do seu HTML.
* **`closest(seletor)`**: Um "super buscador" que sobe na árvore até encontrar um ancestral que combine com o seletor CSS (muito útil para eventos em listas ou cards).



### ⚠️ Dica de Manutenção:
Embora `parentElement` e `closest()` sejam poderosos, o uso excessivo pode tornar seu JavaScript "frágil". Se você mudar uma `<div>` de lugar no HTML, a navegação pode quebrar. 
**Regra de ouro:** Sempre que possível, prefira selecionar elementos diretamente por `ID` ou `Classe` única.