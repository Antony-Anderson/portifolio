<template>
    <div class="profile-container">
        <div class="profile-info">
            <h1 class="profile-name">Antony Anderson Vieira Seixas</h1>
            <h2 class="profile-title">Desenvolvedor Full Stack</h2>
            <hr>
            <p class="profile-description">
                Durante o período de mais de um ano, mergulhei profundamente no mundo da programação e adquiri uma sólida base em diversas tecnologias.
            </p>
            <p class="profile-description">
                Meu objetivo é contribuir com soluções inovadoras e eficientes, seja em front-end, back-end, ou no desenvolvimento de aplicativos móveis.
            </p>
            <hr>
        </div>
        <img src="../assets/images/perfil.jpeg" alt="Foto de Antony" class="profile-img">
    </div>
</template>

<style scoped>
    .profile-container {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
        height: 100vh;
        padding: 20px;
        gap: 20px;
    }

    .profile-info {
        flex: 1;
        max-width: 50%;
        text-align: left;
    }

    .profile-img {
        flex: 1;
        max-width: 30vw;
        height: auto;
        border-radius: 10%;
        object-fit: cover;
    }

    .profile-name {
        font-size: 2.5rem;
        margin: 10px 0;
        font-family: 'Courier New', Courier, monospace;
        font-weight: 700;
        color: white;
    }

    .profile-title {
        color: white;
        font-size: 1.8rem;
        margin: 10px 0;
        font-family: 'Copperplate', fantasy;
    }

    .profile-description {
        font-size: 1.2rem;
        color: rgb(168, 160, 160);
        margin: 10px 0;
        line-height: 1.6;
        text-align: justify;
    }

    @media (max-width: 768px) {
        .profile-container {
            flex-direction: column;
            align-items: center;
            height: auto;
            text-align: center;
        }

        .profile-info {
            max-width: 100%;
        }

        .profile-img {
            max-width: 80vw;
            margin-top: 20px;
        }

        .profile-name {
            font-size: 2rem;
        }

        .profile-title {
            font-size: 1.5rem;
        }

        .profile-description {
            font-size: 1rem;
        }
    }

    @media (max-width: 480px) {
        .profile-name {
            font-size: 1.5rem;
        }

        .profile-title {
            font-size: 1.2rem;
        }

        .profile-description {
            font-size: 0.9rem;
        }
    }
</style>
