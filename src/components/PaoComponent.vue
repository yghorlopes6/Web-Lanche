<template>
  <div class="col">
    <div class="card">
      <div class="card-header">PÃO</div>
      <div class="card-body">
        <div
          class="form-check form-check-inline"
          v-for="tipoPao in tiposPao"
          :key="tipoPao.value"
        >
          <input
            class="form-check-input"
            :type="tipoPao.type"
            :value="tipoPao.value"
            v-model="inputTipoPao"
          />
          <label class="form-check-label">{{ tipoPao.label }}</label>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      inputTipoPao: "",
      tiposPao: [
        { label: "Gergelim", value: "gergelim", type: "radio" },
        { label: "Australiano", value: "australiano", type: "radio" },
      ],
    };
  },
};
</script>
