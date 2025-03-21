<script lang="ts">
    import { locale } from "../../../utils/stores";

</script>

{#if $locale === 'es'}
    <div>
        <p>
            Próximamente <strong>se vienen más artículos</strong>!
        </p>
        <p>Stay tuned! 😉</p>
    </div>
{:else if $locale === 'en'}
    <div>
        <p>
            More articles <strong>coming soon</strong>!
        </p>
        <p>Stay tuned! 😉</p>
    </div>
{/if}
