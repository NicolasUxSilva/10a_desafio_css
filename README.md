# TechNews Today

Projeto de estudo em HTML5 + CSS3 para criar um portal de notícias com visual moderno, estrutura semântica e layout responsivo.

Este projeto foi desenvolvido com base no material visual do PPTX anexado, e tem como objetivo demonstrar como cada tag HTML faz parte da organização e do significado da página, além de mostrar como o CSS transforma essa estrutura em uma interface visual agradável.

## Objetivo do projeto

O desafio consiste em montar uma página de notícias tech com:

- cabeçalho com logo e slogan;
- destaque para uma notícia principal;
- bloco com vídeo incorporado;
- formulário de newsletter;
- rodapé com informações de contato;
- layout moderno em dark mode com elementos em gradiente e glassmorphism.

A ideia principal é entender a semântica do HTML, ou seja, não apenas “como a página fica”, mas também “qual é o significado do conteúdo” para acessibilidade, SEO e manutenção.

## Estrutura do projeto

O projeto está dividido em dois arquivos principais:

- `10a_desafio.html` — contém a marcação da página;
- `10a_desafio.css` — contém o estilo visual da interface.

## Visão geral da página

A página foi organizada com as principais áreas semânticas do HTML:

- `header`: área do topo com logo e slogan;
- `main`: conteúdo principal da página;
- `article`: notícia em destaque;
- `section`: blocos temáticos, como vídeo e newsletter;
- `footer`: rodapé com informações finais.

Essa divisão é importante porque deixa o código mais claro, mais acessível e mais fácil de manter.

## Trechos principais do código

O HTML do projeto usa várias tags semânticas e interativas para montar a estrutura do portal:

```html
<header class="cabecalho">
  <h1 class="logo">📱 TechNews Today</h1>
  <p class="tagline">As <strong>últimas novidades</strong> do mundo <em>tech</em></p>
</header>

<main class="conteudo">
  <article class="artigo-destaque">
    <h2>🚀 IA Revoluciona Desenvolvimento</h2>
    <time datetime="2025-08-07" class="data">7 de Agosto, 2025</time>
    <p>Inteligência artificial está transformando como criamos software...</p>
    <details class="leia-mais">
      <summary>Leia mais &rarr;</summary>
      <p>ChatGPT e outras ferramentas estão mudando o cenário tech mundial.</p>
    </details>
  </article>

  <section class="secao-video">
    <h3>📺 Tech em Vídeo</h3>
    <iframe
      class="video-embed"
      width="300"
      height="200"
      src="https://www.youtube.com/embed/eqUFcr1mI3Y"
      title="Tech News Video">
    </iframe>
  </section>

  <section class="secao-newsletter">
    <h3>📧 Newsletter</h3>
    <form action="subscribe.php" method="post" class="form-newsletter">
      <label for="email">Email:</label>
      <input type="email" id="email" name="email" required>

      <label for="interesse">Área de Interesse:</label>
      <select id="interesse" name="interesse">
        <option value="ia">Inteligência Artificial</option>
        <option value="mobile">Desenvolvimento Mobile</option>
        <option value="web">Tecnologias Web</option>
      </select>

      <div class="checkbox-container">
        <input type="checkbox" id="aceito" name="aceito" required>
        <label for="aceito">Aceito os termos</label>
      </div>

      <button type="submit" class="btn-inscrever">Inscrever-se</button>
    </form>
  </section>
</main>

<footer class="rodape">
  <p>&copy; 2025 TechNews Today &nbsp; Todos os direitos reservados</p>
  <address>Contato: <a href="mailto:info@technews.com">info@technews.com</a></address>
</footer>
```

## Tags e elementos utilizados

A página demonstra uma variedade de elementos HTML essenciais:

### Estrutura e semântica

- `<!DOCTYPE html>`: informa ao navegador que o documento é HTML5.
- `<html>`: raiz do documento.
- `<head>`: metadados da página.
- `<meta>`: configurações como charset e responsividade.
- `<title>`: título exibido na aba do navegador.
- `<link>`: ligação com o arquivo CSS.
- `<body>`: conteúdo visível da página.
- `<header>`, `<main>`, `<article>`, `<section>`, `<footer>`: blocos semânticos da página.

### Texto e apresentação

- `<h1>`, `<h2>`, `<h3>`: títulos e subtítulos.
- `<p>`: parágrafos.
- `<strong>`: destaque visual importante.
- `<em>`: ênfase em texto.
- `<time>`: data em formato legível para humanos e máquinas.
- `<address>`: informação de contato.

### Interação e mídia

- `<details>` e `<summary>`: bloco expansível, como o “Leia mais”.
- `<iframe>`: incorpora conteúdo externo, como o vídeo do YouTube.
- `<a href>`: links como e-mail ou navegação.

### Formulários

- `<form>`: agrupamento de campos do formulário.
- `<label>`: texto que identifica o campo.
- `<input>`: campos de entrada, como email, checkbox e botão.
- `<select>` e `<option>`: listas de seleção.
- `<button>`: ação de envio ou interação.

## Estilização em CSS

O CSS do projeto também foi pensado para refletir o visual moderno do portal tech.

### Principais recursos aplicados

- fundo escuro em tom azul/indigo;
- gradientes de cor para criar contraste e modernidade;
- cards com bordas translúcidas e efeito de glassmorphism;
- layout em grid para organização dos blocos;
- efeito hover em cards e botão de inscrição;
- responsividade para telas maiores, com ajuste de layout em desktop.

Exemplo de estilos importantes:

```css
body {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
  background: #0a0e27;
  color: #e4e4e7;
  line-height: 1.6;
}

.cabecalho {
  background: linear-gradient(135deg, rgba(99,102,241,0.1), rgba(219,39,119,0.1));
  backdrop-filter: blur(10px);
  border-bottom: 1px solid rgba(255,255,255,0.1);
  padding: 30px;
  text-align: center;
}

.logo {
  font-size: 36px;
  background: linear-gradient(90deg, #6366f1, #db2777);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.conteudo {
  display: grid;
  grid-template-columns: 1fr;
  gap: 30px;
  max-width: 800px;
  margin: 40px auto;
  padding: 0 20px;
}
```

## Importância do projeto

Este trabalho funciona como um exercício prático para aprender:

- HTML semântico;
- organização visual com CSS;
- estrutura de páginas de notícias;
- uso de formulários, mídia e conteúdo interativo;
- acessibilidade e manutenção de código.

O projeto também ilustra que, em desenvolvimento web, o HTML define o significado e a estrutura; o CSS define a aparência; e a combinação dos dois gera uma experiência melhor para o usuário.

## Como executar

Para visualizar o projeto:

1. Abra o arquivo `10a_desafio.html` em um navegador.
2. Ou use uma extensão como Live Server em um editor de código para abrir a página em ambiente local.

Como o projeto é estático, não há necessidade de instalação de dependências ou servidor complexo.

## Conclusão

O TechNews Today é um exemplo didático de como criar uma landing page de notícias com HTML5 e CSS3, combinando:

- organização semântica;
- conteúdo editorial;
- elementos interativos;
- layout moderno e responsivo.

É um excelente projeto para praticar fundamentos web e entender a lógica por trás de um portal de notícias funcional e visualmente atraente.
