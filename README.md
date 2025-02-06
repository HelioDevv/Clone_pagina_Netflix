# Netflix Clone

Este projeto é um clone da interface da Netflix, desenvolvido com **HTML**, **CSS** e **JavaScript**. O objetivo é aprimorar habilidades em **layout responsivo**, **carrossel de imagens** e **design moderno**.

## 🚀 Tecnologias Utilizadas

- **HTML5**: Estrutura do projeto.
- **CSS3**: Estilização e responsividade.
- **JavaScript**: Interatividade e lógica do carrossel.
- **[Owl Carousel](https://owlcarousel2.github.io/OwlCarousel2/)**: Biblioteca para criação do carrossel de filmes.
- **[FontAwesome](https://fontawesome.com/)**: Ícones utilizados nos botões.

## 📌 Funcionalidades

✔️ Interface semelhante à Netflix.<br>
✔️ Carrossel de filmes dinâmico.<br>
✔️ Responsividade para diversos dispositivos.<br>
✔️ Estilização moderna utilizando CSS.<br>
✔️ Botões interativos.

## 📁 Estrutura do Projeto

```bash
📦 netflix-clone
├── 📂 img                # Imagens do projeto
├── 📂 js                 # Scripts JavaScript
│   ├── jquery.min.js     # Biblioteca jQuery
│   ├── owl.carousel.min.js  # Biblioteca Owl Carousel
│   ├── setup.js          # Configuração do carrossel
├── 📂 style              # Arquivos de estilo
│   ├── main.css          # Estilos principais
│   ├── responsive.css    # Estilos responsivos
│   ├── owl.carousel.min.css  # Estilos do carrossel
│   ├── owl.theme.default.min.css # Tema do carrossel
├── index.html            # Página principal
└── README.md             # Documentação do projeto
```

## 📜 Código Principal

### 🔹 HTML
```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Netflix Clone</title>
    <link rel="stylesheet" href="style/main.css">
    <link rel="stylesheet" href="style/responsive.css">
    <link rel="stylesheet" href="style/owl/owl.carousel.min.css">
    <link rel="stylesheet" href="style/owl/owl.theme.default.min.css">
</head>
<body>
    <header>
        <div class="container">
            <h2 class="logo">NETFLIX</h2>
            <nav>
                <a href="#">Início</a>
                <a href="#">Séries</a>
                <a href="#">Filmes</a>
                <a href="#">Documentários</a>
            </nav>
        </div>
    </header>

    <main>
        <div class="filme-principal">
            <div class="container">
                <h3 class="titulo">ROUND 6</h3>
                <p class="descricao">Centenas de jogadores falidos aceitam um estranho convite para um jogo de sobrevivência...</p>
                <div class="botoes">
                    <button class="botao">
                        <i class="fa-solid fa-play"></i>
                        ASSISTIR AGORA
                    </button>
                    <button class="botao">
                        <i class="fa-solid fa-circle-info"></i>
                        MAIS INFORMAÇÕES
                    </button>
                </div>
            </div>
        </div>
    </main>

    <div class="carrosel-filmes">
        <div class="owl-carousel owl-theme">
            <div class="item"><img class="box-filme" src="img/mini1.jpg" alt=""></div>
            <div class="item"><img class="box-filme" src="img/mini2.jpg" alt=""></div>
        </div>
    </div>

    <script src="https://kit.fontawesome.com/dcd2795583.js" crossorigin="anonymous"></script>
    <script src="js/owl/jquery.min.js"></script>
    <script src="js/owl/owl.carousel.min.js"></script>
    <script src="js/owl/setup.js"></script>
</body>
</html>
```

### 🔹 JavaScript (Configuração do Carrossel)
```js
$('.owl-carousel').owlCarousel({
    loop: true,
    margin: 10,
    nav: false,
    responsive: {
        0: { items: 1 },
        600: { items: 3 },
        1000: { items: 5 }
    }
});
```

## 🎨 Estilização (CSS Principal)
```css
:root {
    --vermelho: #E50914;
    --preta: #141414;
}

body {
    background: var(--preta);
    color: white;
    font-family: 'Arial', sans-serif;
}

header .logo {
    color: var(--vermelho);
    font-size: 40px;
}

.filme-principal {
    background: linear-gradient(rgba(0,0,0,.50), rgba(0,0,0,.50)), url('/img/round-6-imag-fundo.jpg');
    background-size: cover;
}
```

## 🔗 Links e Recursos

- [Owl Carousel](https://owlcarousel2.github.io/OwlCarousel2/) - Biblioteca utilizada para o carrossel.
- [FontAwesome](https://fontawesome.com/) - Ícones utilizados no projeto.
- [Documentação Oficial do jQuery](https://jquery.com/) - Biblioteca JavaScript utilizada.

## 📌 Como Executar o Projeto

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/seu-usuario/netflix-clone.git
   ```
2. **Abra o arquivo `index.html` no navegador.**
3. **Para modificar, edite os arquivos CSS e JS conforme necessário.**

## 📜 Licença

Este projeto foi desenvolvido apenas para fins educacionais e não tem qualquer vínculo com a Netflix. Use livremente para aprendizado!

---

Feito com ❤️ por Hélio Junior 🚀
