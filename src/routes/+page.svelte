<script>
    import Button from '$lib/components/Button.svelte'
    import Card from '$lib/components/Card.svelte';
</script>

<h1>Welcome to SvelteKit</h1>
<div class="conteiner">
    <Button color="brown">Login</Button>
    <Button color="brown">Register</Button>
</div>

<Card label="Nadpis 1">
    lorelmm msdfm fmdmsf d sd
</Card>

<Card label="Nadpis 2">
    lorelmm msdfm fmdmsf d sd
</Card>
<Card label="Nadpis 3">
    lorelmm msdfm fmdmsf d sd
</Card>

<style lang="scss">

    .conteiner{
        display: flex;
        width: 100%;
        max-width: 1300px;
        gap: 36px;
        justify-content: center;
        align-items: center;
        margin: auto;
    }
</style>

