<section>
    <article>
        <h1>Was wir machen</h1>
        <div class="services" id="services">

            <div class="service">
                <div class="beschreibung grafikdesign">
                    <h3>Grafikdesign</h3>
                    <p>Wir bringen deine Marke zum Leben - von Konzept bis Umsetzung. Ideen werden durch Farben, Formen, Typografie und Bilder zu ansprechenden Designs.</p>
                </div>
            </div>
                
            <div class="service">
                <div class="beschreibung webdesign">
                    <h3>Webdesign</h3>
                    <p>Wir verwandeln deine Vision in eine Online-Präsenz, die nicht nur ästhetisch ansprechend ist, sondern mit deinem Look & Feel und einer intuitiven Nutzerführung punktet.</p>
                </div>
            </div>

            <div class="service">
                <div class="beschreibung branddesign">
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
        height: 300px;
        width: 330px;
        border-radius: 20px;
        display: flex;
        flex-direction: column;
        gap: 1rem;
        justify-content: center;
        align-items: center;
        cursor: pointer;
        background-color: var(--secondary);
    }
    

    .beschreibung{
        padding: 35px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        gap: 1rem;
    }

    .beschreibung h3{
        font-weight: 400;
    }


    .grafikdesign h3{
        color: var(--green);
        text-shadow: 0px 0px 30px var(--green);
    }

    .webdesign h3{
        color: var(--blue);
        text-shadow: 0px 0px 30px var(--blue);
    }

    .branddesign h3{
        color: var(--primary);
        text-shadow: 0px 0px 30px var(--primary);
    }

    .beschreibung p{
        color: var(--gray);
    }
    



</style>