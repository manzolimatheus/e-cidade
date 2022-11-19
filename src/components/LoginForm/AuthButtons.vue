<template>
    <div class="buttons">
        <button class="button-danger" disabled>
            <ion-icon name="logo-google"></ion-icon>
            Entrar com o Google
        </button>
        <button class="button-safe" disabled>
            <ion-icon name="logo-facebook"></ion-icon>
            Entrar com o Facebook
        </button>
        <button disabled>
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/11/Gov.br_logo.svg/1200px-Gov.br_logo.svg.png" alt="Logo Gov.br" width="50">
            Entrar com o Gov.br
        </button>
    </div>
</template>

<script>
    export default {
        name: 'AuthButtons'
    }
</script>

<style>

    .buttons {
        display: flex;
        flex-direction: column;
        gap: 10px;
        width: 100%;
    }

    .buttons button {
        padding: 3%;
        border-radius: 20px;
        font-size: 14pt;
        text-align: left;
    }

</style>