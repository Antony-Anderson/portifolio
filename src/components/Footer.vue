<template>
    <footer class="footer">
        <div class="content">
            <h3 class="titulo">Precisa de um desenvolvedor?</h3>
            <a href="https://wa.me/75988152683" class="cta-link" target="_blank">
                <h1>Vamos trabalhar juntos →</h1>
            </a>
            <hr>
            <div class="footer-sections">
                <div class="contact-section">
                    <h3>Informações de contato</h3>
                    <p>Email: <a href="https://mail.google.com/mail/u/0/?tab=rm&ogbl#inbox?compose=DmwnWrRnXVNXZzhgFKpSsgwrhckfDfvSGtQHNSkRdFsSHmcfZtwhrzJQGrVQcPnldWPpRtNWlVGv" target="_blank">antony01anderson@gmail.com</a></p>
                    <p>Telefone: <a href="https://wa.me/75988152683" target="_blank">+55 75 98815-2683</a></p>
                </div>
                <div class="social-section">
                    <h3>Me siga</h3>
                    <div class="social-icons">
                        <a href="https://www.linkedin.com/in/antony-anderson-7238701bb/" target="_blank">
                            <i class="fa-brands fa-linkedin" style="color: #74C0FC;"></i>
                        </a>
                        <a href="https://github.com/Antony-Anderson" target="_blank">
                            <i class="fa-brands fa-github" style="color: #eef1f7;"></i>
                        </a>
                        <a href="https://wa.me/75988152683" target="_blank">
                            <i class="fa-brands fa-whatsapp" style="color: #1e7158;"></i>
                        </a>
                    </div>
                </div>
                <div class="availability-section">
                    <h3>Atual disponibilidade</h3>
                    <p>Aberto 24 horas, ficarei feliz em discutir novas oportunidades, entre em contato!</p>
                </div>
            </div>
        </div>
    </footer>
</template>

<style scoped>
    .footer {
        padding: 50px 20px;
        text-align: center;
        color: white;
    }

    h1 {
        font-size: 2em;
        margin-top: 20px;
        color: #fff;
        margin-bottom: 20px;
    }

    hr {
        margin-bottom: 50px;
        border: 0;
        border-top: 1px solid #555; /* Ajuste a cor do separador */
    }

    .titulo {
        color: #ff5733;
    }

    .footer-sections {
        display: flex;
        flex-wrap: wrap;
        gap: 20px; /* Adiciona espaço entre as seções */
        justify-content: center;
    }

    .contact-section, .social-section, .availability-section {
        flex: 1;
        min-width: 200px; /* Define um tamanho mínimo para as seções */
        margin: 10px;
    }

    h3 {
        font-size: 1.3em;
        margin-bottom: 20px;
    }

    .contact-section p, .availability-section p {
        margin: 10px 0;
    }

    .contact-section a {
        color: #ff5733;
        text-decoration: none;
    }

    .contact-section a:hover {
        text-decoration: underline;
    }

    .social-icons {
        margin: 20px 0;
    }

    .social-icons a {
        margin: 0 10px;
        display: inline-block;
        transition: transform 0.3s ease, opacity 0.3s ease;
    }

    .social-icons i {
        font-size: 2em;
    }

    .social-icons a:hover i {
        transform: scale(1.2);
        opacity: 0.8;
    }

    a.cta-link {
        text-decoration: none;
        display: inline-block;
    }

    a.cta-link h1 {
        color: #fff;
        transition: color 0.3s ease;
    }

    a.cta-link h1:hover {
        color: #ff5733;
        text-decoration: underline;
    }

    @media (max-width: 768px) {
        h1 {
            font-size: 1.8em;
        }

        .footer-sections {
            flex-direction: column;
            align-items: center;
        }

        .contact-section, .social-section, .availability-section {
            min-width: auto;
            margin: 10px 0;
        }

        .social-icons a {
            margin: 0 10px;
        }

        .social-icons i {
            font-size: 1.8em;
        }
    }

    @media (max-width: 480px) {
        h1 {
            font-size: 1.5em;
        }

        .footer-sections {
            padding: 0 10px;
        }

        .contact-section, .social-section, .availability-section {
            min-width: auto;
            margin: 5px 0;
        }

        .social-icons a {
            margin: 0 8px;
        }

        .social-icons i {
            font-size: 1.5em;
        }
    }
</style>
