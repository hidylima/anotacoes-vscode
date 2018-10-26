# anotacoes-vscode

## [Integrando cmder como terminal do vscode](https://code.visualstudio.com/docs/editor/integrated-terminal#_can-i-use-cmders-shell-with-the-terminal-on-windows)
```javascript
 // settings.json
{
  // ...
  "terminal.integrated.shell.windows": "C:\\WINDOWS\\System32\\cmd.exe",
  "terminal.integrated.shellArgs.windows": ["/K", "C:\\Users\\roger\\cmder\\vscode.bat"]
}
```

## Abas do terminal
- Abrir uma 2ª aba no terminal: `ctrl + ]`
- alternar entre abas: `alt + left / right`

## [Emmet](https://docs.emmet.io/abbreviations/syntax/)
- Já vem instalado
- É possível habilitá-lo em 'settings > emmet.triggerExpansionOnTab' 

### HTML Emmet Expressions 
- `>` - filho
- `+` - irmão
- `^` - volta um nível acima
- `.` - classe
  - `.nomeDaClasse` declarauma `div`, por padrão
  - Pode haver mais de uma por elemento
  - Pode ser declarado com id's
- `#` - id
  - `#nomeDoId` declara uma `div`, por padrão
  - Pode haver mais de um por elemento
  - Pode ser declarado com classes 
- `[attr1="" attr2=""]` declara atributo(s) ao elemento
- `{text}` insere texto no elemento

Exemplo voltando dois níveis acima - `div>p>span+em^^bq`:

```html
<div>
  <p><span></span><em></em></p>
</div>
<blockquote></blockquote>
```

- `bq` - blockquote 
- `()` - agrupamento 
  - Permite escrever duas tags irmãs que possuem muitos 
  filhos 
  - Evita, por exemplo, o uso da volta para o nível 
  duas vezes

Exemplo de agrupamento - `div>(header>nav>li*3)+footer+p`: 

```html
<div>
  <header>
    <nav>
      <li></li>
      <li></li>
      <li></li>
    </nav>
  </header>
  <footer></footer>
  <p></p>
</div>
```

Exemplo de agrupamentos aninhados - `div>(header>nav>(li+div)*3)+footer+p`: 

```html
<div>
  <header>
    <nav>
      <li></li>
      <div></div>
      <li></li>
      <div></div>
      <li></li>
      <div></div>
    </nav>
  </header>
  <footer></footer>
  <p></p>
</div>
```

- `*` multiplica o elemento  quantas vezes forem especificadas
- `$` numera nomes de atributos de elementos multiplicados 
  - Múltiplos `$` inserem `0` antes do número 
  - `@3` após o cifrão declara à partir do número especificado 
  - `@-` após o cifrão declara os números em ordem decrescente 

Exemplos de atributos numerados - `ul>li.item-menu.item-$*5`:

```html
<ul>
    <li class="item-menu item-1"></li>
    <li class="item-menu item-2"></li>
    <li class="item-menu item-3"></li>
    <li class="item-menu item-4"></li>
    <li class="item-menu item-5"></li>
  </ul>
```

### CSS Emmet Expressions 

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
- `anfn` arrow function anônima
- `nfn` arrow function nomeada (atribuída a uma const)
- `prom` cria uma nova promise sendo retornada 
- `thenc` cria um .then e .catch
- `clg` console.log()

### User-defined snippets 
- `ctrl + shift + p + 'snippets' + 'lang. name'` Abre o painel de  
definições de snippets do usuário 

#### My Custom JavaScript Snippets 
- `nafun + tab` declara uma arrow function nomeada (atribuída à uma  
const) 
- `afun + tab` declara uma arrow function anônima 
- `fun + tab` declara uma ES5 function 
- `r + tab` declara um `return` 
- `c + tab` declara uma const
- `L + tab` declara uma let
- `ts + tab` declara uma template string 
- `log + tab` declara um console.log()
- `bc + tab` declara um bloco de código 

#### My Custom Markdown Snippets 
- **Para que o comando funcione, é necessário que o gatilho  
com o snippet seja mostrado e selecionado antes, com `ctrl + space`**
- `jsc + ctrl + space + tab` declara um bloco de código javascript
- `hc + ctrl + space + tab` declara um bloco de código HTML 
- `cc + ctrl + space + tab` declara um bloco de código CSS 
- `ic + space + tab` declara um código inline 
- `h1c + ctrl + space + tab` declara um bloco h1 com código no início 
- `h2c + ctrl + space + tab` declara um bloco h2 com código no início 
