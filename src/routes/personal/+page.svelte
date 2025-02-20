<script>
  import logo from '$lib/assets/cdmx.png';
  import persona from '$lib/assets/person.webp'

  const people = ['Hugo Sanchez', 'Juan Hernandez', 'Adolfo Almazán', 'Hector Díaz', 'Alberto Jimenez', 'Ana Zavala', 'María Diaz', 'Rebecca Alaníz']
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
  <div class="personal_list">
    <button class="add_new">Añadir Inspector</button>
    <h3>Lista de Inspectores</h3>
    {#each people as humano}
    <div class="person">
      <img src={persona} alt="person">
      <h5>{humano}</h5>
      <p>Última Inspección</p>
      <button>Enviar mensaje</button>
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

  .personal_list {
    margin-top: 20px;
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 90%;
  }

  .person {
    margin-top: 20px;
    width: 90%;
    height: 150px;
    background-color: indianred;
    display: flex;
    justify-content: flex-start;
    align-items: center;
    border-radius: 10px;
    box-shadow: 1px 1px 2px 2px gray;
  }

  .person img {
    margin: 20px;
    width: 150px;
    border-radius: 15px;
  }

  .person h5 {
    margin: 20px;
  }

  .person p {
    margin: 20px;
  }

  .add_new {
    position: absolute;
    right: 100px;
    top: 210px;
  }
</style>
