# Aprendendo [Front-End](https://developer.mozilla.org/pt-BR/docs/Learn/Getting_started_with_the_web) - mdn web docs - Mozilla Developer Network

## Iniciando com HTML

> HTML (Linguagem de Marcação de Hipertexto) é o código que você usa para estruturar uma página web e seu conteúdo.<br><br>
> HTML não é uma linguagem de programação; é uma linguagem de marcação, usada para definir a estrutura do seu conteúdo.<br><br>
> HTML consiste de uma série de `elementos`, que você usa para delimitar ou agrupar diferentes partes do conteúdo para que ele apareça ou atue de determinada maneira. As tags anexas podem transformar uma palavra ou imagem num hiperlink, pode colocar palavras em itálico, pode aumentar ou diminuir a fonte e assim por diante.

### Anatomia de um elemento HTML
![elemento html explicado: tag de abertura, conteúdo, tag de fechamento](https://developer.mozilla.org/pt-BR/docs/Learn/Getting_started_with_the_web/HTML_basics/gato-rabujento-pequeno.png)

1. `A tag de abertura`: Consiste no nome do elemento (no caso, p), envolvido em parênteses angulares de abertura e fechamento. Isso demonstra onde o elemento começa, ou onde seu efeito se inicia — nesse caso, onde é o começo do parágrafo.
2. `A tag de fechamento`: Isso é a mesma coisa que a tag de abertura, exceto que inclui uma barra antes do nome do elemento. Isso demonstra onde o elemento acaba — nesse caso, onde é o fim do parágrafo. Esquecer de incluir uma tag de fechamento é um dos erros mais comuns de iniciantes e pode levar a resultados estranhos.
3. `O conteúdo`: Esse é o conteúdo do elemento, que nesse caso é apenas texto.
4. `O elemento`: A tag de abertura, a de fechamento, e o conteúdo formam o elemento.

### Atributos
Elementos também podem ter atributos, que parecem assim:

![](https://developer.mozilla.org/pt-BR/docs/Learn/Getting_started_with_the_web/HTML_basics/gato-rabujento-atributo-pequeno.png)

Atributos contém informação extra sobre o elemento que você não quer que apareça no conteúdo real. Aqui, class é o nome do atributo e editor-note é o valor do atributo. O atributo class permite que você forneça ao elemento um identificador que possa ser usado posteriormente para aplicar ao elemento informações de estilo e outras coisas.

Um atributo sempre deve ter:

1. Um espaço entre ele e o nome do elemento (ou o atributo anterior, se o elemento já tiver um).
2. O nome do atributo, seguido por um sinal de igual.
3. Aspas de abertura e fechamento, envolvendo todo o valor do atributo.

### Elementos vazios - sem tag de fechamento </>
Alguns elementos não possuem conteúdo e são chamados de elementos vazios. Considere o elemento `<img>` que temos na nossa página HTML:

`<img src="imagens/firefox-icon.png" alt="Minha imagem de teste" />`

Ele contém dois atributos, mas não há tag `</img>` de fechamento, e não há conteúdo interno. Isso acontece porque um elemento de imagem não envolve conteúdo para ter efeito em si mesmo. Sua proposta é incorporar uma imagem na página HTML no lugar que o código aparece.


### Principais elementos de um documento HTML

`<!DOCTYPE html>` — o doctype. É a parte inicial obrigatória do documento. Sinaliza que esse arquivo deve ser entendido como um documento HTML 5.

`<html></html>` — o elemento `<html>`. Esse elemento envolve todo o conteúdo da página e às vezes é conhecido como o elemento raiz.

`<head></head>` — o elemento `<head>` (cabeçalho). O conteúdo do `<head>` não aparece no site. Aqui vão os "metadados" do arquivo - informações do arquivo, como a declaração do conjunto de caracteres (charset) que o navegador deve entender, palavras-chave, descrição que você quer que apareça nos resultados de buscas, link do arquivo CSS, scrips em JS que serão incorporados no site.

`<meta charset="utf-8">` — esse elemento define o conjunto de caracteres que seu documento deve usar para o UTF-8, que inclui praticamente todos os caracteres da grande maioria dos idiomas escritos. Essencialmente, agora ele pode manipular qualquer conteúdo textual que você possa colocar.

`<title></title>` — o elemento `<title>.` Ele define o título da sua página, que é o título que aparece na guia do navegador onde sua página é carregada. Ele também é usado para descrever a página quando você a adiciona aos favoritos.

`<body></body>` — o elemento `<body>`. Contém todo o conteúdo que você quer mostrar ao público que visita sua página, seja texto, imagens, vídeos, jogos, faixas de áudio reproduzíveis ou qualquer outra coisa.

`<!--  -->` - comentário HTML