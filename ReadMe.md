# Dummy Less CSS PHP

Projeto simples para leigos ou designers que não querem entender muito de como compilar esta coisa.


## Instalação
Basta baixar este repositorio ou clicar em Download e baixar tudo.


## Utilizado
- Primeiramente você precisará de um servidor local em php, tipo... XAMPP, WAMPP, EasyPHP
- Segundo, você precisa estar acostumado a rodar o servidor local, tipo... digitar no navegador http://localhost e funcionar
- depois é só ir na sua pasta onde se encontra o diretório css e colocar os arquivos deste projeto próximos á ela
- exemplo:
<pre>
    meu_projeto
        css
        less
            estilos.less
        javascript
        img
        index.html
        less.php
</pre>

## Transformando .less em .css

Se suas pastas estiverem parecidas com o exemplo acima, basta chamar http://localhost/meu_projeto/less.php e pronto! Ele irá buscar o estilos.less e transformar ele em <b>estilos.css</b> dentro da pasta css.

## Boas Práticas

Em seus arquivos <b>.less</b>, quando for utilizar o <b>@import</b> do <i>LessCSS</i>, utilize os nomes com o caracter <b>_</b> (underline) antes do nome. Ex.:
<pre>
    meu_projeto
        css
        less
            estilos.less
            _formularios.less
            _geral.less
</pre>
Desta forma, será criado somente um arquivo estilos.css os demais o compilador irá ignorar

## License
<pre>
This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.
</pre>