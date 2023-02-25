<script>
    import WorkHistoryCard from "../components/WorkHistoryCard.svelte";
    let sonrai_logo = '/images/sonrai_logo.jpeg';
    let sonrai_highlights = ['Made stuff', 'Did things', 'More stuff', 'And again'];
    let title = 'Chief butter-patter';
</script>

<h1>Welcome to my website!</h1>
<WorkHistoryCard title={title} logo={sonrai_logo} highlights={sonrai_highlights}/>