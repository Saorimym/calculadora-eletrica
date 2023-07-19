<template>
  <div class="form-box">
    <h2>Cadastro Setor</h2>

    <form action="#">
      <div class="input-group">
        <label for="name">E-mail:</label>
        <input type="text" id="industryname" placeholder="Digite o nome do setor" required>
      </div>

      <div class="input-group button-group">
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
  padding: 5vw 5vh; /* Aumente o padding para tornar o formulário maior */
  max-width: 90vw; /* Defina a largura máxima para 90% da largura da janela */
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
  height: 5vh; /* Aumente a altura dos inputs */
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

form .input-group.button-group {
  display: flex;
  justify-content: space-between; /* Alinha os botões na horizontal com espaço entre eles */
}

form .input-group button {
  width: 23%; /* Defina a largura dos botões para ocupar espaço igualmente na linha */
  height: 5vh; /* Aumente a altura dos botões */
  background: #3232CD;
  border-radius: 20px;
  outline: none;
  border: none;
  color: white;
  cursor: pointer;
  font-size: 16px;
}

/* ajustar */
@media (max-width: 768px) {
  .form-box {
    padding: 3vw; /* Reduza o padding para manter o formulário maior em telas menores */
  }

  form .input-group.button-group {
    flex-direction: column; /* Alinha os botões verticalmente em telas menores */
  }

  form .input-group button {
    width: 100%;
    margin-top: 2vh;
  }
}
</style>
