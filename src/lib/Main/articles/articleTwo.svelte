    <script lang="ts">
        import { locale } from "../../../utils/stores";
    </script>

    {#if $locale === 'es'}
        <div>
            <p>
                Me voy a otro lugar, llevo mi música, mi vida, una vez más.<br/>
				Ella no viene, <strong>ya no vendrá</strong>, la brisa suave y dulce me invita a volar,<br/>
				a volar.
            </p>
            <p>
                Ya no hay destino (<i>o lo olvidé?</i>), no sé si llegue a algún lugar alguna vez.<br/>
				Pero no importa, yo partiré.<br/>
				<i>[...]</i>
            </p>
            <p>
                Tomaré un café tranquilo, por ahí,<br/>
				recordaré que a veces <i>la vida es así.</i><br/>
				No es nada fácil,<br/>
				para nadie aquí.<br/>
            </p>
            <p>
                Sé que la vida se me pasa se te espero,<br/>
				por eso vivo yéndome a otro lugar.<br/>
				Sé que <strong>el amor cuando es con baile es verdadero</strong>,<br/>
				siempre pensé que estarías por aća<br/>
				para bailar.<br/>
            </p>
            <p>
                No es nada fácil dejar partir todo eso que creímos saber sobre vivir.<br>
                Son los detalles, los momentos, <i>quisiera no perder tu imagen con el tiempo.</i><br>
            </p>
            <p>
                Y <strong>la vida es compleja</strong>, lo sé<br/>
				yo ya <i>aprendí a no preguntar el por qué.</i><br/>
				Estás tan lejos, y yo también.<br/>
            </p>
            <p>
                Sé que <i>la vida se me pasa si te espero</i>,<br/>
				por eso vivo yéndome a otro lugar.<br/>
				Sé que el amor cuando es con baile es verdadero,<br/>
				<i>siempre pensé que estarías por aća</i><br/>
				para bailar.<br/>
            </p>
			<p>
                Ven, <strong>bailemos la noche los dos</strong> si esta historia ya tiene un destino<br>
				no sea cosa que al amanecer nos quedemos sin lo recorrido<br>
                En nuestra suerte <strong>nos toca aprender</strong> que aunque con tiempo las heridas sanan<br>
				por más empeño, inocencia, ilusión <i>hay partidos que nunca se ganan</i><br>
				pero se juegan.<br>
            </p>
            <p>
                Y ahora <strong>a dejarte ir</strong>, mi negra<br/>
				quizás no lleve para siempre el alma en pena<br/>
				porque es extraño <i>vivir a medias</i>.<br/>
            </p>
            <p>
                Sé que la vida se me pasa se te espero,<br/>
				por eso vivo <i>yéndome a otro lugar</i>.<br/>
				Sé que el amor cuando es con baile es verdadero,<br/>
				siempre pensé que estarías pa' bailar.<br/>
			</p>
			<p>
                Si he de extrañarte por siempre, que así sea<br/>
				y que <i>por siempre no me dure mucho más</i><br/>
				Mientras tanto yo me iré de otra manera<br/>
				quizás aprenda nuevos pasos, quizás <i>mi vida sea un poema</i><br/>
				quizás <strong>todo esto haga sentido de alguna manera</strong><br/>
			    quizás tenga una linda historia para contarte cuando te vea<br/>
				mientras tanto yo me iré una vez más<br/>
				<i>a otro lugar.</i>
            </p>
        </div>
    {:else if  $locale === 'en'}
        <div>
            <p>
				Translation not yet ready. Hold tight!
            </p>
        </div>
    {/if}

<style>
div {
	text-wrap: balance;
}
</style>
