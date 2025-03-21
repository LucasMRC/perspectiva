    <script lang="ts">
        import { locale } from "@utils/stores";
    </script>

    {#if $locale === 'es'}
        <div>
            <p>
                A veces me descubro sintiendo que <em>le encuentro la lógica a la vida</em>. Que puedo darle forma a los sucesos que acontecen (por lo menos, una forma medio intelectual). Que si veo las cosas desde una u otra perspectiva, entonces resignifico la experiencia y la modifico. Claro, el truco es sólo <strong>elegir la perspectiva</strong>.
            </p>
            <p>
                También me pasa que a medida que pasa el tiempo, <em>cada vez son menos las certezas que tengo</em>. Así, mis acciones se encuentran escoltadas por preguntas, de esas que <strong>no puedo responder sin al menos ser imparcial</strong>.
            </p>
            <p>
                Muy pocas son las cosas que hago sabiendo realmente <strong><em>si estoy actuando de manera correcta o inteligente</em></strong>. Para el resto de mi vida, no sé si estoy siendo paciente o me estoy dejando estar. Si aguantar un poco el dolor me ayuda a construir mi carácter, o es mejor tomar un analgésico porque necesito descansar. Si debo ayudar al otro, o enfocarme y trabajar en pos de mis objetivos.
            </p>
            <p>
                <em>No tengo métricas para medir mis decisiones</em>. Muchas de las cosas que hago son correctas y no lo son <strong>dependiendo del lugar desde el que se las mire</strong>. Pero no soy yo quien debe elegir ese lugar, a mí me toca actuar.
            </p>
            <p>
                Así que acá estoy, a mis 33 años, estableciendo acuerdos conmigo mismo, <strong>normas de convivencia</strong>. Principalmente, una especie de <em>norma de doble-confianza</em>.
            </p>
            <p>
                Primero, confianza en mí, en Lucas. En que las decisiones que he tomado me trajeron a este lugar. <em>Que no me ha salido tan mal, después de todo</em>. Y que con el tiempo, he ido desarrollando un criterio para tomar decisiones. Bueno o malo, <strong>pero propio</strong>. Messirve.
            </p>
            <p>
                Segundo, <strong>confianza en la otra parte</strong>. A estas alturas ya he aprendido que las cosas toman sentido con el tiempo. <em>La historia les va dando significado</em>. Difícilmente pueda ver hoy cómo se van a desenvolver los acontecimientos. En la mayoría de los casos, no me queda más que tomar una decisión. Jugármela, y después confiar.
            </p>
            <p>
                Quizás la vara vaya por aquel lado. En toda esta incertidumbre, si logro que todo siga teniendo sentido. <em>¿Con cuánta flexibilidad y elegancia puedo seguir dándole forma a mi experiencia de estar vivo?</em>
            </p>
            <p>
                Así, doy lugar a una <strong>segunda norma de convivencia</strong>: la Perspectiva. Y es que <em>la gente siempre eligirá un lugar u otro para decidir si lo que hago está bien o no</em>. Qué saben ellos.
            </p>
            <p>
                Por mi parte, yo dejaré que mi capacidad para elegir una perspectiva propia sea la métrica por la que mido mi vida.
            </p>
        </div>
    {:else if  $locale === 'en'}
        <div>
            <p>
                Sometimes I find myself feeling that <em>I find the logic of life</em>. That I can shape the events that happen (at least, in a somewhat intellectual way). That if I look at things from one or another perspective, then I resignify the experience and modify it. Of course, the trick is just <strong>choosing the right perspective</strong>.
            </p>
            <p>
                It also happens to me that as time goes by, <em>the fewer certainties I have</em>. So, my actions are escorted by questions, those that <strong>I can't answer without at least being impartial</strong>.
            </p>
            <p>
                Very few are the things that I do really knowing <strong><em>if I'm acting in the right or intelligent way</em></strong>. For the rest of my life, I don't know if I'm being patient or letting myself be. If I should endure a little pain to build my character, or it's better to take an analgesic because I really need to rest. If I should help the others, or focus and work towards my own goals.
            </p>
            <p>
                <em>I don't have metrics to measure my decisions</em>. Many of the things I do are right or wrong <strong>depending on the place from which they are seen</strong>. But I'm not the one who should choose that place, I have me to act.
            </p>
            <p>
                So here I am, at 33 years old, establishing agreements with myself, <strong>rules of coexistence</strong>. Mainly, a kind of <em>double-trust rule</em>.
            </p>
            <p>
                First, trust in me, in Lucas. That the decisions I have taken have brought me to this where I'm now. <em>That it hasn't gone so bad, after all</em>. And that over time, I have developed a criterion to make decisions. Good or bad, <strong>but my own</strong>. Messirve.
            </p>
            <p>
                Second, <strong>trust in the other party</strong>. At this point I have learned that things make sense over time. <em>History gives them meaning</em>. It is difficult to see how the events will develop today. In most cases, I have no choice but to make a decision. Bet on it, and then trust.
            </p>
            <p>
                And maybe that's the way to measure this. In all this uncertainty, if I manage to keep making sense out of all of this. <em>With how much flexibility and elegance can I shape my experience of being alive?</em>
            </p>
            <p>
                So, I give way to a <strong>second rule of coexistence</strong>: the Perspective. Because <em>people will always choose one place or another to decide whether what I do is right or not</em>. What do they know.
            </p>
            <p>
                On my end, I will let my ability to choose my own perspective be the metric by which I measure my life.
            </p>
        </div>
    {/if}
