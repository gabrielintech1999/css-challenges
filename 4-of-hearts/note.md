Quando você usa valores negativos na função `scale()` no CSS, ocorre um **espelhamento** ou **inversão** do elemento em torno de um ou ambos os eixos (dependendo se o valor negativo é aplicado ao eixo X, Y ou ambos).

### Explicação:

A função `scale()` é usada para redimensionar um elemento. Ela pode aceitar dois parâmetros:
- **`scaleX(n)`**: Aplica o fator de escala no eixo X (horizontal).
- **`scaleY(n)`**: Aplica o fator de escala no eixo Y (vertical).

### Comportamento com valores negativos:

1. **`scaleX(-1)`**:
   - Inverte o elemento no eixo **horizontal** (espelha da esquerda para a direita).
   - O elemento é virado ao contrário, como se estivesse olhando em um espelho vertical.
   
   Exemplo:
   ```css
   transform: scaleX(-1);
   ```

2. **`scaleY(-1)`**:
   - Inverte o elemento no eixo **vertical** (espelha de cima para baixo).
   - O elemento é virado de cabeça para baixo.

   Exemplo:
   ```css
   transform: scaleY(-1);
   ```

3. **`scale(-1)`**:
   - Quando você aplica apenas um valor negativo para `scale(-1)`, ele aplica tanto no eixo X quanto no Y, o que significa que o elemento será invertido em ambos os eixos (ficará de cabeça para baixo e também espelhado horizontalmente).

   Exemplo:
   ```css
   transform: scale(-1);
   ```

### Exemplos visuais:

- **`scaleX(-1)`**: O elemento fica invertido como se estivesse virado para o lado.
- **`scaleY(-1)`**: O elemento fica de cabeça para baixo.
- **`scale(-1)`**: O elemento é invertido tanto horizontalmente quanto verticalmente, como se estivesse "espelhado" e "de cabeça para baixo" ao mesmo tempo.

### Exemplo prático:

```css
.inverted-horizontal {
    transform: scaleX(-1); /* Espelha no eixo X */
}

.inverted-vertical {
    transform: scaleY(-1); /* Espelha no eixo Y */
}

.inverted-both {
    transform: scale(-1); /* Espelha nos dois eixos */
}
```

Isso é útil para criar efeitos visuais interessantes, como espelhar imagens ou transformar elementos em diferentes direções.