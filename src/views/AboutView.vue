<script setup lang="ts">
import "../views/AboutView.css";
</script>

<template>
  <div class="about">
    <h1>This is an about page</h1>
    <br /><br />
  </div>
  <!-- Header da ficha -->
  <div class="container">
    <div class="header-input-group">
      <div class="input-contents">
        <label>Nome do personagem:</label>
        <input type="text" class="sheet-header-input-short" />
      </div>
      <div class="input-contents">
        <label>Classe do personagem:</label>
        <input type="text" class="sheet-header-input-short" />
      </div>
      <div class="input-contents">
        <label>Nível:</label>
        <input type="text" class="sheet-header-input-short" />
      </div>
    </div>
  </div>
  <!-- Atributos temporários -->
  <div class="container-temp-atr">
    <div class="boxes">
      <div class="box-item">
        <div class="box-item-child">
          <label>Armadura</label>
          <input type="text" class="sheet-header-input-short" />
        </div>
      </div>
      <div class="box-item">
        <div class="box-item-child">
          <label>Pontos de vida</label>
          <input type="text" class="sheet-header-input-short" />
        </div>
      </div>
      <div class="box-item">
        <div class="box-item-child">
          <label>Pontos de mana</label>
          <input type="text" class="sheet-header-input-short" />
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.boxes {
  display: flex;
  flex-direction: row;
  align-items: stretch;
  justify-content: space-evenly;
}

.box-item {
  display: flex;
  flex-direction: column;
  margin: 5px;
  border: solid;
  border-radius: 12px;
  border-width: 1px;
  padding: 8px;
  margin-top: 15px;
  align-items: center;
}

.box-item-child {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100%;
  text-align: center;
}

.box-item-child input {
  margin-top: 50px;
  text-align: center;
}

.container-temp-atr {
  display: flex;
  flex-direction: row;
  padding: 15px;
  margin: 5px;
}

.container {
  display: flex;
  flex-direction: row;
  border: solid;
  border-width: 1px;
  border-radius: 42px;
  padding: 15px;
  margin: 5px;
}

.header-input-group {
  display: flex;
  flex-direction: row;
  padding: 5px;
}

.input-contents {
  display: flex;
  flex-direction: column;
  margin-right: 15px;
}

.input-contents label {
  margin-bottom: 5px; /* Espaço entre o label e o input */
}

.sheet-header-input-short {
  width: 100%;
}
</style>
