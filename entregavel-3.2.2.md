Agora, vamos ao entregável!

Assuma o seguinte vetor de objetos de gatos:

```js
const catCatalog = [
  {
    raca: "Persa",
    origem: "Irã",
    anoReconhecimento: 1871,
    soltaPelo: true,
    temperamento: "Calmo, afetuoso e silencioso",
    imagem: "/gatos/persian.jpg",
  },
  {
    raca: "Siamês",
    origem: "Tailândia",
    anoReconhecimento: 1878,
    soltaPelo: true,
    temperamento: "Brincalhão, vocal e inteligente",
    imagem: "/gatos/siamese.jpg",
  },
  {
    raca: "Maine Coon",
    origem: "Estados Unidos",
    anoReconhecimento: 1976,
    soltaPelo: true,
    temperamento: "Gentil, amigável e gigante",
    imagem: "/gatos/maine_coon.jpg",
  },
  {
    raca: "Sphynx",
    origem: "Canadá",
    anoReconhecimento: 2005,
    soltaPelo: false,
    temperamento: "Extrovertido, enérgico e apegado",
    imagem: "/gatos/sphynx.jpg",
  },
  {
    raca: "Bengal",
    origem: "Estados Unidos",
    anoReconhecimento: 1983,
    soltaPelo: true,
    temperamento: "Ativo, curioso e independente",
    imagem: "/gatos/bengal.jpg",
  },
  {
    raca: "Ragdoll",
    origem: "Estados Unidos",
    anoReconhecimento: 1960,
    soltaPelo: true,
    temperamento: "Dócil, tranquilo e carinhoso",
    imagem: "/gatos/ragdoll.jpg",
  },
  {
    raca: "British Shorthair",
    origem: "Reino Unido",
    anoReconhecimento: 1870,
    soltaPelo: true,
    temperamento: "Sossegado, leal e paciente",
    imagem: "/gatos/british_shorthair.jpg",
  },
  {
    raca: "Scottish Fold",
    origem: "Escócia",
    anoReconhecimento: 1966,
    soltaPelo: true,
    temperamento: "Amoroso, companheiro e adaptável",
    imagem: "/gatos/scottish_fold.jpg",
  },
  {
    raca: "American Curl",
    origem: "Estados Unidos",
    anoReconhecimento: 1986,
    soltaPelo: true,
    temperamento: "Orelhas curvadas, interativo e alegre",
    imagem: "/gatos/american_curl.jpg",
  },
  {
    raca: "Exótico",
    origem: "Estados Unidos",
    anoReconhecimento: 1966,
    soltaPelo: true,
    temperamento: "Preguiçoso, brincalhão e afetuoso",
    imagem: "/gatos/exotic_shorthair.jpg",
  },
  {
    raca: "Munchkin",
    origem: "Estados Unidos",
    anoReconhecimento: 2003,
    soltaPelo: true,
    temperamento: "Pernas curtas, veloz e muito dócil",
    imagem: "/gatos/munchkin.jpg",
  },
  {
    raca: "Devon Rex",
    origem: "Reino Unido",
    anoReconhecimento: 1979,
    soltaPelo: false,
    temperamento: "Travesso, palhaço e apegado",
    imagem: "/gatos/devon_rex.jpg",
  },
  {
    raca: "Abissínio",
    origem: "Etiópia",
    anoReconhecimento: 1882,
    soltaPelo: true,
    temperamento: "Super ativo, atlético e expressivo",
    imagem: "/gatos/abyssinian.jpg",
  },
  {
    raca: "Ocicat",
    origem: "Estados Unidos",
    anoReconhecimento: 1987,
    soltaPelo: true,
    temperamento: "Aparência selvagem, sociável e treinável",
    imagem: "/gatos/ocicat.jpg",
  },
  {
    raca: "Egyptian Mau",
    origem: "Egito",
    anoReconhecimento: 1956,
    soltaPelo: true,
    temperamento: "Rápido, leal e independente",
    imagem: "/gatos/egyptian_mau.jpg",
  },
  {
    raca: "Savannah",
    origem: "Estados Unidos",
    anoReconhecimento: 2001,
    soltaPelo: true,
    temperamento: "Extremamente alto, ativo e inteligente",
    imagem: "/gatos/savannah.jpg",
  },
  {
    raca: "Toyger",
    origem: "Estados Unidos",
    anoReconhecimento: 2007,
    soltaPelo: true,
    temperamento: "Parece um tigre, amigável e focado",
    imagem: "/gatos/toyger.jpg",
  },
  {
    raca: "Burmese",
    origem: "Mianmar",
    anoReconhecimento: 1936,
    soltaPelo: true,
    temperamento: "Sociável, brincalhão e confiante",
    imagem: "/gatos/burmese.jpg",
  },
  {
    raca: "Birmanês",
    origem: "França",
    anoReconhecimento: 1925,
    soltaPelo: true,
    temperamento: "Doce, gentil e curioso",
    imagem: "/gatos/birman.jpg",
  },
  {
    raca: "Singapura",
    origem: "Singapura",
    anoReconhecimento: 1982,
    soltaPelo: true,
    temperamento: "Pequeno, curioso e muito ativo",
    imagem: "/gatos/singapura.jpg",
  },
  {
    raca: "Korat",
    origem: "Tailândia",
    anoReconhecimento: 1965,
    soltaPelo: true,
    temperamento: "Observador, apegado ao dono e calmo",
    imagem: "/gatos/korat.jpg",
  },
  {
    raca: "Bobtail Japonês",
    origem: "Japão",
    anoReconhecimento: 1976,
    soltaPelo: true,
    temperamento: "Rabo curto, expressivo e ativo",
    imagem: "/gatos/japanese_bobtail.jpg",
  },
  {
    raca: "Russian Blue",
    origem: "Rússia",
    anoReconhecimento: 1912,
    soltaPelo: true,
    temperamento: "Tímido, inteligente e reservado",
    imagem: "/gatos/russian_blue.jpg",
  },
  {
    raca: "Norueguês da Floresta",
    origem: "Noruega",
    anoReconhecimento: 1977,
    soltaPelo: true,
    temperamento: "Independente, amigável e robusto",
    imagem: "/gatos/norwegian_forest_cat.jpg",
  },
  {
    raca: "Chartreux",
    origem: "França",
    anoReconhecimento: 1928,
    soltaPelo: true,
    temperamento: "Gentil, silencioso e excelente caçador",
    imagem: "/gatos/chartreux.jpg",
  },
  {
    raca: "Siberiano",
    origem: "Rússia",
    anoReconhecimento: 1990,
    soltaPelo: true,
    temperamento: "Pelagem tripla, brincalhão e hipoalergênico",
    imagem: "/gatos/siberian.jpg",
  },
  {
    raca: "Bombaim",
    origem: "Estados Unidos",
    anoReconhecimento: 1970,
    soltaPelo: true,
    temperamento: "Alerta, amigável e miado baixo",
    imagem: "/gatos/bombay.jpg",
  },
  {
    raca: "Manx",
    origem: "Ilha de Man",
    anoReconhecimento: 1920,
    soltaPelo: true,
    temperamento: "Sem cauda, brincalhão e inteligente",
    imagem: "/gatos/manx.jpg",
  },
  {
    raca: "Turco de Van",
    origem: "Turquia",
    anoReconhecimento: 1969,
    soltaPelo: true,
    temperamento: "Gosta de água, energético e inteligente",
    imagem: "/gatos/turkish_van.jpg",
  },
  {
    raca: "Havana Brown",
    origem: "Reino Unido",
    anoReconhecimento: 1958,
    soltaPelo: true,
    temperamento: "Exigente por atenção, brincalhão e dócil",
    imagem: "/gatos/havana_brown.jpg",
  },
];
```

1. Crie um elemento div com o id gatos;
2. Mapeie o vetor de gatos para dentro desta div (deve mostrar apenas imagem e raça);
3. Ao clicar, faça aparecer em um alert um texto informando origem, ano de reconhecimento e temperamento;
4. Crie um botão para pintar de vermelho o fundo dos itens de gatos que soltam pelo
5. Crie um botão para pintar de azul o fundo dos itens de gato cuja origem são os Estados Unidos
6. Crie um campo de texto e um botão filtrar. Ao pressionar o botão, pinte de roxo o fundo dos itens de gato que possuem o texto inserido no campo de texto (pesquisa nos campos raça, origem e temperamento). Sua busca deve ser case-insensitive. Utilize os método toLowerCase e includes. Exemplo:

```js
const textinho =
  "Vamos dar um rolê, eu vou te apresentar o melhor baile do Rio de Janeiro. Tu já sabe qual é, o Complexo da Penha é um verdadeiro pu...";
const textinhoEmMinusculas = textinho.toLowerCase();

const esseTrechoExiste = textinho.includes("Vamos dar um rolê"); // true
const esseTrechoNaoExiste = textinho.includes(
  "Golfinhos com botas de gelatina",
); // false
```

A partir daqui, é pra fazer aparecer no console, sem HTML:

7. Filtre os gatos reconhecidos depois dos anos 2000;
8. Qual a média dos anos de reconhecimento dos gatos?
9. Quantos gatos cuja origem não é dos Estados Unidos não soltam pelo?
10. Pergunte para o usuário via prompt qual gato ele quer ver (lá ele). Baseado na raça informada, redirecione o usuário para o link da imagem.

```js
window.location.href = "/gatos/havana_brown.jpg";
```

A entrega deve ser realizada através de um único link do GitHub. Apenas um integrante do grupo precisa entregar.
Lembre-se: nada de let, for, if, switch e outras paradas. O único momento onde o forEach é admitido é no momento de atribuir os eventos de clique!
