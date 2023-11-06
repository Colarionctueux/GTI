<main>
    <img src="/top-bg.svg" alt="top background">
    <nav>
        <img src="/Logo.svg" alt="logo GTI">
        <div>
            <p>Compétences</p>
            <p>Fournisseurs</p>
            <p>Clients</p>
        </div>
    </nav>
</main>

<style>
    main>img{
        margin: 0;
        padding: 0;
        z-index: -1;
        position: absolute;
        width: 100%;

        top:0px;
        left:0px;
    }

    nav{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        margin: 50px;
        margin-top: 20px;
    }

    nav img{
        width: 171;
        height: 112;
    }

    nav p{
        color: #002B3D;
        margin-bottom: 0;
        background: linear-gradient(to bottom, #ffffff00 95%, #002B3D 95%);
        margin-left: 25px;
        margin-right: 25px;
        font-size: 1.6em;
        font-family: "Prompt", sans-serif;
        font-weight: 200;
    }
    
    nav div{
        display: flex;
        height: 60px;
    }
</style>