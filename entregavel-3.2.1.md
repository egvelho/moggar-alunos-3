# Entregável 3.2

Observe o seguinte vetor de objetos de personagens de animes:

```js
const personagensAnime = [
  { nome: "Naruto", sobrenome: "Uzumaki", anime: "Naruto" },
  { nome: "Sasuke", sobrenome: "Uchiha", anime: "Naruto" },
  { nome: "Monkey D.", sobrenome: "Luffy", anime: "One Piece" },
  { nome: "Roronoa", sobrenome: "Zoro", anime: "One Piece" },
  { nome: "Son", sobrenome: "Goku", anime: "Dragon Ball" },
  { nome: "Vegeta", sobrenome: "Briefs", anime: "Dragon Ball" },
  { nome: "Light", sobrenome: "Yagami", anime: "Death Note" },
  { nome: "Lelouch", sobrenome: "Lamperouge", anime: "Code Geass" },
  { nome: "Izuku", sobrenome: "Midoriya", anime: "My Hero Academia" },
  { nome: "Katsuki", sobrenome: "Bakugo", anime: "My Hero Academia" },
  { nome: "Satoru", sobrenome: "Gojo", anime: "Jujutsu Kaisen" },
  { nome: "Yuji", sobrenome: "Itadori", anime: "Jujutsu Kaisen" },
  { nome: "Tanjiro", sobrenome: "Kamado", anime: "Demon Slayer" },
  { nome: "Nezuko", sobrenome: "Kamado", anime: "Demon Slayer" },
  { nome: "Eren", sobrenome: "Yeager", anime: "Attack on Titan" },
  { nome: "Mikasa", sobrenome: "Ackerman", anime: "Attack on Titan" },
  { nome: "Killua", sobrenome: "Zoldyck", anime: "Hunter x Hunter" },
  { nome: "Gon", sobrenome: "Freecss", anime: "Hunter x Hunter" },
  { nome: "Edward", sobrenome: "Elric", anime: "Fullmetal Alchemist" },
  { nome: "Roy", sobrenome: "Mustang", anime: "Fullmetal Alchemist" },
];
```

Além disso, imagine uma página HTML que contém o seguinte elemento:

```html
<ul id="personagens"></ul>
```

Agora, observe o seguinte código JS:

```js
const personagensUl = document.querySelector("#personagens");
const personagensList = personagensAnime.map(
  ({ nome, sobrenome, anime }) => `<li>${nome} ${sobrenome} (${anime})</li>`,
);
const personagensLi = personagensList.join("");

personagensUl.innerHTML = personagensLi;
```

Guarde essas informações...

Por seguinte, observe o seguinte vetor de objetos de animes:

```js
const animes = [
  {
    nome: "Naruto",
    ano: 2002,
    autor: "Masashi Kishimoto",
    imagem: "/animes/142503.jpg",
  },
  {
    nome: "One Piece",
    ano: 1999,
    autor: "Eiichiro Oda",
    imagem: "/animes/138851.jpg",
  },
  {
    nome: "Dragon Ball Z",
    ano: 1989,
    autor: "Akira Toriyama",
    imagem: "/animes/142022.jpg",
  },
  {
    nome: "Attack on Titan (Shingeki no Kyojin)",
    ano: 2013,
    autor: "Hajime Isayama",
    imagem: "/animes/47347.jpg",
  },
  {
    nome: "Death Note",
    ano: 2006,
    autor: "Tsugumi Ohba",
    imagem: "/animes/9453.jpg",
  },
  {
    nome: "Demon Slayer (Kimetsu no Yaiba)",
    ano: 2019,
    autor: "Koyoharu Gotouge",
    imagem: "/animes/99889.jpg",
  },
  {
    nome: "Fullmetal Alchemist: Brotherhood",
    ano: 2009,
    autor: "Hiromu Arakawa",
    imagem: "/animes/94745.jpg",
  },
  {
    nome: "Jujutsu Kaisen",
    ano: 2020,
    autor: "Gege Akutami",
    imagem: "/animes/109222.jpg",
  },
];
```

Assuma um HTML que contém os seguintes elementos:

```html
<div id="animes"></div>
<button id="fundo-aleatorio-btn">Trocar fundo aleatório</button>
```

Com o JS a seguir sendo aplicado:

```js
const animesDiv = document.querySelector("#animes");
const btnFundoAleatorio = document.querySelector("#fundo-aleatorio-btn");

const animesEls = animes.map(({ nome, ano, autor, imagem }) => {
  const animeEl = document.createElement("div");
  animeEl.className = "anime";
  animeEl.innerHTML = `<img src="${imagem}" width="100px"><span>${nome}</span>`;
  animeEl.onclick = () => alert(`${autor} criou ${nome} em ${ano}.`);
  return animeEl;
});

animesDiv.append(...animesEls);

function fundoAleatorioPAnimes() {
  const animesDivs = document.querySelectorAll(".anime");
  animesDivs.forEach((animeDiv) => {
    const randomRGB = `rgb(${Math.floor(Math.random() * 256)}, ${Math.floor(Math.random() * 256)}, ${Math.floor(Math.random() * 256)})`;
    animeDiv.style.backgroundColor = randomRGB;
  });
}

btnFundoAleatorio.onclick = fundoAleatorioPAnimes;
```
