<template>
    <div>
        <h1>Formações e Cursos</h1>
        <div id="carouselExampleControls" class="carousel slide" data-bs-ride="carousel">
            <div class="carousel-inner">
                <!-- Slide 1 -->
                <div class="carousel-item active">
                    <div class="row">
                        <div class="col">
                            <a href="https://cursos.alura.com.br/user/antony01anderson/degree-linguagem-php-v597958-597958/certificate">
                                <img src="../assets/images/certificados/php.png" class="d-block w-100" alt="Imagem 1">
                            </a>
                        </div>
                        <div class="col">
                            <a href="https://cursos.alura.com.br/user/antony01anderson/degree-linguagem-php-v597958-597958/certificate">
                                <img src="../assets/images/certificados/php-verso.png" class="d-block w-100" alt="Imagem 2">
                            </a>
                        </div>
                    </div>
                </div>
                <!-- Slide 2 -->
                <div class="carousel-item">
                    <div class="row">
                        <div class="col">
                            <img src="../assets/images/certificados/logica.png" class="d-block w-100" alt="Imagem 3">
                        </div>
                        <div class="col">
                            <img src="../assets/images/certificados/logica-verso.png" class="d-block w-100" alt="Imagem 4">
                        </div>
                    </div>
                </div>
                <!-- Slide 3 -->
                <div class="carousel-item">
                    <div class="row">
                        <div class="col">
                            <img src="../assets/images/certificados/javascript.png" class="d-block w-100" alt="Imagem 5">
                        </div>
                        <div class="col">
                            <img src="../assets/images/certificados/javascript-verso.png" class="d-block w-100" alt="Imagem 6">
                        </div>
                    </div>
                </div>
                <!-- Slide 4 -->
                <div class="carousel-item">
                    <div class="row">
                        <div class="col">
                            <img src="../assets/images/certificados/laravel.png" class="d-block w-100" alt="Imagem 7">
                        </div>
                        <div class="col">
                            <img src="../assets/images/certificados/laravel-verso.png" class="d-block w-100" alt="Imagem 8">
                        </div>
                    </div>
                </div>
                <!-- Slide 5 -->
                <div class="carousel-item">
                    <div class="row">
                        <div class="col">
                            <img src="../assets/images/certificados/typescript.png" class="d-block w-100" alt="Imagem 9">
                        </div>
                        <div class="col">
                            <img src="../assets/images/certificados/typescript-verso.png" class="d-block w-100" alt="Imagem 10">
                        </div>
                    </div>
                </div>
                <!-- Slide 6 -->
                <div class="carousel-item">
                    <div class="row">
                        <div class="col">
                            <img src="../assets/images/certificados/vue.png" class="d-block w-100" alt="Imagem 11">
                        </div>
                        <div class="col">
                            <img src="../assets/images/certificados/vue-verso.png" class="d-block w-100" alt="Imagem 12">
                        </div>
                    </div>
                </div>
                <!-- Slide 7 -->
                <div class="carousel-item">
                    <div class="row">
                        <div class="col">
                            <img src="../assets/images/certificados/sql.png" class="d-block w-100" alt="Imagem 13">
                        </div>
                        <div class="col">
                            <img src="../assets/images/certificados/sql-verso.png" class="d-block w-100" alt="Imagem 14">
                        </div>
                    </div>
                </div>
                <!-- Slide 8 -->
                <div class="carousel-item">
                    <div class="row">
                        <div class="col">
                            <img src="../assets/images/certificados/javascript-cv.png" class="d-block w-100" alt="Imagem 15">
                        </div>
                        <div class="col">
                            <img src="../assets/images/certificados/javascript-cv.png" class="d-block w-100" alt="Imagem 16">
                        </div>
                    </div>
                </div>
            </div>

            <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Previous</span>
            </button>
            <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Next</span>
            </button>
        </div>
    </div>
</template>

<style scoped>
    h1 {
        color: white;
        margin-top: 30px;
        text-align: center;
        margin-bottom: 50px; /* Ajustado para menor espaçamento inferior */
    }

    .carousel-inner {
        max-width: 1200px; 
        height: 600px;
        margin: 0 auto;
        position: relative; /* Necessário para posicionar os botões corretamente */
    }

    .carousel-item {
        height: 100%; 
    }

    .carousel-item img {
        width: 100%;
        height: 100%; 
        object-fit: cover; 
    }

    .carousel-control-prev, .carousel-control-next {
        width: 5%; /* Ajuste a largura dos botões */
        top: 50%; /* Centraliza verticalmente os botões */
        transform: translateY(-50%); /* Ajusta a posição vertical dos botões */
    }

    .carousel-control-prev {
        left: 0;
    }

    .carousel-control-next {
        right: 0;
    }

    @media (max-width: 768px) {
        .carousel-control-prev, .carousel-control-next {
            width: 10%; /* Largura maior dos botões em telas menores */
        }
    }

    @media (max-width: 480px) {
        .carousel-control-prev, .carousel-control-next {
            width: 15%; /* Largura ainda maior dos botões em telas muito pequenas */
        }
    }
</style>
