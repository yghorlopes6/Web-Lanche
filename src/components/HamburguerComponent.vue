<template>
  <div class="col">
    <div class="card">
      <div class="card-header">HAMBÚRGUER</div>
      <div class="card-body">
        <div
          class="form-check form-check-inline"
          v-for="tipoHamburguer in tiposHamburguer"
          :key="tipoHamburguer.value"
        >
          <input
            class="form-check-input"
            :type="tipoHamburguer.type"
            :value="tipoHamburguer.value"
            v-model="inputTipoHamburguer"
          />
          <label class="form-check-label">{{ tipoHamburguer.label }}</label>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      inputTipoHamburguer: "",
      tiposHamburguer: [
        { label: "Bovino", value: "bovino", type: "radio" },
        { label: "Frango", value: "frango", type: "radio" },
        { label: "Soja", value: "soja", type: "radio" },
      ],
    };
  },
};
</script>
