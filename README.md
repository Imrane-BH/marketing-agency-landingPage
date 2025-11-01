# marketing-agency-landingPage
This website for an online marketing agency, it is responsive for all devices and clean code
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cloudline Media</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <a href="#hero" class="logo">Cloudline Media</a>
    </header>
    <section id="hero" class="hero">
        <p>"Welcome to Cloudline Media, where creativity meets strategy. We build standout brands, craft data-driven campaigns, and deliver high-converting websites that grow with you."</p>
        <img src="images/hero.jpg" alt="marketing img">
    </section>
    <section class="services">
        <h2>services</h2>
        <p>“We specialize in brand identity, content strategy, performance marketing, and web development. From concept to execution, we help you attract, engage, and convert your audience.”</p>
        <div class="cards">
            <div class="card">
                <strong>web development</strong>
            </div>
            <div class="card">
                <strong>performance marketing</strong>
            </div> 
            <div class="card">
                <strong>brand identity</strong>
            </div>
        </div>
    </section>
    <h2 class="review-h2">Our customer reviews</h2>
    <section class="reviews">
        <div class="review">
            <img src="images/fman.jpg" alt="">
            <p>“Creative, data-driven, and on time. Our campaigns finally started delivering real ROI.”</p>
        </div>
        <div class="review">
            <img src="images/sman.jpg" alt="">
            <p>“Amazing team that truly listens. Our brand story felt clearer and more compelling after just one brief.”</p>
        </div>
        <div class="review">
            <img src="images/tman.jpg" alt="">
            <p>“Reliable and proactive. Transparent reporting and measurable results—we’re ROI-positive month after month.”</p>
        </div>
    </section>
    <section class="contact">
        <h2>contact us</h2>
        <form action="">
            <input type="text" placeholder="enter your name">
            <input type="tel" placeholder="enter your phone number">
            <input type="email" placeholder="enter your email">
            <input type="password" placeholder="enter your password">
            <input type="submit" value="submit" class="btn">
        </form>
    </section>
</body>
</html>
:root {
    --main-color: #1e3a8a; 
    --secondary-color: #4c1d95; 
    --accent-color: #2563eb; 
    --bg-gradient-start: #1e3a8a;
    --bg-gradient-end: #7c3aed; 
    --brand-gradient: linear-gradient(135deg, var(--bg-gradient-start) 0%, var(--bg-gradient-end) 100%);
    }

    *{
        margin: 0;
        padding: 0;
        font-family: sans-serif;
    }

    header{
        width: 90vw;
        display: flex;
        background: white;
    }

    header .logo{
        text-decoration: none;
        color: var(--secondary-color);
        font-size: xx-large;
        margin: 20px 30px;
        font-weight: 600;
        letter-spacing: 1px;
    }

    .hero p{
        width: 350px;
        margin: 20px 40px;
        font-weight: 600;
        line-height: 20px;
        letter-spacing: 1px;
        color: var(--main-color);
    }

    .hero img{
        width: 300px;
        margin: 20px 30px;
        border-radius: 5px;
        box-shadow: 0 0 20px var(--secondary-color);
    }

    .services p{
        width: 350px;
        margin: 20px 40px;
        font-weight: 600;
        line-height: 20px;
        letter-spacing: 1px;
        color: var(--main-color);
    }

    .services h2{
        color: var(--secondary-color);
        font-size: xx-large;
        font-weight: 500;
        margin: 20px 40px;
        text-transform: capitalize;
        letter-spacing: 1px;

    }

    .cards{
        width: 90%;
        display: flex;
        justify-content: space-evenly;
        flex-wrap: wrap;
        margin: 10px auto;
    }

    .cards .card{
        width: 250px;
        margin: 20px auto;
        height: 150px;
        text-align: center;
        display: flex;
        align-items: center;
        justify-content: center;
        background-color: var(--bg-gradient-end);
        border-radius: 10px;
        transition: .3s;
    }

    .cards .card strong{
        font-size: 1.3rem;
        color: white;
    }

    .cards .card:hover{
        transform: scale(120%) translateY(-20px);
    }

    @media (min-width:550px){
        .hero{
            display: flex;
            justify-content: space-between;
        }

        .hero p{
            width: 200px;
        }

        .hero img{
            min-width: 200px;
            min-height: 200px;
            margin: 10px auto;
        }
    }

    .reviews {
        width: 90%;
        display: flex;
        justify-content: space-evenly;
        flex-wrap: wrap;
        margin: 10px auto;
    }

    .review-h2{
        color: var(--secondary-color);
        font-size: xx-large;
        font-weight: 500;
        margin: 20px 40px;
        text-transform: capitalize;
        letter-spacing: 1px;
    }

    .reviews .review{
        display: block;
        width: 250px;
        height: 300px;
    }

    .reviews .review img{
        width: 90%;
        border-radius: 8px;
    }

    .reviews .review p{
        margin: 15px 10px;
    }
    .contact h2{
        color: var(--secondary-color);
        font-size: xx-large;
        font-weight: 500;
        margin: 20px 40px;
        text-transform: capitalize;
        letter-spacing: 1px;
    }

    .contact form{
        min-width: 250px;
        max-width: 350px;
        display: block;
        height: 300px;
        margin: auto;
    }

    .contact form input{
        width: 80%;
        height: 30px;
        margin: 10px auto;
        padding: 0px 5px;
        border-radius: 20px;
        border: solid 2px var(--bg-gradient-end);
    }

    .contact form .btn{
        color: white;
        font-size: 1.3rem;
        letter-spacing: 2px;
        transition: .2s;
        background: var(--bg-gradient-end);
    }

    .contact form .btn:hover{
        transform: scale(120%);
    }
