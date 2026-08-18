### BIBLIOTECAS DA LINGUAGEM C
*   `<stdio.h>`: Standard Input Output (Entrada e Saída Padrão).
*   `<stdlib.h>`: Standard Library (Biblioteca Padrão). Usada para gerenciar memória, fazer contas complexas ou converter textos.
*   `<string.h>`: Usada para manipular textos.
*   `<ctype.h>`: Character Type. Usada para verificar caracteres isolados.

### APLICAÇÕES “DO C” EM PYTHON
*   **If/Else:** `&&` no C vira `and` no Python. `||` vira `or`. `!` vira `not`. `else if` vira `elif`.
*   **For:** No Python, o for itera diretamente sobre coleções (como listas) ou usa a função `range(início, parada, passo)` para gerar uma sequência numérica.

### Passagem por Valor x Referência (Python)
*   **Tipos Imutáveis (números, strings, booleanos):** Funcionam como a passagem por valor do C. Se alterar a variável dentro da função, a original não muda.
*   **Tipos Mutáveis (listas e dicionários):** Funcionam como a passagem por referência do C. Se você alterar lá dentro da função, vai alterar o dado original.

### Funções com número indefinido de parâmetros
*   `*args` (Arguments): Pega todos os parâmetros extras enviados por ordem e empacota em uma Tupla.
*   `**kwargs` (Keyword Arguments): Pega todos os parâmetros extras enviados com nome (`chave="valor"`) e empacota em um dicionário.

### Dicionário (dict) e JSON
O dicionário é a implementação nativa do Python para a Tabela Hash. Guarda pares de `chave: valor`.
```python
contato = {"nome": "Akemi", "telefone": "9999-8888"}
```
O JSON é baseado em texto simples e serve para gravar as informações que estão apenas na memória temporária do programa direto no disco rígido (`.json`).
```python
import json
with open("agenda.json", "w") as arquivo:
    json.dump(contatos, arquivo)
```
