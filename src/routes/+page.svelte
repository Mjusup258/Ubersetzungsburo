<script>
    import { onMount } from "svelte";
    import Navbar from './Navbar.svelte';
    import Sidebar from './Sidebar.svelte';
    import Main from './Main.svelte';

    let open = true;

    onMount(() => {
        open = window.innerWidth > 768;
    });

    $: {
        if (typeof document !== 'undefined') {
            if (open && window.innerWidth <= 768) {
                document.body.classList.add('no-scroll');
            } else {
                document.body.classList.remove('no-scroll');
            }
        }
    }
</script>

<title>Übersetzungsbüro Vlado Stanić</title>

<Sidebar bind:open />
<Navbar bind:sidebar={open} />

<div class:content-shifted={open}>
    <Main />
</div>

<svelte:head>
    <link href="https://unpkg.com/tailwindcss@^1.0/dist/tailwind.min.css" rel="stylesheet"/>
</svelte:head>

<style>
    :global(body) {
        padding: 0;
        margin: 0;
        box-sizing: border-box;
        overflow-x: hidden; /* Prevent horizontal scrolling */
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
