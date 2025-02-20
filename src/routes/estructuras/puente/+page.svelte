<script>
  import logo from '$lib/assets/cdmx.png';
  import img_bridge from '$lib/assets/telford-bridge-craigellachie.jpg';
  import map from '$lib/assets/map.png'
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
  <div class="info">
    <div class="images">
      <img class="img_main" src={img_bridge} alt="puente">
      <div class="mini_img">
        <img src={img_bridge} alt="puente">
        <img src={img_bridge} alt="puente">
        <img src={img_bridge} alt="puente">
        <img src={img_bridge} alt="puente">
      </div>
    </div>
    <div class="general_info">
      <h5>Nombre del Puente</h5>
      <p class="gray_info">100+050</p>

      <div class="inspector">
        <h5>Última Inspección</h5>
        <div>
          <div class="user">
            <img src="" alt="I">
            <h6>Jorge Sanchez</h6>
          </div >
          <p class="gray_info">12/05/2025</p>
          <p>Crítica</p>
        </div>
      </div>
      <div class="general">
        <div>
          <p>Condición General:</p>
          <p>Crítica</p>
        </div>
        <div>
          <p>Tipo de Puente:</p>
          <p>Concreto Armado</p>
        </div>
      </div>
      <div class="bloques_info">
        <h5>Información General</h5>
        <div>
          <p class="gray_info">Nombre del Puente:</p>
          <p>Sin Nombre</p>
        </div>
        <div>
          <p class="gray_info">Colonia:</p>
          <p>Peralvillo</p>
        </div>
        <div>
          <p class="gray_info">Alcaldía:</p>
          <p>Venustiano Carranza</p>
        </div>
        <div>
          <p class="gray_info">Entre Calles:</p>
          <p>Wagner y Mapimí</p>
        </div>
        <div>
          <p class="gray_info">Ubicado en:</p>
          <p>Vialidad Primaria</p>
        </div>
      </div>
      <div class="bloques_info">
        <h5>Daños y Agrietamientos</h5>
        <div>
          <p class="gray_info">Agrietamiento en Losas de Apoyo:</p>
          <p class="regular">Regular</p>
        </div>
        <div>
          <p class="gray_info">Daño en Parapeto/Pasamanos:</p>
          <p class="bueno">Bueno</p>
        </div>
        <div>
          <p class="gray_info">Superficie de Rodamiento:</p>
          <p class="malo">Malo</p>
        </div>
        <div>
          <p class="gray_info">Daño por Impacto Vehicular:</p>
          <p class="critico">Crítico</p>
        </div>
        <div>
          <p class="gray_info">Desnivelación de Coladeras:</p>
          <p class="critico">Crítico</p>
        </div>
      </div>
      <img class="map" src={map} alt="map">
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

  .info {
    width: 85vw;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .images {
    margin-top: 30px;
    width: 100%;
    border-radius: 10px;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .img_main {
    width: 500px;
    border-radius: 10px;
    cursor: pointer;
  }

  .mini_img {
    width: 100px;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    cursor: pointer;
  }

  .mini_img img {
    margin: 10px;
    width: 100%;
    border-radius: 10px;
  }

  .general_info {
    width: 85%;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }

  .general_info h5 {
    margin: 0;
    padding: 0;
  }

  .gray_info {
    padding: 0;
    margin: 0;
    color: gray;
    font-size: 0.8rem;
  }

  .inspector {
    width: 100%;
  }

  .inspector div {
    display: flex;
    padding-right: 50px;
    justify-content: flex-start;
    align-items: center;
  }

  .inspector div p {
    padding-right: 50px;
  }

  .inspector div p:last-child {
    color: red;
  }

  .user img{
    margin-right: 10px;
  }

  .general {
    width: 100%;
  }

  .general div {
    width: 100%;
    display: flex;
    justify-content: flex-start;
    align-items: flex-start;
  }

  .general div p:nth-child(1) {
    font-weight: bold;
    margin-right: 50px;
  }

  .general div:nth-child(1) p:nth-child(2) {
    color: red;
  }

  .bloques_info {
    width: 100%;
  }

  .bloques_info div {
    display: grid;
    grid-template-columns: 70% 30%;
  }

  .bloques_info div p {
    margin: auto 0 auto 0;
  }

  .regular {
    color: yellow;
  }

  .bueno {
    color: green;
  }

  .malo {
    color: orange;
  }

  .critico {
    color: red;
  }

  .map {
    margin-top: 50px;
    margin-bottom: 50px;
    width: 100%;
    border-radius: 10px;
  }

</style>
