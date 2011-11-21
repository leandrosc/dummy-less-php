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
Desta forma, será criado somente um arquivo estilos.css os demais o compilador irá ignorar. Ex.:
<i>estilos.less</i>
<pre>
body{
    p{
        text-align: left;
    }
}
@import "_formularios";
@import "_geral";

table{
.
.
.

</pre>

## Alterando o Dreameaver para aceitar extenssões .less

- Vá até a pasta onde você instalou seu Dreamweaver, ex: C:/Arquivos de programas/Adobe/Adobe Dreamweaver CS3/
- entre na pasta configuration/DocumentTypes
- abra o arquivo MMDocumentTypes.xml
- procure pelo trecho:
<pre>
&lt;documenttype id="CSS" internaltype="Text" winfileextension="css" macfileextension="css" file="Default.css" writebyteordermark="false"&gt;
        &lt;TITLE&gt;
                &lt;MMString:loadString id="mmdocumenttypes_30" /&gt;
        &lt;/TITLE&gt;
        &lt;description&gt;
                &lt;MMString:loadString id="mmdocumenttypes_31" /&gt;
        &lt;/description&gt;
&lt;/documenttype&gt;
</pre>
- inclua a extensão less juntamente com a extensão css, de forma que fique assim:
<pre>
&lt;documenttype id="CSS" internaltype="Text" <b>winfileextension="css,less" macfileextension="css,less"</b> file="Default.css" writebyteordermark="false"&gt;
        &lt;TITLE&gt;
                &lt;MMString:loadString id="mmdocumenttypes_30" /&gt;
        &lt;/TITLE&gt;
        &lt;description&gt;
                &lt;MMString:loadString id="mmdocumenttypes_31" /&gt;
        &lt;/description&gt;
&lt;/documenttype&gt;
</pre>

## License
<pre>
This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.
</pre>