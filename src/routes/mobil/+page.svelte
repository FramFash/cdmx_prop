<script>
  import logo from '$lib/assets/cdmx.png';
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
      <div class="login">
        <h4>Iniciar Sesión</h4>
        <input type="text" placeholder="Correo Electronico">
        <input type="text" placeholder="Contraseña">
      </div>
      <div class="inicio_boton"><a href="../mobil/lista">Iniciar</a></div>
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
  }

  .topbar {
    width: 100%;
    height: 20px;
    background-color: black;
    border-radius: 15px 15px 0 0;
  }

  .mobil img {
    margin-top: 30%;
    margin-left: 10%;
    width: 80%;
  }

  .login {
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .login input {
    margin-bottom: 10px;
    border-radius: 5px;
    background-color: lightgray;
  }

  .inicio_boton {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 5%;
    margin-left: 30%;
    width: 40%;
    height: 10%;
    background-color: indianred;
    color: black;
    font-weight: bold;
    border-radius: 10px;
    box-shadow: 1px 1px 2px 2px gray;
  }

  .inicio_boton a {
    text-decoration: none;
    color: black;
  }
</style>
