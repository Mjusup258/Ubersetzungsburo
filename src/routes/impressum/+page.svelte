<script>
    import Navbar from '../Navbar.svelte'
    import Sidebar from '../Sidebar.svelte'
    import Impressum from './src/routes/impressum/Impressum.svelte'

    let open = false
</script>

<title>Übersetzungsbüro Vlado Stanić</title>
<Sidebar bind:open/>
<Navbar bind:sidebar={open}/>
<Impressum/>


<svelte:head>
    <link href="https://unpkg.com/tailwindcss@^1.0/dist/tailwind.min.css" rel="stylesheet"/>
</svelte:head>

<style>
    :global(body) {
        padding: 0;
    }
</style>