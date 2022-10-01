<template>
    <p className="message">
       {{message}}
       </p>
</template>
<script setup>

defineProps({
    message: {
        type: String,
        default:"Some generic Tweet about dogs",
    },
});

</script>

<style></style>