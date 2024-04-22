<section>
    <article>
        <h1>Unsere Services</h1>
        <div class="services" id="services">

            <div class="service">
                <img src="images/grafik-design.jpg" alt="">
                <div class="beschreibung">
                    <h3>Grafikdesign</h3>
                    <p>Wir bringen deine Marke zum Leben - von Konzept bis Umsetzung. Ideen werden durch Farben, Formen, Typografie und Bilder zu ansprechenden Designs.</p>
                </div>
            </div>
                
            <div class="service">
                <img src="images/web-design.jpg" alt="">
                <div class="beschreibung">
                    <h3>Webdesign</h3>
                    <p>Wir verwandeln deine Vision in eine Online-Präsenz, die nicht nur ästhetisch ansprechend ist, sondern mit deinem Look & Feel und einer intuitiven Nutzerführung punktet.</p>
                </div>
            </div>

            <div class="service">
                <img src="images/brand-design.jpg" alt="">
                <div class="beschreibung">
                    <h3>Brand Design</h3>
                    <p>Wir verleihen deiner Marke mit einem Brand Design ein einheitliches Erscheinungsbild und eine ganzheitliche visuelle Präsenz. Grafikdesign und Webdesign im Komplettpaket.</p>
                </div>
            </div>

        </div>
    </article>
</section>

<style>
    section{
        padding: 2rem 0rem;
        width: 100%;
        display: flex;
    }

    article{
        width: 1120px;
        margin: 0 auto;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        gap: 3rem;
    }

    h1{
        font-size: 36px;
    }


    .services{
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: space-between;

    }

    .service{
    box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px;
        height: 450px;
        width: 300px;
        border-radius: 0.5rem;
        display: flex;
        flex-direction: column;
        gap: 1rem;
        align-items: center;
        overflow: hidden;
        transition: all 0.2s;
        cursor: pointer;
    }
    
    .service:hover{
        scale: 1.03;
    }

    .service img{
        height: 200px;
        width: 100%;
        object-fit: cover;
    }

    .beschreibung{
        color: white;
        padding: 0rem 1rem;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        gap: 0.5rem;
    }

    .beschreibung p{
        text-align: center;
        color: var(--secondary);
    }

    h3{
        color: var(--primary);
    }
</style>