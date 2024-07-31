<script>
    import Navbar from '../Navbar.svelte'
    import Sidebar from '../Sidebar.svelte'
    import Impressum from '../Impressum.svelte'
    import {onMount} from "svelte";

    let open = true

    onMount(() => {
        open = window.innerWidth > 768;
    });
    $: {
        // Disable scrolling when sidebar is open, only on the client
        if (typeof document !== 'undefined') {
            if (open) {
                document.body.classList.add('no-scroll');
            } else {
                document.body.classList.remove('no-scroll');
            }
        }
    }
</script>

<title>Übersetzungsbüro Vlado Stanić</title>
<Sidebar bind:open/>
<Navbar bind:sidebar={open}/>

<div class:content-shifted={open}>
    <Impressum/>
</div>


<svelte:head>
    <link href="https://unpkg.com/tailwindcss@^1.0/dist/tailwind.min.css" rel="stylesheet"/>
</svelte:head>

<style>
    :global(body) {
        padding: 0;
    }
    .content-shifted {
        margin-right: 25%;
        transition: margin-right 0.3s ease-in-out;
    }
    /* When the sidebar is closed */
    div:not(.content-shifted) {
        margin-right: 0;
        transition: margin-right 0.3s ease-in-out;
    }

    @media (max-width: 768px) {
        .content-shifted {
            margin-left: 0;
        }
    }
    :global(.no-scroll) {
        overflow: hidden;
    }
</style>