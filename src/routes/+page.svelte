<script>
    import Contacts from "$components/Contacts.svelte";
</script>

<main>
    <img src="/assets/top-bg.svg" alt="top background">
    <nav>
        <img src="/assets/Logo.svg" alt="logo GTI">
        <div>
            <p>Compétences</p>
            <p>Fournisseurs</p>
            <p>Clients</p>
        </div>
    </nav>
    <section class="accueil">
        <div>
            <h1>Gestion technique informatisée</h1>
            <p>Spécialistes de la gestion technique des <br>
                bâtiments capables d’assembler et <br>
                mettre en œuvre des systèmes ouverts <br>
                au besoin du client</p>
        </div>
        <div class="fournisseurs">
            <img src="/assets/trend.png" alt="logo fournisseur trend">
            <img src="/assets/wago.png" alt="logo fournisseur trend">
            <img src="/assets/distech.png" alt="logo fournisseur trend">
            <p>Voir d'autres</p>
        </div>
    </section>
    <Contacts />
</main>

<style>
    :global(*){
        font-family: "Prompt", sans-serif;
    }

    main>img{
        z-index: -1;
        position: absolute;
        width: 100%;
        top:-13%;
        left:0;
    }

    nav{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        padding: 50px;
        padding-left: 100px;
    }
    
    nav img{
        width: 171px;
        height: 112px;
    }
    
    nav p{
        color: #002B3D;
        margin-bottom: 0;
        background: linear-gradient(to bottom, #ffffff00 96%, #002B3D 96%);
        margin-left: 25px;
        margin-right: 25px;
        font-size: 1.6em;
        font-weight: 200;
    }
    
    nav div{
        display: flex;
        height: 60px;
    }

    section p{
        font-size: 32px;
        font-weight: 300;
    }

    h1{
        font-size: 38px;
        font-weight: 700;
    }

    .accueil{
        padding-left: 100px;
        padding-top: 100px;
        display: flex;
    }

    .fournisseurs{
        position: relative;
        /* border: 1px solid red; */
        width: 50%;
        margin-left: 20px;
    }

    .fournisseurs img{
        width: 274px;
    }

    .fournisseurs > img:nth-child(1){
        position: absolute;
        top: 0;
        left: 10%;
    }

    .fournisseurs > img:nth-child(2){
        position: absolute;
        top: 25%;
        right: 5%;
    }

    .fournisseurs > img:nth-child(3){
        position: absolute;
        bottom: 10%;
        left: 5%;
    }

    .fournisseurs p{
        font-size: 25px;
        position: absolute;
        bottom: 0;
        right: 0;
    }

</style>