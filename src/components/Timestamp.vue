<template>
  <span className="timestamp">{{timestamp}}</span>
</template>
<script setup>

defineProps({
    timestamp: {
        type: String,
        default: () =>{
             let date= new Date();
             return date.toISOString().split("T")[0];
        }
        // Hacemos esto de arriba en el default para que se nos imprima la fecha del dia de hoy
        // en el cado de que hay algun error en el array
    },
});

</script>

<style></style> 