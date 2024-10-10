<script>
    import {onMount} from 'svelte'
    import {postStore} from '../store.js'
    import Post from '$lib/components/Post.svelte'

    export let data;

    onMount(()=> {
        postStore.set(data.posts)
    })

</script>

<p>Svelte Test</p>
<hr>
{#each $postStore as p}
    <Post post={p}/>
{/each}

