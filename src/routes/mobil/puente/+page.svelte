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
      <a href="./lista" class="back">atras</a>
      <div class="info">
        <h5>Calz.Misterios y Circuito Interior (Dir. F.C. Hidalgo)(Sur)</h5>
        <div class="table">
          <p>Colonia:</p>
          <p>Peralvillo</p>
          <p>Alcaldía:</p>
          <p>Venustiano Carranza</p>
          <p>Entre Calles:</p>
          <p>Wagner y Mapimí</p>
          <p>Ubicado En:</p>
          <p>Vialidad Primaria</p>
        </div>

        <h5>Superestructura</h5>

        <label for="losas">Agrietamiento en losas de Apoyo</label>
        <select name="losas" id="losas" class="selection">
          <option value="" selected disabled hidden></option>
          <option value="bueno">Bueno</option>
          <option value="regular">Regular</option>
          <option value="malo">Malo</option>
          <option value="critico">Crítico</option>
        </select>
        <label for="pasamanos">Daño en Parapeto/Pasamanos:</label>
        <select name="pasamanos" id="pasamanos" class="selection">
          <option value="" selected disabled hidden></option>
          <option value="bueno">Bueno</option>
          <option value="regular">Regular</option>
          <option value="malo">Malo</option>
          <option value="critico">Crítico</option>
        </select>
        <label for="rodamiento">Superficie de Rodamiento:</label>
        <select name="rodamiento" id="rodamiento" class="selection">
          <option value="" selected disabled hidden></option>
          <option value="bueno">Bueno</option>
          <option value="regular">Regular</option>
          <option value="malo">Malo</option>
          <option value="critico">Crítico</option>
        </select>
        <label for="rodamiento">Daño por Impacto Vehicular:</label>
        <select name="vehicular" id="vehicular" class="selection">
          <option value="" selected disabled hidden></option>
          <option value="bueno">Bueno</option>
          <option value="regular">Regular</option>
          <option value="malo">Malo</option>
          <option value="critico">Crítico</option>
        </select>
        <label for="coladeras">Desnivelación de Coladeras:</label>
        <select name="coladeras" id="coladeras" class="selection">
          <option value="" selected disabled hidden></option>
          <option value="bueno">Bueno</option>
          <option value="regular">Regular</option>
          <option value="malo">Malo</option>
          <option value="critico">Crítico</option>
        </select>
        <h5>Comentarios:</h5>
        <textarea cols="40" rows="5" class="comentarios"></textarea>
        <button class="submit">Guardar</button>
        <div class="bottom_bar">
          <a href="../mobil/puente">Superestructura</a>
          <a href="../mobil/puente/otros">Otros</a>
        </div>
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
    overflow-x: hidden;
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

  .back {
    margin-left: 10%;
    text-decoration: none;
    color: black;
    background-color: lightgray;
    border: 1px solid gray;
    border-radius: 5px;
  }

  .info {
    width: 100%;
    padding: 10px;
  }

  .table {
    width: 80%;
    display: grid;
    grid-template-columns: 50% 50%;
    color: gray;
    font-size: 0.7rem; 
    margin-bottom: 10px;
  }

  .table p {
    margin: 0;
  }

  .selection {
    width: 90%;
    height: 25px;
    border: none;
    border-radius: 5px;
  }

  .comentarios {
    width: 90%;
    height: 50px;
  }

  .bottom_bar {
    width: 100%;
    height: 40px;
    margin-top: 10px;
    background-color: black;
    color: white;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
  }

  .bottom_bar a {
    text-decoration: none;
    color: white;
  }

  .submit {
    margin-top: 10px;
    margin-bottom: 20px;
    width: 90%;
    height: 40px;
    background-color: indianred;
    border-radius: 10px;
  }
</style>
