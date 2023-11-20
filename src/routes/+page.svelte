<script>
  import Competence from "$components/Competence.svelte";
  import Contacts from "$components/Contacts.svelte";
  import Fa from "svelte-fa";
  import { faLongArrowDown } from "@fortawesome/free-solid-svg-icons";
</script>

<main>
  <img src="/assets/top-bg.svg" alt="top background" />
  <img src="/assets/bottom-bg.svg" alt="bottom background" />
  <nav>
    <img src="/assets/Logo.svg" alt="logo GTI" />
    <div>
      <a href="#competences">Compétences</a>
      <a href="#fournisseurs">Fournisseurs</a>
      <a href="#clients">Clients</a>
    </div>
  </nav>
  <section class="accueil">
    <div>
      <h1>Gestion technique informatisée</h1>
      <p>
        Spécialistes de la gestion technique des <br />
        bâtiments capables d’assembler et <br />
        mettre en œuvre des systèmes ouverts <br />
        au besoin du client
      </p>
    </div>
    <div class="side-accueil">
      <img src="/assets/trend.png" alt="logo fournisseur trend" />
      <img src="/assets/wago.png" alt="logo fournisseur wago" />
      <img src="/assets/distech.png" alt="logo fournisseur distech" />
      <a href="#fournisseurs">Voir d'autres</a>
    </div>
  </section>
  <Contacts />
  <section id="competences">
    <h2>
      Nous travaillons dans <br />
      de nombreux domaines <br />
      pour plusieurs entreprises
    </h2>
  </section>
  <section class="competences">
    <Competence src="/assets/datacenter.png" alt="Datacenter">
      <span slot="title"> Datacenter </span>
      <span slot="paragraph"
        >Nous intervenons dans les data centers pour faire des trucs mais je ne
        sais pas quoi moi je fais juste des sites je demanderai quoi mettre</span
      >
    </Competence>
    <Competence
      src="/assets/sports.png"
      alt="tuyauterie sous-terraine de piscine"
    >
      <span slot="title"> Sports et loisirs </span>
      <span slot="paragraph"
        >Nous offrons nos services à des piscines et je coble le vide parceque
        je sais pas exactement ce que vous faites pour les piscines</span
      >
    </Competence>
    <Competence
      src="/assets/bureaux.png"
      alt="immeubles vue en contre-plongée avec les ciel derriere"
    >
      <span slot="title"> Bureaux </span>
      <span slot="paragraph"
        >Les bureaux ca nous connait parcequ’on travaille dedans comme 99% des
        entreprises je pense et ca parrait assez logique</span
      >
    </Competence>
    <Competence
      src="/assets/education.png"
      alt="étudiant lisant un livre dans une bibliothèque moderne"
    >
      <span slot="title"> Éducations </span>
      <span slot="paragraph"
        >Les écoles peuvent profiter de nos services pour etre connecté a
        internet ou je sais pas je comble pour faire semblant</span
      >
    </Competence>
    <Competence
      src="/assets/sante.png"
      alt="Materiel médical issu d'un hopital"
    >
      <span slot="title"> Santé </span>
      <span slot="paragraph"
        >La santé c’est important, mangez au moins cinq fruits et légumes par
        jour, ne mangez pas entre les repas et brossez vous les dents</span>
    </Competence>
  </section>
  <section id="fournisseurs">
    <h2>
      Les multiples fournisseurs<br />
      avec qui nous travaillons
    </h2>
  </section>
  <section class="fournisseurs">
  <div>
    <picture><img src="/assets/trend.png" alt="logo fournisseur trend" /></picture>
    <button><Fa icon={faLongArrowDown} /></button>
  </div>
  <div>
    <picture><img src="/assets/wago.png" alt="logo fournisseur wago" /></picture>
    <button><Fa icon={faLongArrowDown} /></button>
  </div>
  <div>
    <picture><img src="/assets/distech.png" alt="logo fournisseur distech" /></picture>
    <button><Fa icon={faLongArrowDown} /></button>
  </div>
  <div>
    <picture><img src="/assets/distech.png" alt="logo fournisseur distech" /></picture>
    <button><Fa icon={faLongArrowDown} /></button>
  </div>
  <div>
    <picture><img src="/assets/trend.png" alt="logo fournisseur trend" /></picture>
    <button><Fa icon={faLongArrowDown} /></button>
  </div>
  <div>
    <picture><img src="/assets/wago.png" alt="logo fournisseur wago" /></picture>
    <button><Fa icon={faLongArrowDown} /></button>
  </div>
  <div>
    <picture><img src="/assets/wago.png" alt="logo fournisseur wago" /></picture>
    <button><Fa icon={faLongArrowDown} /></button>
  </div>
  <div>
    <picture><img src="/assets/distech.png" alt="logo fournisseur distech" /></picture>
    <button><Fa icon={faLongArrowDown} /></button>
  </div>
  <div>
    <picture><img src="/assets/trend.png" alt="logo fournisseur trend" /></picture>
    <button><Fa icon={faLongArrowDown} /></button>
    </div>
  </section>
  <section id="clients">
    <h2>Les clients qui nous font confiance</h2>
    <h2>Nos clients constructeurs</h2>
  </section>
  <section class="clients">
    <div>
      <img src="/assets/cofidis.png" alt="logo cofidis">
      <img src="/assets/helicea.png" alt="logo hélicéa piscines">
      <img src="/assets/centerparcs.png" alt="logo center parcs">
    </div>
    <div>
      <img src="/assets/cofidis.png" alt="logo cofidis">
      <img src="/assets/helicea.png" alt="hélicéa piscines">
      <img src="/assets/centerparcs.png" alt="logo center parcs">
    </div>
  </section>
  <footer>
    <img src="/assets/Logo.svg" alt="logo GTI" />
    <a href="google.com" target="_blank">Mentions légales</a>
    <a href="google.com" target="_blank">Conditions générales</a>
    <a href="mailto:stephane.eckman@gestion-technique-informatisee.fr">Nous contacter</a>
  </footer>
</main>

<style>
  :global(*) {
    font-family: "Prompt", sans-serif;
    scroll-behavior: smooth;
  }

  main > img:first-of-type {
    z-index: -1;
    position: absolute;
    width: 100%;
    top: -13%;
    left: 0;
  }

  main > img:last-of-type {
    z-index: -1;
    position: absolute;
    width: 100%;
    left: 0;
    top: 340%;
  }

  nav {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding: 50px;
    padding-left: 100px;
  }

  nav img {
    width: 171px;
    height: 112px;
  }

  nav a {
    color: #002b3d;
    display: inline-block;
    margin-bottom: 0;
    background-image: linear-gradient(#002b3d 0 0);
    background-position: 0 100%;
    background-size: 0% 2px;
    background-repeat: no-repeat;
    height: 70%;
    transition: background-size 0.3s, background-position 0s 0.3s;
    margin-left: 25px;
    margin-right: 25px;
    font-size: 1.6em;
    font-weight: 200;
    text-decoration: none;
  }

  nav a:hover{
    background-position: 100% 100%;
    background-size: 100% 2px;
  }

  nav div {
    display: flex;
    height: 60px;
  }

  section p {
    font-size: 32px;
    font-weight: 300;
  }

  h1 {
    color: #002b3d;
    font-size: 38px;
    font-weight: 700;
  }

  .accueil {
    padding-left: 100px;
    padding-top: 50px;
    margin-bottom: 60px;
    display: flex;
  }

  .side-accueil {
    position: relative;
    width: 50%;
    margin-left: 20px;
  }

  .side-accueil img {
    width: 274px;
  }

  .side-accueil > img:nth-child(1) {
    position: absolute;
    top: 0;
    left: 10%;
  }

  .side-accueil > img:nth-child(2) {
    position: absolute;
    top: 25%;
    right: 5%;
  }

  .side-accueil > img:nth-child(3) {
    position: absolute;
    bottom: 15%;
    left: 5%;
  }

  .side-accueil a {
    font-size: 25px;
    position: absolute;
    bottom: 0;
    right: 0;
    color: #002b3d;
    text-decoration: none;
  }

  h2 {
    font-size: 34px;
    font-weight: 400;
    text-align: center;
    position: absolute;
    color: #002b3d;
  }

  #competences {
    position: relative;
    height: 200px;
    color: #002b3d;
    margin-bottom: 10px;
  }


  #competences h2 {
    top: 0;
    left: 130px;
  }

  .competences {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    margin-bottom: 300px;
  }

  #fournisseurs {
    position: relative;
    height: 200px;
    color: #002b3d;
  }

  #fournisseurs h2 {
    top: 0;
    left: 100px;
    color: #002b3d;
  }

  .fournisseurs{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    padding: 50px;
    margin-bottom: 110px;
  }

  .fournisseurs div{
    display: flex;
    position: relative;
    justify-content: center;
    align-items: center;
    transform: translateY(0);
    max-width: 450px;
  }
  
  .fournisseurs img {
    height: 110px;
  }
  
  picture{
    border-radius: 10px;
    box-sizing: border-box;
    margin: 50px;
    transition: all .3s;
    background-color: rgb(255, 255, 255);
    border: 1px solid #002b3d;
    padding: 10px;
    z-index: 1;
    display: block;
    position: relative;
  }

  .fournisseurs picture::after{
    content: "";
    position: absolute;
    bottom: -2px;
    left: 50%;
    transform: translateX(-50%);
    width: 39px;
    height: 4px;
    z-index: 20000;
    background-color: white;
    opacity: 0;
  }

  .fournisseurs picture:hover::after{
    opacity: 1;
  }
  
  .fournisseurs button{
    text-align: center;
    position: absolute;
    bottom: 25%;
    transform: translateY(0);
    transition: all .3s;
    color: #002b3d;
    background-color: rgb(255, 255, 255);
    border-radius: 0;
    height: 40px;
    width: 40px;
    font-size: 1.4em;
    border: 1px solid #002b3d;
    border-top: none;
  }
  
  .fournisseurs picture:hover + button{
    border-radius: 0 0 25% 25%;
    transform: translateY(23px);
  }

  .fournisseurs picture:hover{
    transform: translateY(-23px);
  }

  #clients{
    position: relative;
    height: 200px;
    color: #002b3d;
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 50px;
  }

  #clients h2:last-of-type{
    right: 9%;
    width: 27%;
  }

  #clients h2:first-of-type{
    left: 12%;
    width: 25%;
  }

  .clients{
    display: flex;
    justify-content: space-around;
  }

  .clients img{
    width:186px;
  }

  footer{
    background-color: rgb(192, 192, 192);
    left: 0;
    position: absolute;
    width: 100%;
    height: 80px;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 70px;
  }

  footer img{
    height: 80%;
    margin-right: 20px;
  }

  footer a{
    margin-left: 20px;
    margin-right: 20px;
    color: #002b3d;
    text-decoration: none;
  }

</style>
