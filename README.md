# Página de destino do Huddle com uma única seção introdutória


Esta é uma solução para o [desafio da página de destino com uma única seção do Huddle no Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0/hub). Os desafios do Frontend Mentor ajudam você a melhorar suas habilidades de codificação através da construção de projetos realistas. 

## Índice

- [Overview](#overview)
  - [O desafio](#o-desafio)
  - [Print do projeto](#print-do-projeto)
  - [Link](#link)
- [Meu processo](#meu-processo)
  - [Construído com](#construido-com)
  - [O que aprendi](#o-que-aprendi)
  - [Desenvolvimento contínuo](#desenvolviment-continuo)
- [Autora](#autora)
- [Agradecimentos](#agradecimentos)

## Overview

### O desafio

O desafio constiste em:

- testar nossos conhecimentos com front-end, mas expecificadamente o CSS, na parte de flexbox;
- mostrar nossa capacidade em utilizar as propriedades relacionadas ao flex e seus atributos;
- mostrar nossos conhecimento em mobile;

### Print do projeto

![](./src/images/print.png) 

### Link

- Código do desenvolvimento: [Huddle](https://github.com/maiarasteffen/quest-desafio)
- Front do projeto: [Front](https://joyful-brigadeiros-7572ca.netlify.app/)

## Meu processo

### Construído com

- Semântica HTML;
- Propriedades CSS;
- Flexbox;
- Positions;
- Variáveis no CSS;
- Media querie;

### O que aprendi

Aprendi como utilizar e centralizar os elementos como flexbox, propriedades mais usadas foram: display, justify-content e align-itens; além de aprender sobre responsividade.

Código utilizado:

```html
<body>
  <header>
    <div class="logo">
      <img src="./src/images/logo.svg" alt="logo">
    </div>
  </header>
  <section class="section">
    <div class="image">
      <img src="./src/images/illustration-mockups.svg" alt="Mockups">
    </div>
    <div class="info">
      <h3>Build The Community Your Fans Will Love</h3>
      <p>Huddle re-imagines the way we build communities. You have a voice, but so does your audience. 
        Create connections with your users as you engage in genuine discussion.</p>
      <button>Register</button>
    </div>
  </section>

  <footer class="social">
    <span><i class="fa fa-facebook"></i></span>
    <span><i class="fa fa-twitter"></i></span>
    <span><i class="fa fa-instagram"></i></span>
  </footer>
  <!-- FONT AWESOME -->
  <script src="https://kit.fontawesome.com/3212825096.js" crossorigin="anonymous"></script>
</body>
```
```css
body {
    min-height: 100vh;
    background: url('../images/bg-desktop.svg');
    background-color: var(--violet-color);
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    font-family: var(--font-body);
    color: #fff;
}

.logo {
    display: flex;
    align-items: center;
    padding: 0 50px 0 50px ;
}

.logo img {
    max-width:220px;
    max-height:150px;
}

.section {
    display: flex;
}

.section .image {
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 50px;
}

.section .info {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    height: 100%;
    width: 100%;
}

.section .info h3 {
    font-size: 4rem;
    font-weight: 600;
    max-width: 560px;
    font-family: var(--font-headings);
    margin-top: 20%;
}

.section .info p {
    font-size: 1.8rem;
    max-width: 520px;
    line-height: 25px;
    margin: 25px 0;
}

.section .info button {
    background-color: #fff;
    border: none;
    padding: 15px 65px;
    border-radius: 50px;
    font-size: 1.8rem;
    font-family: var(--font-headings);
    color: var(--violet-color);
    margin-top: 5px;
    cursor: pointer;
    transition: 0.3s;
}

.section .info button:hover {
    background-color: var(--soft-magenta-color);
    color: #fff;
    box-shadow: 5px 5px 15px 5px rgba(3, 3, 3, 0.2);
}

.social {
    display: flex;
    align-items: center;
    justify-content: flex-end;
    padding: 15px;
}

.social span {
    width: 40px;
    height: 40px;
    display: grid;
    margin: 0 10px;
    place-items: center;
    border: 1px solid #fff;
    border-radius: 50%;
    cursor: pointer;
}

.social span:hover {
    color: var(--soft-magenta-color);
    border-color: var(--soft-magenta-color);
}

.social span i {
    font-size: 15px;
}

@media (max-width: 375px) {
    body {
        background: url('../images/bg-desktop.svg');
        background-color: var(--violet-color);
        background-position: center;
        background-size: cover;
        background-repeat: no-repeat;
    }
    
    .section {
        flex-direction: column;
        height:80%;
        width: 375px;
    }

    .section .image {
        margin: 20px;
    }

    .section .image img {
        height: 100%;
        width: 100%;
    }

    .section .info {
        align-items: center;
        text-align: center;
    }

    .section .info h3 {
        font-size: 2.5rem;
        margin: auto;
    }

    .section .info p {
        font-size: 1.5rem;
        width: 300px;
    }

    .social {
        justify-content: center;
        margin-top: 25px;
    }   
}
```

### Desenvolvimento contínuo

Irei continuar me aperfeiçoando na parte de CSS, focando no Flexbox e Grid. Além de estilizar elementos com pseudo-elementos. Também daqui em diante irei me aperfeiçoar na área de React Native e Rest API com Node.js! Por isso estou treinando bem a base do Front-end!

## Author

- Linkedin - [Maiara Steffen](https://www.linkedin.com/in/maiara-steffen/)
- Frontend Mentor - [@maiarasteffen](https://www.frontendmentor.io/profile/maiarasteffen)
- Instagram - [@maiara_steffen](https://www.instagram.com/maiara_steffen/)
- GitHub - [@maiarasteffen](https://github.com/maiarasteffen/)

## Agradecimentos

Primeiro quero agradecer muito a Deus por sempre estar me dando oportunidades de me desenvolver cada vez mais na carreira de programadora, também quero agradecer muito ao [Dev Em Dobro](https://www.instagram.com/devemdobro/), os irmãos que me ensinam muitas pessoas a se desenvolverem e crescerem no mercado de trabalho como programador!
