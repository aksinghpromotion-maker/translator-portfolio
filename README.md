# translator-portfolio
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Translator Portfolio</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <div class="container">
            <a class="navbar-brand" href="index.html">Translator Portfolio</a>
            <ul class="navbar-nav ms-auto">
                <li class="nav-item"><a class="nav-link" href="index.html">Home</a></li>
                <li class="nav-item"><a class="nav-link" href="portfolio.html">Portfolio</a></li>
                <li class="nav-item"><a class="nav-link" href="contact.html">Contact</a></li>
            </ul>
            <select id="language-selector" class="form-select ms-3" style="width: auto;">
                <option value="en">English</option>
                <option value="es">Español</option>
                <option value="fr">Français</option>
            </select>
        </div>
    </nav>

    <div class="container mt-5">
        <h1 id="home-title">Welcome to My Translation Portfolio</h1>
        <p id="home-description">I am a professional translator specializing in English, Spanish, and French. Explore my samples and get in touch for your projects.</p>
        <a href="portfolio.html" class="btn btn-primary">View Portfolio</a>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <script>
        const translations = {
            en: {
                title: "Welcome to My Translation Portfolio",
                description: "I am a professional translator specializing in English, Spanish, and French. Explore my samples and get in touch for your projects."
            },
            es: {
                title: "Bienvenido a Mi Portafolio de Traducción",
                description: "Soy un traductor profesional especializado en inglés, español y francés. Explora mis muestras y ponte en contacto para tus proyectos."
            },
            fr: {
                title: "Bienvenue sur Mon Portefeuille de Traduction",
                description: "Je suis un traducteur professionnel spécialisé en anglais, espagnol et français. Explorez mes échantillons et contactez-moi pour vos projets."
            }
        };

        document.getElementById('language-selector').addEventListener('change', function() {
            const lang = this.value;
            document.getElementById('home-title').textContent = translations[lang].title;
            document.getElementById('home-description').textContent = translations[lang].description;
        });
    </script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio - Translator</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <div class="container">
            <a class="navbar-brand" href="index.html">Translator Portfolio</a>
            <ul class="navbar-nav ms-auto">
                <li class="nav-item"><a class="nav-link" href="index.html">Home</a></li>
                <li class="nav-item"><a class="nav-link" href="portfolio.html">Portfolio</a></li>
                <li class="nav-item"><a class="nav-link" href="contact.html">Contact</a></li>
            </ul>
            <select id="language-selector" class="form-select ms-3" style="width: auto;">
                <option value="en">English</option>
                <option value="es">Español</option>
                <option value="fr">Français</option>
            </select>
        </div>
    </nav>

    <div class="container mt-5">
        <h1 id="portfolio-title">My Translation Samples</h1>
        <p id="portfolio-description">Here are some real examples of my work. Click to expand.</p>
        
        <div class="accordion" id="samplesAccordion">
            <div class="accordion-item">
                <h2 class="accordion-header">
                    <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#sample1">English to Spanish: Business Email</button>
                </h2>
                <div id="sample1" class="accordion-collapse collapse show" data-bs-parent="#samplesAccordion">
                    <div class="accordion-body">
                        <strong>Original (English):</strong> "Dear Sir, We are pleased to inform you that your order has been processed and will be shipped within 24 hours."<br>
                        <strong>Translation (Spanish):</strong> "Estimado Señor, Nos complace informarle que su pedido ha sido procesado y será enviado dentro de 24 horas."
                    </div>
                </div>
            </div>
            <div class="accordion-item">
                <h2 class="accordion-header">
                    <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#sample2">English to French: Marketing Copy</button>
                </h2>
                <div id="sample2" class="accordion-collapse collapse" data-bs-parent="#samplesAccordion">
                    <div class="accordion-body">
                        <strong>Original (English):</strong> "Discover our innovative solutions that save time and money for your business."<br>
                        <strong>Translation (French):</strong> "Découvrez nos solutions innovantes qui économisent du temps et de l'argent pour votre entreprise."
                    </div>
                </div>
            </div>
            <div class="accordion-item">
                <h2 class="accordion-header">
                    <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#sample3">Spanish to English: Legal Document</button>
                </h2>
                <div id="sample3" class="accordion-collapse collapse" data-bs-parent="#samplesAccordion">
                    <div class="accordion-body">
                        <strong>Original (Spanish):</strong> "El contrato se considera válido una vez firmado por ambas partes."<br>
                        <strong>Translation (English):</strong> "The contract is considered valid once signed by both parties."
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <script>
        const translations = {
            en: {
                title: "My Translation Samples",
                description: "Here are some real examples of my work. Click to expand."
            },
            es: {
                title: "Mis Muestras de Traducción",
                description: "Aquí hay algunos ejemplos reales de mi trabajo. Haz clic para expandir."
            },
            fr: {
                title: "Mes Échantillons de Traduction",
                description: "Voici quelques exemples réels de mon travail. Cliquez pour développer."
            }
        };

        document.getElementById('language-selector').addEventListener('change', function() {
            const lang = this.value;
            document.getElementById('portfolio-title').textContent = translations[lang].title;
            document.getElementById('portfolio-description').textContent = translations[lang].description;
        });
    </script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact - Translator</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <div class="container">
            <a class="navbar-brand" href="index.html">Translator Portfolio</a>
            <ul class="navbar-nav ms-auto">
                <li class="nav-item"><a class="nav-link" href="index.html">Home</a></li>
                <li class="nav-item"><a class="nav-link" href="portfolio.html">Portfolio</a></li>
                <li class="nav-item"><a class="nav-link" href="contact.html">Contact</a></li>
            </ul>
            <select id="language-selector" class="form-select ms-3" style="width: auto;">
                <option value="en">English</option>
                <option value="es">Español</option>
                <option value="fr">Français</option>
            </select>
        </div>
    </nav>

    <div class="container mt-5">
        <h1 id="contact-title">Get in Touch</h1>
        <p id="contact-description">Ready to start your translation project? Contact me below.</p>
        <form>
            <div class="mb-3">
                <label for="name" class="form-label" id="name-label">Name</label>
                <input type="text" class="form-control" id="name">
            </div>
            <div class="mb-3">
                <label for="email" class="form-label" id="email-label">Email</label>
                <input type="email" class="form-control" id="email">
            </div>
            <div class="mb-3">
                <label for="message" class="form-label" id="message-label">Message</label>
                <textarea class="form-control" id="message" rows="4"></textarea>
            </div>
            <button type="submit" class="btn btn-primary" id="submit-btn">Send Message</button>
        </form>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <script>
        const translations = {
            en: {
                title: "Get in Touch",
                description: "Ready to start your translation project? Contact me below.",
                name: "Name",
                email: "Email",
                message: "Message",
                submit: "Send Message"
            },
            es: {
                title: "Ponte en Contacto",
                description: "¿Listo para iniciar tu proyecto de traducción? Contáctame a continuación.",
                name: "Nombre",
                email: "Correo Electrónico",
                message: "Mensaje",
                submit: "Enviar Mensaje"
            },
            fr: {
                title: "Entrer en Contact",
                description: "Prêt à commencer votre projet de traduction ? Contactez-moi ci-dessous.",
                name: "Nom",
                email: "Email",
                message: "Message",
                submit: "Envoyer le Message"
            }
        };

        document.getElementById('language-selector').addEventListener('change', function() {
            const lang = this.value;
            document.getElementById('contact-title').textContent = translations[lang].title;
            document.getElementById('contact-description').textContent = translations[lang].description;
            document.getElementById('name-label').textContent = translations[lang].name;
            document.getElementById('email-label').textContent = translations[lang].email;
            document.getElementById('message-label').textContent = translations[lang].message;
            document.getElementById('submit-btn').textContent = translations[lang].submit;
        });
    </script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    background-color: #f8f9fa;
}

.navbar-brand {
    font-weight: bold;
}

.container {
    max-width: 800px;
}

.accordion-button {
    font-weight: bold;
}
