# Seguidores-de-Jesus
# Seguidores de Jesus - Doutrina Espírita

Este é um projeto de página web (ainda em desenvolvimento) estática desenvolvido com **HTML** e **CSS**, que apresenta de forma clara e acessível os princípios da **Doutrina Espírita**, codificada por Allan Kardec. O objetivo é divulgar os fundamentos do Espiritismo e destacar suas obras principais com uma interface moderna e responsiva.

## Descrição

A página contém:

- Um **cabeçalho estilizado** com o nome do projeto;
- Um **menu de navegação** fixo com âncoras internas para facilitar o acesso ao conteúdo;
- Uma **seção de introdução** sobre o propósito da doutrina;
- Uma seção dedicada à **biografia de Allan Kardec**;
- Explicações didáticas sobre os **cinco pilares da Doutrina Espírita**;
- Um **catálogo visual** com as **cinco obras fundamentais** do Espiritismo;
- Um **rodapé institucional** com direitos autorais e propósito da página.

## Estilo Visual

O projeto utiliza **variáveis CSS** com uma paleta de cores suave e espiritualizada, com tons de:

- `--azul-celeste`: transmite paz e leveza;
- `--bege`: base neutra e acolhedora;
- `--cinza`: contraste sutil para elementos de navegação.

Além disso, a página conta com:

- **Imagem de fundo** com sobreposição translúcida para facilitar a leitura;
- **Cards interativos** para os livros, com efeito de "hover" (elevação);
- Layout **responsivo** para dispositivos móveis (media queries).

## Conteúdo

A estrutura HTML é organizada em seções:

- `<header>`: título principal;
- `<nav>`: menu de navegação;
- `<section>`: conteúdo dividido por temas (sobre, doutrina, obras);
- `<div class="book-card">`: estrutura para os cards de livros com imagem, título e descrição;
- `<footer>`: rodapé com direitos reservados.

## Responsividade

A responsividade foi trabalhada com `flex-wrap` e `@media (max-width: 768px)`, ajustando:

- Navegação para coluna vertical;
- Cards dos livros para uma única coluna.

## Funcionalidade Extra

O projeto inclui um **script em JavaScript** que ativa o **scroll suave** ao clicar nos links do menu:

```js
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
        e.preventDefault();
        document.querySelector(this.getAttribute('href')).scrollIntoView({
            behavior: 'smooth'
        });
    });
});

