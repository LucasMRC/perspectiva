<script lang="ts">
    export let language: string;
</script>

{#if language === 'es'}
    <div>
        <p>
            Próximamente <strong>se vienen más artículos</strong>!
        </p>
        <p>Stay tuned! 😉</p>
    </div>
{:else if language === 'en'}
    <div>
        <p>
            More articles <strong>coming soon</strong>!
        </p>
        <p>Stay tuned! 😉</p>
    </div>
{/if}