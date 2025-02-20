<script>
  import logo from '$lib/assets/cdmx.png';
  import stats from '$lib/assets/stats.png';
</script>

<header><img src={logo} alt="cdmx"></header>

<div class="booty">
  <div class="Navbar">
    <div>
      <img src="" alt="I">
      <a href="./">Avance</a>
    </div>
    <div>
      <img src="" alt="I">
      <a href="./estructuras">Estructuras</a>
    </div>
    <div>
      <img src="" alt="I">
      <a href="./personal">Personal</a>
    </div>
    <div>
      <img src="" alt="I">
      <a href="./mensajes">Mensajes</a>
    </div>
    <div>
      <img src="" alt="I">
      <a href="./mobil">Móbil</a>
    </div>
  </div>
  <div class="stats">
    <input type="text" placeholder="Buscar">
    <button class="PDF">Generar PDF</button>
    <img src={stats} alt="stats">
  </div>
</div>

<style>
  header {
    height: 20vh;
  }

  header img {
    height: 100%;
  }

  .booty {
    display: flex;
    height: 80vh;
  }

  .Navbar {
    height: 100%;
    width: 15vw;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    border: gray 1px solid;
    border-radius: 4px;
  }

  .Navbar div {
    margin: 10px 0 10px 20px;
  }

  .Navbar div a {
    text-decoration: none;
    color: black;
    
  }

  .stats {
    width: 85vw;
  }

  .stats input {
    height: 20px;
    width: 400px;
    margin-left: 30px;
    margin-bottom: 20px;
    background-color: lightgray;
    border-radius: 6px;
  }

  .stats img {
    width: 100%;
  }

  .PDF {
    position: absolute;
    height: 20px;
    width: 100px;
    right: 90px;
    border: 1px solid lightgray;
    border-radius: 5px;
  }
</style>
