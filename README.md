# 🙏 Projeto Site — Frei Gilson

Este projeto foi desenvolvido como **projeto final do curso de Git e GitHub**, realizado na plataforma **Curso em Vídeo**, com o professor **Gustavo Guanabara**.

Como atividade final, o desafio proposto foi desenvolver um pequeno site utilizando **HTML e CSS**, versionar o projeto com Git e publicá-lo utilizando o **GitHub Pages**, aproveitando o domínio gratuito disponibilizado pela plataforma.

Para colocar o conhecimento em prática, escolhi desenvolver um site sobre o **Frei Gilson**, apresentando um pouco de sua história, suas principais músicas e o destaque de suas transmissões durante a Quaresma.

## 🌐 Projeto publicado

🔗 **Acesse o site:**
https://victor-aandrade.github.io/projeto-site/

## 📖 Sobre o projeto

O objetivo do site é apresentar informações sobre Frei Gilson de maneira simples e organizada, utilizando os conhecimentos adquiridos durante o curso.

O projeto possui páginas com:

* 📌 Informações sobre Frei Gilson;
* 🎵 Principais músicas;
* 🙏 Conteúdos relacionados à Quaresma;
* ▶️ Links e vídeos direcionando para o YouTube;
* 🔙 Navegação entre as páginas;
* 📱 Adaptação para dispositivos móveis.

## 🛠️ Tecnologias utilizadas

* **HTML5** — estruturação das páginas;
* **CSS3** — estilização, organização e responsividade;
* **Git** — controle de versão;
* **GitHub** — armazenamento e gerenciamento do código;
* **GitHub Pages** — hospedagem gratuita do site.

## 📁 Estrutura do projeto

```text
projeto-site/
│
├── index.html
├── musicas.html
├── quarentena.html
│
├── estilos/
│   └── style.css
│
└── imagens/
    ├── Frei-Gilson 1.png
    ├── cover-do-frei-gilson 2.png
    ├── imagemchurchpo 3.png
    └── voltar.png
```

## 💻 Desenvolvimento

Durante o desenvolvimento, coloquei em prática conceitos estudados no curso, principalmente a criação de páginas HTML, utilização de links, imagens, organização de arquivos, estilização com CSS e publicação através do GitHub Pages.

Também trabalhei com recursos como:

* `header`, `main`, `article` e `footer`;
* links internos entre páginas;
* imagens com `alt`;
* incorporação de vídeos do YouTube utilizando `iframe`;
* classes CSS;
* `float`;
* `margin` e `padding`;
* `max-width`;
* `@media queries`;
* `aspect-ratio`;
* design responsivo.

## 🚧 Dificuldades encontradas

Durante o desenvolvimento, algumas dificuldades apareceram e fizeram parte importante do processo de aprendizagem.

### 1. Imagens não apareciam corretamente

No início, algumas imagens não eram carregadas corretamente.

A solução foi verificar a organização das pastas e conferir se os caminhos utilizados no atributo `src` correspondiam exatamente à localização e ao nome dos arquivos.

Exemplo:

```html
<img src="imagens/cover-do-frei-gilson 2.png">
```

### 2. Imagens não ficavam ao lado do texto

Outra dificuldade foi posicionar as imagens ao lado dos textos.

Para solucionar o problema, utilizei CSS com `float`:

```css
.imagem-lado {
    float: right;
    width: 300px;
    max-width: 40%;
    height: auto;
    margin-left: 25px;
}
```

Isso permitiu que o texto ocupasse o espaço ao redor da imagem.

### 3. O CSS não estava sendo carregado

Esse foi um dos problemas que mais me ajudou a entender a importância da organização dos arquivos.

Meu arquivo `style.css` estava dentro da pasta `estilos`, mas inicialmente o HTML procurava o arquivo na pasta principal.

O problema foi resolvido alterando:

```html
<link rel="stylesheet" href="style.css">
```

para:

```html
<link rel="stylesheet" href="estilos/style.css">
```

### 4. Vídeo do YouTube não se adaptava ao celular

O `iframe` do YouTube funcionava corretamente no computador, mas ultrapassava a largura da tela em dispositivos móveis.

A solução foi criar um container responsivo:

```css
.video {
    width: 100%;
    max-width: 800px;
    margin: 30px auto;
    aspect-ratio: 16 / 9;
}

.video iframe {
    width: 100%;
    height: 100%;
}
```

Dessa maneira, o vídeo mantém a proporção 16:9 e se adapta automaticamente ao tamanho da tela.

## 📱 Responsividade

Um dos objetivos durante os ajustes finais foi fazer com que o site funcionasse não apenas no computador, mas também em celulares.

Para isso, utilizei `@media queries`:

```css
@media (max-width: 600px) {
    body {
        padding: 10px;
    }

    .imagem-lado {
        float: none;
        display: block;
        width: 90%;
        margin: 15px auto;
    }
}
```

Assim, elementos que funcionavam lado a lado no computador passam a ser organizados verticalmente em telas menores.

## 🚀 Publicação com GitHub Pages

Depois de finalizar o desenvolvimento, utilizei o Git e o GitHub para versionar e armazenar o projeto.

Por fim, utilizei o **GitHub Pages** para disponibilizar o site publicamente na internet, utilizando o domínio gratuito:

**victor-aandrade.github.io/projeto-site/**

Esse processo foi especialmente importante porque permitiu colocar em prática não apenas a criação do site, mas também o fluxo de publicação de um projeto web utilizando Git e GitHub.

## 📚 Curso

Este projeto foi desenvolvido como atividade final do curso de **Git e GitHub** do **Curso em Vídeo**, ministrado pelo professor **Gustavo Guanabara**.

O curso foi fundamental para compreender conceitos relacionados a:

* Git;
* GitHub;
* repositórios;
* commits;
* versionamento;
* publicação de projetos;
* GitHub Pages.

## 🎯 O que aprendi

Mais do que simplesmente criar uma página HTML, este projeto me ajudou a entender que desenvolver um site envolve várias etapas.

Aprendi a organizar melhor meus arquivos, solucionar problemas de caminhos, utilizar CSS para posicionamento e responsividade, incorporar conteúdos externos e, principalmente, utilizar Git e GitHub para versionar e publicar um projeto.

Também percebi a importância de testar o projeto em diferentes tamanhos de tela e de buscar soluções para os problemas que surgem durante o desenvolvimento.

## 🔮 Próximos passos

Este projeto representa uma das primeiras etapas da minha jornada na área de tecnologia.

Pretendo continuar aprimorando meus conhecimentos em:

* HTML e CSS;
* JavaScript;
* Python;
* Git e GitHub;
* desenvolvimento web;
* responsividade e acessibilidade.

A ideia é continuar evoluindo este projeto e utilizar os conhecimentos adquiridos para desenvolver projetos cada vez mais completos.

---

### 👨‍💻 Autor

**Victor Andrade**

Estudante de **Análise e Desenvolvimento de Sistemas**.

📌 Este projeto foi desenvolvido para fins educacionais como conclusão do curso de Git e GitHub do Curso em Vídeo.
