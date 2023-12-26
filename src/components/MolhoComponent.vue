<template>
  <div class="col">
    <div class="card">
      <div class="card-header">MOLHOS</div>
      <div class="card-body">
        <div
          class="form-check form-check-inline"
          v-for="tipoMolho in tiposMolho"
          :key="tipoMolho.value"
        >
          <input
            :id="tipoMolho.value"
            class="form-check-input"
            :type="tipoMolho.type"
            :value="tipoMolho.value"
            v-model="inputTipoMolho"
          />
          <label class="form-check-label">{{ tipoMolho.label }}</label>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      inputTipoMolho: [],
      tiposMolho: [
        { label: "Ketchup", value: "ketchup", type: "checkbox" },
        { label: "Mostarda", value: "mostarda", type: "checkbox" },
        { label: "Maionese", value: "maionese", type: "checkbox" },
      ],
    };
  },
};
</script>
