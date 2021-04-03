<script>
    import { each } from "svelte/internal";

    export let navBar = ['sobre mi'];

    let burger_menu = '';
    let navbar__hiden = '';

    const activate = () => {
        if(burger_menu == '') {
            burger_menu =  'burger--active';
            navbar__hiden = 'navbar--hiden';
        } else {
            burger_menu =  '';
            navbar__hiden = '';
            
        }
    };


</script>


<header>
    <div class="header">
        <a class="header-link" href="./">
            <img class="header-logo" src="./assets/logo.svg" alt="david">
        </a>

        <div class="burger-icon" on:click="{activate}">
            <div class="burger-icon__bar {burger_menu}"></div>
        </div>
    </div>

    <nav class="navbar {navbar__hiden}" id="navbar">
        <ul class="navbar__list">
            {#each navBar as opc}
                <li class="navbar__item"><a href="#{opc}" class="navbar__link">{opc}</a></li>
            {/each}
        </ul>
    </nav>
</header>


<style>
    header {
        background-color: #234;
        display: block;
        position: sticky;
        top: 0;
        width: 100vw;
        height: 65px;
    }

    .header {
        display: flex;
        height: 100%;
        margin: 0 40px;
        align-items: center;
    }

    .header-link {
        height: 100%;
    }

    .header-logo {
        height: 90%;
    }

    .burger-icon {
        display: flex;
        align-items: center;
        justify-content: center;
        width: 50px;
        height: 50px;
        margin-right: 20px;
        cursor: pointer;
        position: fixed;
        right: 0;
        z-index: 100;
    }

    .burger-icon__bar {
        background-color: #fff;
        width: 40px;
        height: 5px;
        border-radius: 2.5px;
        position: relative;
        /* z-index: 100; */
    }

    .burger-icon__bar::before, .burger-icon__bar::after {
        content: '';
        background-color: #fff;
        width: 40px;
        height: 5px;
        border-radius: 2.5px;
        position: absolute;
        display: block;
        transition: .5s;
    }

    .burger-icon__bar::before {
        top: -11px;
    }
    
    .burger-icon__bar::after {
        top: 11px;
    }

    .burger--active {
        background-color: transparent;
    }

    .burger--active::before {
        top: 0;
        transform: rotate(-45deg);
    }
    
    .burger--active::after {
        top: 0;
        transform: rotate(45deg);
    }

    .navbar {
        position: fixed;
        width: 0;
        right: 0;
        top: 0;
        height: 100vh;
        transition: 1s;
        /* z-index: -1; */
    }

    .navbar--hiden {
        background-color: rgba(34, 51, 68, 0.9);
        
        width: 100vw;

    }

    .navbar__list {
        display: flex;
        align-items: center;
        justify-content: center;
        background-color: hsla(210, 33, 20, .95);
        width: 100vw;
        height: 100vh;
        margin: 0;
        padding: 0;
        display: flex;
        flex-direction: column;
        list-style: none;
    }

    .navbar__item {
        margin: 1rem;
        display: flex;
    }
    
    .navbar__link {
        font-family: sans-serif;
        font-size: 1.2rem;
        text-transform: uppercase;
        text-decoration: none;
        color: #fff;
        margin: auto;
    }

    .navbar__link:hover {
            color: #4981B8;
            font-weight: 600;
        }

    

 </style>