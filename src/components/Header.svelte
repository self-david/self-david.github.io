<script>
    import { each } from "svelte/internal";

    export let cssVar;





</script>


<header
    style="--background: {cssVar.background};">
    
    <div class="header">
        <a class="header-link" href="./">
            <img  class="header-logo" src="./assets/logo.svg" alt="david">
        </a>
    </div>
</header>


<style>
    header {
        background-color: var(--background);
        display: block;
        position: sticky;
        top: 0;
        width: 100vw;
        height: 56px;
        /* margin:  0 16px 0 16px; */
        z-index: 100;
    }

    .header {
        display: flex;
        height: 100%;
        /* background-color: red; */
        margin: 0 1.5rem;
        align-items: center;
    }

    .header-link {
        display: flex;
        align-items: center;
        height: 100%;
    }

    .header-logo {
        height: 80%;
        background-color: transparent;
    }


</style>