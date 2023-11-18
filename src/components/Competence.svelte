<script>
  export let src;
  export let alt;
</script>

<main>
  <img {src} {alt} />
  <h3>
    <slot name="title" />
  </h3>
  <p>
    <slot name="paragraph" />
  </p>
</main>

<style>
  img {
    width: 100%;
  }

  main {
    border-radius: 38px;
    padding: 15px;
    width: 24%;
    min-width: 220px;
    box-sizing: border-box;
    height: 470px;
    margin: 50px;
    margin-bottom: 20px;
    box-shadow: 0 0 6px rgba(60, 60, 60, 0.2);
    display: flex;
    flex-direction: column;
    align-items: center;
    transition: transform .3s ease;
  }

  h3 {
    font-size: 1.9em;
    font-weight: bold;
    margin-top: 10px;
    margin-bottom: 12px;
    padding-bottom: 15px;
    text-align: center;
    width: 85%;
    color: #002b3d;
    border-bottom: 2px solid #002b3d;
  }

  p {
    font-size: 1.2em;
    font-weight: 300;
    width: 100%;
    text-align: center;
    margin-top: 20px;
    color: #002b3d;
  }

  main:hover{
    transform: scale(1.02);
  }
</style>
