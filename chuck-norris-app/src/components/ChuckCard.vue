<template>
    <div class="col-lg-4 col-md-6 col-sm-12 mb-4">
      <div class="card">
        <img :src="iconUrl" class="card-img-top" alt="Chuck Norris">
        <div class="card-body">
          <p class="card-text">{{ value }}</p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ChuckCard',
    props: {
      iconUrl: {
        type: String,
        required: true
      },
      value: {
        type: String,
        required: true
      }
    }
  };
  </script>
  
  <style scoped>
  /* Aquí puedes agregar estilos adicionales si es necesario */
  </style>
  