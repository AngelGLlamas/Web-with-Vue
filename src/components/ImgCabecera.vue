<template>
    <div class="flex flex-h">
        <div class="flex flex-h">
            <img id="cabecera" class="relative limit-height" src="../assets/imgcabecera.jpg" alt="imagen principal">
            <div id="eslogan" class="absolute">
                <h1>Eslogan de la empresa</h1>
                <h2>Servicio principal </h2>
            </div> 
        </div>
    </div>
</template>

<style lang="scss">
    #cabecera {
        opacity: 0.6;
    }
    #eslogan{
        h1, h2{
            color:rgb(39, 39, 39);
        }
    }
</style>

