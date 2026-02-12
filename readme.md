# mi pagina "gymaesthe"
/*css*/
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    background-color: #0d0d0d;
    color: #f5f5f5;
    font-family: 'Montserrat', sans-serif;
}

/* NAV */

nav {
    display: flex;
    justify-content: space-between;
    padding: 20px 60px;
}

nav ul {
    display: flex;
    list-style: none;
    gap: 30px;
}

nav li {
    cursor: pointer;
}

.logo {
    font-weight: 700;
    letter-spacing: 4px;
}
/*____________________________________________________*/
.svg-button {
    display: grid;
    grid-template-columns: 1, 1fr;
    justify-content: center;
    align-items: center;
}
.button {
    width: 110px;
    height: 40px;
    display: flex;
    align-items: center;
    justify-content: flex-start;
    gap: 10px;
    background-color: #1f1f1f;
    border-radius: 30px;
    color: white;
    font-weight: 600;
    border: none;
    position: relative;
    cursor: pointer;
    transition-duration: 0.2s;
    box-shadow: 5px 5px 10px rgba(0, 0, 0, 0.116);
    padding-left: 8px;
    transition-duration: 0.5s;
}

.svgIcon {
    height: 25px;
    transition-duration: 1.5s;
}

.bell path {
    fill: rgb(19, 19, 19);
}

.button:hover {
    background-color: #ff4d00;
    transition-duration: 0.5s;
}

.button:active {
    transform: scale(0.97);
    transition-duration: 0.2s;
}

.button:hover .svgIcon {
    transform: rotate(250deg);
    transition-duration: 1.5s;
}

/*_______________________________________________________*/

/* HERO */

.hero {
    height: 90vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.hero h1 {
    font-size: 60px;
    letter-spacing: 10px;
}

.hero p {
    margin: 20px 0;
    font-size: 20px;
}

.hero button {
    padding: 12px 30px;
    border: 2px solid #ff4d00;
    background: transparent;
    color: white;
    cursor: pointer;
    transition: 0.3s;
}

.hero button:hover {
    background-color: #ff4d00;
}

/* COLLECTIONS */

.collections {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    padding: 60px;
    gap: 20px;
}

.box {
    background: #1f1f1f;
    height: 250px;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 22px;
    transition: 0.3s;
}

.box:hover {
    background-color: #ff4d00;
}

/* PHILOSOPHY */

.philosophy {
    text-align: center;
    padding: 100px 20px;
}

.philosophy span {
    color: #ff4d00;
}

/* FOOTER */

footer {
    text-align: center;
    padding: 30px;
    background-color: #1f1f1f;
}
/* html*/
<!doctype html>
<html lang="es">
    <head>
        <meta charset="UTF-8" />
        <title>GYMAESTHE</title>
        <link rel="stylesheet" href="gym.css" />
        <link rel="shortcut icon" href="favicon.ico" type="image/x-icon" />
        <link
            href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap"
            rel="stylesheet"
        />
    </head>
    <body>
        <header>
            <nav>
                <div class="logo">GYMAESTHE</div>
                <ul>
                    <li>Shop</li>
                    <li>About</li>
                    <li>Contact</li>
                </ul>
            </nav>
        </header>
        <section class="svg-button">
            <div>
                <!-- From Uiverse.io by vinodjangid07 -->
                <button class="button">
                    <svg
                        class="svgIcon"
                        viewBox="0 0 512 512"
                        height="1em"
                        xmlns="http://www.w3.org/2000/svg"
                    >
                        <path
                            d="M256 512A256 256 0 1 0 256 0a256 256 0 1 0 0 512zm50.7-186.9L162.4 380.6c-19.4 7.5-38.5-11.6-31-31l55.5-144.3c3.3-8.5 9.9-15.1 18.4-18.4l144.3-55.5c19.4-7.5 38.5 11.6 31 31L325.1 306.7c-3.2 8.5-9.9 15.1-18.4 18.4zM288 256a32 32 0 1 0 -64 0 32 32 0 1 0 64 0z"
                        ></path>
                    </svg>
                    Explore
                </button>
            </div>
        </section>
        <section class="hero">
            <h1>GYMAESTHE</h1>
            <p>Built Different.</p>
            <button>Shop Now</button>
        </section>

        <section class="collections">
            <div class="box">Oversize</div>
            <div class="box">Performance</div>
            <div class="box">Essentials</div>
        </section>

        <section class="philosophy">
            <h2><span>Discipline</span> creates aesthetics.</h2>
        </section>
        <footer>
            <p>© 2026 GYMAESTHE</p>
        </footer>
    </body>
</html>
