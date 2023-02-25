<script>
    export let title = 'Job title';
    export let logo = '/images/working_logo.png';
    export let highlights = ['Made stuff', 'Did things', 'More stuff', 'And again'];
</script>

<div class="card">
    <div class="top-row">
        <img src={logo} alt="logo">
        <h1 class="title">{title}</h1>
    </div>
    
    
    <div class="highlights">
        <ul>
            {#each highlights as highlight}
                <li>
                    <h6>{highlight}</h6>
                </li>
            {/each}
        </ul>
    </div>
    
</div>

<style>
    .top-row {
        display: flex;
        flex-direction: row;
        align-items: center;
    }

    .title {
        font: "helvetica";
        font-size: 1em;
        top: 20px;
        text-align: center;
        width: 75%;

    }

    .card {
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        border-radius: 10px;
        width: 30%;
        font-family: Arial, Helvetica, sans-serif;
    }

    .card:hover {
        box-shadow: 0 8px 16px 0 rgba(0,0,0,0.4);
    }

    .highlights {
        padding-bottom: 10px;
    }

    img {
        border-radius: 5px 5px 0 0;
        width: 25%;
        height: 25%;
        top: 20px;
        left: 20px;
    }

</style>
