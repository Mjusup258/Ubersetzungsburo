<script>
    import Hamburger from './Hamburger.svelte';

    export let sidebar = false;

    function toggleSidebar() {
        sidebar = !sidebar;
    }
</script>

<style>
    .navbar {
        position: fixed;
        top: 1rem; /* Adjust this value as needed */
        right: 1rem; /* Adjust this value as needed */
        z-index: 50;
    }
    .button {
        background-color: aliceblue;
        padding: 0.5rem;
        box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
        border-radius: 3px;
        display: flex;
        justify-content: center;
        align-items: center;
    }
</style>

<div class="navbar">
    <button on:click={toggleSidebar} class="button">
        <Hamburger {sidebar}/>
    </button>
</div>
