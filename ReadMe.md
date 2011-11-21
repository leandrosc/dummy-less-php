# Dummy Less CSS PHP

Projeto simples para leigos ou designers que não querem entender muito de como compilar esta coisa.


## Instalação
Basta baixar este repositorio ou clicar em Download e baixar tudo.


## Utilizado
- Primeiramente você precisará de um servidor local em php, tipo... XAMPP, WAMPP, EasyPHP
- Segundo, você precisa estar acostumado a rodar o servidor local, tipo... digitar no navegador http://localhost e funcionar
- depois é só ir na sua pasta onde se encontra o diretório css e colocar os arquivos deste projeto próximos á ela
- exemplo:
    meu_projeto
        css
        less
            estilos.less
        javascript
        img
        index.html
        less.php

## Transformando .less em .css

Se suas pastas estiverem parecidas com o exemplo acima, basta chamar http://localhost/meu_projeto/less.php e pronto! Ele irá buscar o estilos.less e tranformar ele em estilos.css dentro da pasta css.

## Boas Práticas

Em seus arquivos .less, quando for utilizar o <b>@import</b> do LessCSS, utilize os nomes com o caracter '_' (underline) antes do nome. Ex.:
    meu_projeto
        css
        less
            estilos.less
            _formularios.less
            _geral.less

Desta forma, será criado somente um arquivo estilos.css os demais o compilador irá ignorar

## License
This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.
