<script>
  import logo from '$lib/assets/cdmx.png';

  const messajes = [{name: 'Hugo Zavala', message: 'problemas en inspección', estado: 'Urgente'},{name: 'Maria Sanchez', message: 'Información erronea', estado: 'Atención'},{name: 'Adolfo Almazán', message: 'Inspecciónes Completadas', estado: 'Positivo'},{name: 'Hugo Zavala', message: 'suspención de actividades por lluvia', estado: 'informativo'},{name: 'Hugo Zavala', message: 'retraso de 1 día', estado: 'Informativo'}];
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
  <div class="message_list">
    {#each messajes as item}
    	<div class= 'message_card'>
    	  <p>{item.name}</p>
    	  <p>{item.message}</p>
    	  <p>{item.estado}</p>
    	</div>
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

  .message_list {
    display: grid;
    grid-template-columns: 33% 33% 33%;
  }

  .message_card {
    margin: 10px;
    width: 24vw;
    height: 24vw;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    align-items: center;
    text-align: center;
    background-color: lightcoral;
    border-radius: 6px;
    cursor: pointer;
    box-shadow: 1px 1px 2px 2px gray;
  }

  .message_card:nth-child(2) {
    background-color: yellow;
  }
  .message_card:nth-child(3) {
    background-color: green;
  }
  .message_card:nth-child(4) {
    background-color: lightgray;
  }
  .message_card:nth-child(5) {
    background-color: lightgray;
  }

  .message_card p:nth-child(1) {
    font-weight: bold;
  }

  .message_card p:nth-child(2) {
    font-size: 0.7rem; 
  }

  .message_card p:nth-child(3) {
    font-size: 0.9rem; 
    font-weight: bold;
  }
</style>
