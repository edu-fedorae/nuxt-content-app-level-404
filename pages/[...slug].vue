<script setup>
const notFoundError = () => {
    throw createError({ statusCode: 404, statusMessage: "Page not found", fatal: true });
};
</script>

<template>
    <main>
        <ContentDoc>
            <template #not-found>
                {{ notFoundError() }}
            </template>
        </ContentDoc>
    </main>
</template>
