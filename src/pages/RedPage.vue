<template>
    <section class="colour-page has-background-danger">
        <div class="colour-card card">
            <div class="card-content">
                <p class="title has-text-white has-text-centered">Red</p>
            </div>
        </div>
    </section>
</template>

<style scoped>
.colour-page {
    display: flex;
    align-items: center;
    justify-content: center;
    height: calc(100vh - 52px);
    /* full height minus navbar */
    width: 100%;
}

.colour-card {
    width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    background: transparent;
    box-shadow: none;
}

.title {
    font-size: 15vw;
    font-weight: 900;
    letter-spacing: 0.05em;
    text-shadow: 0 4px 24px rgba(0, 0, 0, 0.25);
}
</style>