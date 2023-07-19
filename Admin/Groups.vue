<template>
  <div class="form-box">
    <h2>Cadastro de grupos</h2>

    <form action="#">
      <div class="input-group">
        <label for="adm">Administrador: </label>
        <input type="text" id="adm" placeholder="Digite o Administrador" required>
      </div>

      <div class="input-group">
        <label for="operation">Operação: </label>
        <input type="operation" id="operation" placeholder="Digite a sua operação" required>
      </div>

      <div class="input-group">
        <button>Incluir</button>
        <button>Alterar</button>
        <button>Gravar</button>
        <button>Excluir</button>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  //caso necessário
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500&display=swap');
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
}

body {
  background-image: url(background.png);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
}

.form-box {
  background-color: rgba(255, 255, 255, 0.4);
  backdrop-filter: blur(40px);
  padding: 30px 40px;
  max-width: 800px; /* Aumente a largura máxima para tornar o formulário maior na horizontal */
  width: 100%;
  border-radius: 20px;
}

.form-box h2 {
  font-size: 30px;
}

form .input-group {
  margin-bottom: 15px;
}

form .input-group label {
  color: #3D3D3D;
  font-weight: bold;
  display: block;
  margin-bottom: 5px;
}

form .input-group input {
  width: 100%;
  height: 47px;
  background-color: rgba(255, 255, 255, 0.32);
  border-radius: 20px;
  outline: none;
  border: 2px solid transparent;
  padding: 15px;
  font-size: 15px;
  color: #616161;
  transition: all 0.4s ease;
}

form .input-group input:focus {
  border-color: #ff008869;
}

form .input-group button {
  width: 20%;
  height: 47px;
  background: #3232CD;
  border-radius: 20px;
  outline: none;
  border: none;
  margin-right: 15px;
  margin-top: 15px;
  color: white;
  cursor: pointer;
  font-size: 16px;
}

/* ajustar */
@media (max-width: 768px) {
  .form-box {
    padding: 20px;
  }

  form .input-group button {
    width: 100%;
    margin-right: 0;
    margin-top: 10px;
  }
}
</style>
