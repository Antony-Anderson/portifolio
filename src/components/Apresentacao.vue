<template>
    <div class="profile-container">
        <div class="profile-info">
            <h1 class="profile-name">Antony Anderson Vieira Seixas</h1>
            <h2 class="profile-title">Desenvolvedor Full Stack</h2>
            <hr>
            <p class="profile-description">
                Como programador full stack apaixonado por tecnologia e inovação, tenho 19 anos e uma sólida experiência em Laravel, PHP, Vue.js, JavaScript, TypeScript, React Native e banco de dados. Minha abordagem para o desenvolvimento de software é marcada por um compromisso inabalável com a qualidade e a eficiência, sempre buscando criar soluções elegantes e funcionais.            
            </p>
            <p class="profile-description">
                Trabalhar em equipe é uma das minhas maiores fortalezas. Valorizo a colaboração e a comunicação aberta, acreditando que um bom projeto é fruto de uma sinergia entre profissionais dedicados. Estou sempre disposto a compartilhar conhecimentos e aprender com os outros, o que contribui para um ambiente de trabalho harmonioso e produtivo.            
            </p>
            <p class="profile-description">
                Minha proatividade e espírito autodidata me permitem enfrentar desafios com confiança e buscar constantemente novas habilidades e tecnologias. Tenho um forte desejo de aprimorar minhas competências e estou sempre atualizado com as tendências mais recentes do setor.
            </p>
            <p class="profile-description">
                Estou pronto para trazer minha experiência e entusiasmo para sua equipe, contribuindo para o desenvolvimento de soluções inovadoras e impactantes.
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
