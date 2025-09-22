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
			No es nada fácil dejar partir todo eso que creímos saber sobre vivir.<br/>
			Son los detalles, los momentos, <i>quisiera no perder tu imagen con el tiempo.</i><br/>
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
			Ven, <strong>bailemos la noche los dos</strong> si esta historia ya tiene un destino<br/>
			no sea cosa que al amanecer nos quedemos sin lo recorrido<br/>
			En nuestra suerte <strong>nos toca aprender</strong> que aunque con tiempo las heridas sanan<br/>
			por más empeño, inocencia, ilusión <i>hay partidos que nunca se ganan</i><br/>
			pero se juegan.<br/>
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
			I'm leaving to another place, taking my music, my life, once again.<br/>
			She isn’t coming, <strong>she won’t come anymore</strong>, the gentle sweet breeze invites me to fly away,<br/>
			to fly away.
		</p>
		<p>
			There’s no destination (<i>or did I forget it?</i>), I don’t know if I’ll ever reach somewhere sometime.<br/>
			But it doesn’t matter, I’ll just leave.<br/>
			<i>[...]</i>
		</p>
		<p>
			I’ll have a quiet coffee somewhere,<br/>
			remembering that sometimes <i>life is that way.</i><br/>
			It’s not easy at all,<br/>
			for anyone here.<br/>
		</p>
		<p>
			I know life slips away if I wait for you,<br/>
			that’s why I live my life always heading to another place.<br/>
			I know <strong>love when it’s with dancing is real</strong>,<br/>
			I always thought you’d be here<br/>
			to dance one more piece.<br/>
		</p>
		<p>
			It’s not easy to let go of everything we thought we knew about living.<br/>
			It’s the details, the moments, <i>I wish I didn’t lose your image over time.</i><br/>
		</p>
		<p>
			And <strong>life is complex</strong>, I know<br/>
			I’ve already <i>learned not to ask why.</i><br/>
			You’re so far away, and so am I.<br/>
		</p>
		<p>
			I know <i>life slips away if I wait for you</i>,<br/>
			that’s why I live my life always heading to another place.<br/>
			I know love when it’s with dancing is real,<br/>
			<i>I always thought you’d be here</i><br/>
			to dance one more piece.<br/>
		</p>
		<p>
			Come, <strong>let’s dance the night together</strong> if this story already has a ending<br/>
			let’s not end up at sunrise without even having the road we traveled<br/>
			In our fate <strong>we have to learn</strong> that even though wounds heal with time<br/>
			no matter the effort, innocence, hope <i>some matches are never won</i><br/>
			but they’re still played.<br/>
		</p>
		<p>
			And now <strong>I'll let you go</strong>, my girl<br/>
			perhaps I won’t carry a grieving soul forever<br/>
			because it’s strange <i>to live half‑heartedly</i>.<br/>
		</p>
		<p>
			I know life slips by if I wait for you,<br/>
			that’s why I live my life <i>always heading to another place</i>.<br/>
			I know love when it’s with dancing is real,<br/>
			I always thought you’d be here to dance one more piece.<br/>
		</p>
		<p>
			If I’m to miss you forever, so be it<br/>
			and may <i>forever not last much longer for me</i><br/>
			Meanwhile I’ll go to another place<br/>
			perhaps I'll learn new steps, perhaps <i>my life becomes a poem</i><br/>
			perhaps <strong>all this will make sense somehow</strong><br/>
			perhaps I’ll have an awesome story to tell you when I see you<br/>
			meanwhile I’ll leave once more<br/>
			<i>to another place.</i>
		</p>
	</div>
{/if}

<style>
div {
	text-wrap: balance;
}
</style>
