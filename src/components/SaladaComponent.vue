<template>
  <div class="col">
    <div class="card">
      <div class="card-header">SALADAS</div>
      <div class="card-body">
        <div
          class="form-check form-check-inline"
          v-for="tipoSalada in tiposSalada"
          :key="tipoSalada.value"
        >
          <input
            :id="tipoSalada.value"
            class="form-check-input"
            :type="tipoSalada.type"
            :value="tipoSalada.value"
            v-model="inputTipoSalada"
          />
          <label class="form-check-label">{{ tipoSalada.label }}</label>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      inputTipoSalada: [],
      tiposSalada: [
        { label: "Alface", value: "alface", type: "checkbox" },
        { label: "Tomate", value: "Tomate", type: "checkbox" },
      ],
    };
  },
};
</script>
