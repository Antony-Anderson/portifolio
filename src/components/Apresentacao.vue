<template>
    <div class="main-container">
        <div class="profile-container">
            <div class="profile-info">
                <h1 class="profile-name">Antony Anderson Vieira Seixas</h1>
                <h2 class="profile-title">Desenvolvedor Full Stack</h2>
                <hr>
                <p class="profile-description">
                    Sou desenvolvedor Full Stack com experiência prática em PHP (Laravel e Symfony), Vue.js, JavaScript/TypeScript e MySQL.
                </p>
                <p class="profile-description">
                    Atuo no desenvolvimento de aplicações web completas, criando APIs REST, implementando regras de negócio, autenticação, CRUDs complexos e filtros avançados.                </p>
                <p class="profile-description">
                    Tenho foco em código limpo, organização do projeto e entrega consistente. Aqui no portfólio você encontra projetos reais com link e demonstração.                </p>
                <hr>
            </div>
            <img src="../assets/images/perfil.jpeg" alt="Foto de Antony" class="profile-img">
        </div>
    </div>
</template>

<script>
    export default {
        computed: {
            idade() {
                const nascimento = new Date(2005, 3, 2)
                const hoje = new Date()

                let idade = hoje.getFullYear() - nascimento.getFullYear()

                const jaFezAniversario =
                    hoje.getMonth() > nascimento.getMonth() ||
                    (hoje.getMonth() === nascimento.getMonth() &&
                    hoje.getDate() >= nascimento.getDate())

                if (!jaFezAniversario) idade--

                return idade
            }
        }
    }
</script>


<style scoped>
    .main-container {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        min-height: 100vh;
        padding: 20px;
        box-sizing: border-box;
    }

    .profile-container {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
        width: 100%;
        max-width: 1200px; 
        margin: 20px 0;
        box-sizing: border-box;
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
        color: #d9dce3;
    }

    .profile-title {
        color: #d9dce3;
        font-size: 1.8rem;
        margin: 10px 0;
        font-family: 'Copperplate', fantasy;
    }

    .profile-description {
        font-size: 1.2rem;
        color: rgb(201, 194, 194);
        margin: 10px 0;
        line-height: 1.6;
        text-align: justify;
    }

    @media (max-width: 768px) {
        .profile-container {
            flex-direction: column;
            align-items: center;
            width: 100%;
            margin: 10px 0; 
        }

        .profile-info {
            max-width: 100%;
        }

        .profile-img {
            max-width: 80vw;
            margin-top: 20px;
            object-fit: contain; 
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
        .profile-img {
            max-width: 90vw;
        }

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
