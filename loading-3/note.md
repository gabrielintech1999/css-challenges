O valor `alternate` no contexto da propriedade `animation` faz com que a animação vá e volte entre os estados definidos no `@keyframes`.

- **Sem o `alternate`**: A animação vai do estado inicial (`from`) até o final (`to`) e, em seguida, reinicia do começo (do `from` novamente).
- **Com o `alternate`**: A animação vai do estado inicial ao final, e depois volta do final para o início, criando um efeito de "vai e vem".

No seu caso, isso significa que o círculo alterna entre os dois estados do `@keyframes` — indo de `var(--color-dark)` para `var(--color-light)` e depois voltando, sem saltos abruptos.