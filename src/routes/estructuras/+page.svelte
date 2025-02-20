<script>
  import logo from '$lib/assets/cdmx.png';

  const list = [1,2,3,4,5,6,7,8,9,10,11,12,13];
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
  </div>
  <div class="list">
    <div class="Names">
    	  <p>No.</p>
    	  <p>Nombre</p>
    	  <p>Ubicación</p>
    	  <p>Estado</p>
    </div>
    {#each list as object}
    	<a href="./estructuras/puente" class="object_list">
    	  <p>{object}</p>
    	  <p>Sin Nombre</p>
    	  <p>100+050</p>
    	  <p>Crítico</p>
    	</a>

    {/each}
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

  .Names {
    display: flex;
    justify-content: space-evenly;
    align-items: flex-start;
    background-color: gray;
  }

  .Names p{
    margin: 0;
  }

  .list {
    width: 85vw;
  }

  .object_list {
    margin: 10px;
    text-decoration: none;
    color: black;
    width: 95%;
    display: flex;
    justify-content: space-evenly;
    background-color: lightcoral;
    border-radius: 5px;
    box-shadow: 1px 1px 1px 1px gray;
  }

</style>
