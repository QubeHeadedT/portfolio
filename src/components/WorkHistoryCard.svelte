<script>
    export let title = 'Job title';
    export let logo = '/images/working_logo.png';
    export let highlights = ['Made stuff', 'Did things'];
</script>

<div>
    <img src={logo} alt="logo">
    <h1>{title}</h1>
    <ul>
        {#each highlights as highlight}
            <li>
                <h6>{highlight}</h6>
            </li>
        {/each}
    </ul>
</div>
