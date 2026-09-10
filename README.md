# meu-blog-tech
/* =========================
   RESET
========================= */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    background: #faf9f7;
    color: #222;
    line-height: 1.6;
}

a {
    text-decoration: none;
    color: inherit;
}

button,
input,
textarea {
    font-family: inherit;
}


/* =========================
   CONTAINER
========================= */

.container {
    width: min(1100px, 90%);
    margin: 0 auto;
}


/* =========================
   HEADER
========================= */

.header {
    background: #ffffff;
    border-bottom: 1px solid #eeeeee;
    position: sticky;
    top: 0;
    z-index: 100;
}

.nav {
    height: 75px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.logo {
    font-size: 1.7rem;
    font-weight: 800;
    color: #222;
}

.logo span {
    color: #7c3aed;
}

nav {
    display: flex;
    gap: 30px;
}

nav a {
    color: #555;
    font-size: 0.95rem;
    transition: 0.3s;
}

nav a:hover {
    color: #7c3aed;
}


/* =========================
   HERO
========================= */

.hero {
    padding: 100px 0;
    background:
        radial-gradient(
            circle at top right,
            #e9ddff,
            transparent 40%
        ),
        #faf9f7;
}

.hero-content {
    display: grid;
    grid-template-columns: 1.4fr 1fr;
    gap: 70px;
    align-items: center;
}

.tag {
    color: #7c3aed;
    font-size: 0.8rem;
    font-weight: 800;
    letter-spacing: 2px;
    margin-bottom: 15px;
}

.hero h1 {
    max-width: 700px;
    font-size: clamp(2.5rem, 6vw, 4.5rem);
    line-height: 1.05;
    margin-bottom: 25px;
}

.hero-text {
    max-width: 600px;
    color: #666;
    font-size: 1.1rem;
    margin-bottom: 35px;
}

.button {
    display: inline-block;
    background: #7c3aed;
    color: white;
    padding: 14px 25px;
    border-radius: 8px;
    font-weight: bold;
    transition: 0.3s;
}

.button:hover {
    background: #6025c5;
    transform: translateY(-2px);
}

.hero-card {
    min-height: 350px;
    padding: 45px;
    border-radius: 25px;
    color: white;

    display: flex;
    flex-direction: column;
    justify-content: center;

    background: linear-gradient(
        135deg,
        #7c3aed,
        #a855f7
    );

    box-shadow: 0 25px 60px rgba(124, 58, 237, 0.25);
}

.hero-card span {
    font-size: 3rem;
    margin-bottom: 20px;
}

.hero-card h2 {
    font-size: 2rem;
    margin-bottom: 15px;
}

.hero-card p {
    color: #eee;
}


/* =========================
   ARTIGOS
========================= */

.articles {
    padding: 100px 0;
    background: white;
}

.section-title {
    text-align: center;
    max-width: 650px;
    margin: 0 auto 55px;
}

.section-title h2 {
    font-size: 2.7rem;
    margin-bottom: 10px;
}

.section-title > p:last-child {
    color: #777;
}

.article-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 25px;
}

.article-card {
    overflow: hidden;
    background: #fff;
    border: 1px solid #eeeeee;
    border-radius: 15px;
    transition: 0.3s;
}

.article-card:hover {
    transform: translateY(-7px);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.08);
}

.article-image {
    height: 200px;
    display: flex;
    align-items: center;
    justify-content: center;
}

.article-image span {
    color: white;
    font-size: 3rem;
    font-weight: bold;
    opacity: 0.8;
}

.image-one {
    background: linear-gradient(135deg, #7c3aed, #c084fc);
}

.image-two {
    background: linear-gradient(135deg, #0ea5e9, #38bdf8);
}

.image-three {
    background: linear-gradient(135deg, #f97316, #facc15);
}

.article-content {
    padding: 25px;
}

.category {
    color: #7c3aed;
    font-size: 0.8rem;
    font-weight: bold;
    text-transform: uppercase;
    margin-bottom: 10px;
}

.article-content h3 {
    font-size: 1.35rem;
    line-height: 1.3;
    margin-bottom: 15px;
}

.article-content > p:not(.category) {
    color: #777;
    font-size: 0.95rem;
    margin-bottom: 20px;
}

.article-content a {
    color: #7c3aed;
    font-weight: bold;
}


/* =========================
   SOBRE
========================= */

.about {
    padding: 100px 0;
    background: #f3efff;
}

.about-content {
    display: grid;
    grid-template-columns: 0.8fr 1.2fr;
    gap: 70px;
    align-items: center;
}

.about-box {
    height: 350px;
    border-radius: 25px;

    display: flex;
    align-items: center;
    justify-content: center;

    background: linear-gradient(
        135deg,
        #7c3aed,
        #c084fc
    );

    box-shadow: 0 20px 50px rgba(124, 58, 237, 0.2);
}

.about-box span {
    font-size: 6rem;
}

.about h2 {
    font-size: 2.8rem;
    line-height: 1.15;
    margin-bottom: 25px;
}

.about p:not(.tag) {
    color: #666;
    margin-bottom: 15px;
}


/* =========================
   CONTATO
========================= */

.contact {
    padding: 100px 0;
    background: white;
}

.contact-form {
    max-width: 750px;
    margin: 0 auto;
}

.form-row {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 15px;
}

.contact-form input,
.contact-form textarea {
    width: 100%;
    padding: 16px;
    margin-bottom: 15px;

    border: 1px solid #ddd;
    border-radius: 8px;

    outline: none;
    font-size: 1rem;

    transition: 0.3s;
}

.contact-form input:focus,
.contact-form textarea:focus {
    border-color: #7c3aed;
    box-shadow: 0 0 0 3px rgba(124, 58, 237, 0.1);
}

.contact-form textarea {
    resize: vertical;
}

.contact-form button {
    border: none;
    background: #7c3aed;
    color: white;
    padding: 15px 25px;
    border-radius: 8px;

    font-size: 1rem;
    font-weight: bold;

    cursor: pointer;
    transition: 0.3s;
}

.contact-form button:hover {
    background: #6025c5;
}


/* =========================
   FOOTER
========================= */

.footer {
    background: #17121f;
    color: #aaa;
    padding: 30px 0;
}

.footer-content {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 20px;
}

.footer a {
    margin-left: 20px;
    transition: 0.3s;
}

.footer a:hover {
    color: white;
}


/* =========================
   RESPONSIVIDADE
========================= */

@media (max-width: 800px) {

    .nav {
        height: auto;
        padding: 20px 0;
        flex-direction: column;
        gap: 15px;
    }

    nav {
        gap: 15px;
        flex-wrap: wrap;
        justify-content: center;
    }

    .hero {
        padding: 70px 0;
    }

    .hero-content {
        grid-template-columns: 1fr;
        gap: 40px;
    }

    .hero-card {
        min-height: 250px;
    }

    .article-grid {
        grid-template-columns: 1fr;
    }

    .about-content {
        grid-template-columns: 1fr;
        gap: 40px;
    }

    .about-box {
        height: 250px;
    }

    .form-row {
        grid-template-columns: 1fr;
        gap: 0;
    }

    .footer-content {
        flex-direction: column;
        text-align: center;
    }

    .footer a {
        margin: 0 8px;
    }
}
