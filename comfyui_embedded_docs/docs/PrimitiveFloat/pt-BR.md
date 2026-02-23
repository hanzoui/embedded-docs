> Esta documentação foi gerada por IA. Se você encontrar erros ou tiver sugestões de melhoria, sinta-se à vontade para contribuir! [Editar no GitHub](https://github.com/hanzoui/embedded-docs/blob/main/hanzo_studio_embedded_docs/docs/PrimitiveFloat/pt-BR.md)

O nó PrimitiveFloat cria um valor numérico de ponto flutuante que pode ser usado em seu fluxo de trabalho. Ele recebe uma única entrada numérica e emite esse mesmo valor, permitindo que você defina e passe valores float entre diferentes nós no seu pipeline do Hanzo Studio.

## Entradas

| Parâmetro | Tipo de Dados | Obrigatório | Intervalo | Descrição |
|-----------|-----------|----------|-------|-------------|
| `value` | FLOAT | Sim | -sys.maxsize a sys.maxsize | O valor numérico de ponto flutuante a ser emitido |

## Saídas

| Nome da Saída | Tipo de Dados | Descrição |
|-------------|-----------|-------------|
| `output` | FLOAT | O valor numérico de ponto flutuante de entrada |