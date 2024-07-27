<script>
    export let open = false
</script>

<button class="hamburger-button" class:open on:click={() => open = !open}>
    <svg width="32" height="24" viewBox="0 0 32 24">
        <line id="top" x1="0" y1="2" x2="32" y2="2"/>
        <line id="middle" x1="0" y1="12" x2="32" y2="12"/>
        <line id="bottom" x1="0" y1="22" x2="32" y2="22"/>
    </svg>
</button>

<style>
    .hamburger-button {
        display: flex;
        align-items: center;
        justify-content: center;
        padding: 0;
        margin: 0;
        border: none;
        background: none;
        cursor: pointer;
        transition: transform 0.3s ease-in-out;
        z-index: 20;
    }

    svg {
        transition: transform 0.3s ease-in-out;
    }

    svg line {
        stroke: currentColor;
        stroke-width: 3;
        transition: transform 0.3s ease-in-out;
    }

    .open svg {
        transform: scale(0.7);
    }

    .open #top {
        transform: translate(6px, 0px) rotate(45deg);
    }

    .open #middle {
        opacity: 0;
    }

    .open #bottom {
        transform: translate(-12px, 9px) rotate(-45deg);
    }
</style>
