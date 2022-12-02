<template>
  <div>
    <p>Componente de mensagem</p>
    <div>
      <form action="" id="burger-form">
        <div class="input-container">
          <label for="name">Nome do Cliente:</label>
          <input
            type="text"
            id="name"
            v-model="name"
            placeholder="Digite seu nome"
          />
        </div>
        <div class="input-container">
          <label for="bread">Escolha seu pão:</label>
          <select name="bread" id="bread" v-model="bread">
            <option value="">Selecione seu pão</option>
            <option value="integral">Integral</option>
          </select>
        </div>
        <div class="input-container">
          <label for="meat">Escolha a carne do seu Burger pão:</label>
          <select name="meat" id="meat" v-model="meat">
            <option value="">Selecione a carne</option>
            <option value="maminha">Maminha</option>
          </select>
        </div>
        <div class="input-container">
          <label id="optinal-title" for="optional"
            >Selecione os opcionais:</label
          >
          <div class="checkbox-container">
            <input
              type="checkbox"
              name="optional"
              v-model="opcionais"
              value="salame"
            />
            <span>Salame</span>
          </div>
        </div>
        <div class="input-optional">
          <input type="submit" class="submit-btn" value="Criar meu Burger!" />
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "BurgerForm",
};
</script>

<style scoped>
#burger-form {
  max-width: 400px;
  margin: 0 auto;
}

.input-container {
  display: flex;
  flex-direction: column;
  margin-bottom: 20px;
}
label {
  font-weight: bold;
  margin-bottom: 15px;
  color: #222;
  padding: 5px 10px;
  border-left: 4px solid #fcba03;
}

input,
select {
  padding: 5px 10px;
  width: 300px;
}

#opcionais-container {
  flex-direction: row;
  flex-wrap: wrap;
}

#optional-title {
  width: 100%;
}

.checkbox-container {
  display: flex;
  align-items: flex-start;
  width: 50%;
  margin-bottom: 20px;
}
</style>
