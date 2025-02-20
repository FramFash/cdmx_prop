<script>
  import logo from '$lib/assets/cdmx.png';

  const lista = [1,2,3,4,5,6];
</script>

<header><img src={logo} alt="cdmx"></header>

<div class="booty">
  <div class="Navbar">
    <div>
      <img src="" alt="I">
      <a href="../">Avance</a>
    </div>
    <div>
      <img src="" alt="I">
      <a href="../estructuras">Estructuras</a>
    </div>
    <div>
      <img src="" alt="I">
      <a href="../personal">Personal</a>
    </div>
    <div>
      <img src="" alt="I">
      <a href="../mensajes">Mensajes</a>
    </div>
    <div>
      <img src="" alt="I">
      <a href="../mobil">Móbil</a>
    </div>
  </div>
  <div class="container">
    <div class="mobil">
      <div class="topbar"></div>
      <img src={logo} alt="logo">
      <div class="lista">
        <a href="../mobil" class="back">atras</a>
        <h5>Lista de Estructuras</h5>
        {#each lista as inspeccion}
        	<div class="listing">
        	  <p>{inspeccion}</p>
        	  <a href="../mobil/puente">Sin Nombre</a>
        	  <p>Completada</p>
        	</div>
        {/each}
      </div>
    </div>
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

  .container {
    width: 85%;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .mobil {
    height: 60vh;
    width: 35vw;
    border-radius: 15px;
    border: 1px solid black;
    overflow-y: scroll;
  }

  .topbar {
    width: 100%;
    height: 20px;
    background-color: black;
    border-radius: 15px 15px 0 0;
  }

  .mobil img {
    margin-left: 10%;
    width: 80%;
  }

  .lista {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .listing {
    width: 80%;
    margin: 5px;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    background-color: indianred;
    border-radius: 10px;
    box-shadow: 1px 1px 1px 1px gray;
  }

  .listing a {
    text-decoration: none;
    color: black;
  }

  .listing p:last-child {
    color: darkgreen;
    font-weight: bold;
  }

  .back {
    position: absolute;
    left: 43%;
    top: 43%;
    text-decoration: none;
    color: black;
    background-color: lightgray;
    border: 1px solid gray;
    border-radius: 5px;
  }
</style>
