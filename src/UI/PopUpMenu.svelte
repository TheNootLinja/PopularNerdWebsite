<script>
    import { createEventDispatcher } from "svelte";
    import { slide } from "svelte/transition";

    const dispatch = createEventDispatcher();

    function closeMenu() {
        dispatch("closemenu");
    }
</script>

<style>
    .container {
        margin-top: 3rem;
        padding-top: 0;
        height: 300px;
        width: 100%;
        background-color: rgb(77, 77, 77);
        position: fixed;
        z-index: 1;
        border-bottom-left-radius: 5%;
        border-bottom-right-radius: 5%;
    }
    ul {
        padding: 0;
        margin: auto;
        margin-top: 1rem;
        width: 50%;
    }
    li {
        list-style: none;
        text-align: center;
    }
    a {
        text-decoration: none;
        color: white;
        font-size: 2.5rem;
    }
</style>

<div class="container" transition:slide>
    <ul>
        <li><a href="#aboutme" on:click={closeMenu}>About</a></li>
        <li><a href="#prevexp" on:click={closeMenu}>Experience</a></li>
        <li><a href="#projectgrid" on:click={closeMenu}>Projects</a></li>
        <li><a href="#contact" on:click={closeMenu}>Contact</a></li>
    </ul>
</div>
