> Esta documentação foi gerada por IA. Se você encontrar erros ou tiver sugestões de melhoria, sinta-se à vontade para contribuir! [Editar no GitHub](https://github.com/hanzoui/embedded-docs/blob/main/hanzo_studio_embedded_docs/docs/CLIPVisionLoader/pt-BR.md)

Este nó detecta automaticamente os modelos localizados na pasta `HanzoStudio/models/clip_vision`, bem como quaisquer caminhos de modelo adicionais configurados no arquivo `extra_model_paths.yaml`. Se você adicionar modelos após iniciar o Hanzo Studio, por favor **atualize a interface do Hanzo Studio** para garantir que os arquivos de modelo mais recentes sejam listados.

## Entradas

| Campo        | Tipo de Dados   | Descrição |
|--------------|-----------------|-----------|
| `clip_name`  | COMBO[STRING]   | Lista todos os arquivos de modelo suportados na pasta `HanzoStudio/models/clip_vision`. |

## Saídas

| Campo         | Tipo de Dados | Descrição |
|---------------|---------------|-----------|
| `clip_vision` | CLIP_VISION   | Modelo CLIP Vision carregado, pronto para codificar imagens ou outras tarefas relacionadas à visão computacional. |