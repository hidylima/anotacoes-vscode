# anotacoes-vscode

## Emmet
- Já vem instalado

## Abrindo o VsCode no terminal 
- `code` abre o editor
- `code .` abre o diretório atual

## Abrindo um diretório de projeto
- `ctrl + k + o`

## Invocar Intellisense
- `ctrl + space` 

## Reposicionando a visualização vertical da linha, mantendo o cursor no mesmo local 
- `ctrl + up/down arrow` 

## Copiando uma linha inteira sem copy e paste 
- `shift + alt + up/down arrow`

## Movendo uma linha inteira ou uma seleção de linhas para cima ou para baixo 
- `alt + up/down arrow`

## Deletando uma linha inteira sem selecioná-la 
- `ctrl + shift + k`

## Comentando uma linha inteira 
- `ctrl + ;`

## Quick open - Abrindo um arquivo sem precisar procurá-lo na sidebar (explorer)
- `ctrl + p` e nome do arquivo 

## Vizualizar todos os atalhos do editor 
- `ctrl + k + s`

## Visualizar explorer dos arquivos 
- `ctrl + shift + e`

## Recolher menu lateral 
- `ctrl + b`

## Integrated command line
- `ctrl + '` abre o terminal
- Abre a linha de comando diretamente na pasta do projeto 

## Command Palette
- `ctrl + shift + p`
- Aumenta a produtividade 
- Permite fazer qualquer coisa no Vscode 
- `reindent` - conserta a indentação das linhas selecionadas
- `change lang` - muda a linguagem do arquivo 

## Visualizando todos os métodos, classes e propriedades de um arquivo JS
- `@`, no quick open (ctrl + p) 

## Peek Definition - Visualizando um módulo importado 
- No arquivo que importa o módulo, selecionar no nome do módulo, clicar  
com o botão direito e escolher 'Peek Definition' 

## Editando com múltiplos cursores 
- `ctrl + shift + alt + up/down arrow`

## Selecionando todas as ocorrências de uma string 
- `ctrl + shift + L` com uma string selecionada **ou com o cursor**.  
Todas as strings similares no documento serão selecionadas 

## Visualizando o elemento HTML de um seletor CSS 
- Basta posicionar o cursor do mouse sobre o seletor (hover) 

## Formatando automaticamente um documento inteiro 
- `shift + alt + f`

## Formatando automaticamente um texto ou linhas selecionadas 
- `ctrl + k + f`

## Code Folding 
- `ctrl + shift + ´` colapsa  sessão do cursor 
- `ctrl + shift + [` descolapsa  sessão do cursor 
- `ctrl + k + 0` colapsa todas as sessões
- `ctrl + k + j` descolapsa todas as sessões
- `ctrl + k + [number]` colapsa o nível de sessões do código  
através do number especificado 

## Renomeando nomes de links, variáveis, funções ou métodos 
- `f2` com o cursor no nome. Isso irá renomear todas as  
instâncias e referências nos documentos do projeto. 

## Visualizar menu de extensões 
- `ctrl + shift + x`

## Instalando snippets e outras extensões 
- Com o menu de extensões aberto, digitar o nome da linguagem  
ou/e extensão 
- Intellisense reconhece snippets instalados

## Snippets 

### VsCode snippets
- Começar a digitar o comando e selecioná-lo, com up/down arrow 
- `tab` navega entre os parâmetros 

### JavaScript (ES6) code snippets

#### Funções 
- `anfn` função anônima
- `nfn` função nomeada (atribuída a uma const)
- `prom` cria uma nova promise sendo retornada 
- `thenc` cria um .then e .catch
- `clg` console.log()

### User-defined snippets 
- `ctrl + shift + p + 'snippets' + 'lang. name'` Abre o painel de  
definições de snippets do usuário 

#### My Custom JavaScript Snippets 
- `c + tab` declara uma const
- `L + tab` declara uma let