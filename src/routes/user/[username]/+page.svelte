<script lang="ts">
    import {onMount} from 'svelte';
    let username: string;
    
    function getSlugFromUrl() {
        const path = window.location.pathname;
        const pathParts = path.split('/');

        return pathParts[pathParts.length-1];
    }


    onMount(() => {
        username = getSlugFromUrl();
    });

</script>

<main class="container">
    <h1>username</h1>
    <h5>Stuff about people</h5>
    <p>Je ne sais pas ces personnes</p>

</main>