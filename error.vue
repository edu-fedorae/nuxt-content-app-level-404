<script setup>
const error = useError();
</script>

<template>
    <div class="uk-container uk-position-center">
        <div class="uk-text-center">
            <h1 class="uk-heading">{{ error.statusCode }}</h1>
            <p>{{ error.statusMessage }}</p>

            <button class="uk-button uk-button-default" @click="clearError({ redirect: '/' })">Home</button>
        </div>
    </div>
</template>
