# Screenshot-Organizer

Este é um script Python que automatiza a criação de documentos do Word a partir de capturas de tela armazenadas em subpastas. O script classifica as capturas de tela por data de modificação e insere-as em documentos do Word individuais, um para cada subdiretório.

## Como o código funciona

O código consiste em várias etapas que são explicadas abaixo:

1. **Importação de Bibliotecas**: O código começa importando as bibliotecas Python necessárias para seu funcionamento. As bibliotecas incluem `os` para operações de sistema de arquivos, `docx` para criar documentos do Word, `PIL` para manipulação de imagens e `Image` para verificar se um arquivo é uma imagem.

2. **Definindo o Diretório Pai**: O script requer que você especifique o diretório pai que contém as subpastas com as capturas de tela. Isso é feito definindo a variável `parent_folder` com o caminho para o diretório pai.

3. **Iteração sobre Subdiretórios**: O código itera sobre os subdiretórios no diretório pai usando `os.listdir(parent_folder)`.

4. **Classificação de Capturas de Tela**: Para cada subdiretório, o código obtém uma lista de arquivos de captura de tela, classificando-os por data de modificação. Isso garante que as capturas de tela mais recentes sejam incluídas primeiro no documento.

5. **Criação de Documento do Word**: Um novo documento do Word é criado para cada subdiretório usando a biblioteca `docx`.

6. **Inserção de Capturas de Tela**: O código itera sobre os arquivos de captura de tela e insere cada um deles no documento do Word. As capturas de tela são verificadas para garantir que sejam imagens suportadas antes da inserção.

7. **Salvar o Documento do Word**: O documento do Word é salvo na mesma pasta do subdiretório de captura de tela com um nome baseado no nome do subdiretório.

## Melhorias Futuras

- Personalizar o script para adicionar suporte a outros formatos de imagem.
- Adicionar tratamento de erros para lidar com problemas que possam surgir durante a execução do script.
- Adicionar opções de linha de comando para permitir que o usuário especifique o diretório pai e outros parâmetros de forma interativa.

## Executando o Script

Para executar o script, basta copiá-lo para o diretório raiz que contém as subpastas com as capturas de tela e executá-lo a partir da linha de comando. Certifique-se de que as bibliotecas necessárias estejam instaladas antes de executar o script.

## Dependências

- Python 3.x
- Bibliotecas Python: `os`, `docx`, `PIL` (Pillow)

## Autor

[Anderson Almeida]

