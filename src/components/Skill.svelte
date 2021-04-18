<script>
    export let data;

    let messege;

    const star = './assets/star.svg';
    const star_media = './assets/star_meida.svg';

    let star_int = 0;
    let star_med = 0;

    const getStart = () => {
        star_int = Math.floor(data[0] / 2);
        star_med = data[0] % 2;
    }

    getStart();


    const leave = () => {
        document.getElementById(data[2]).classList.add('invisible');
    }

    const enter = () => {
        document.getElementById(data[2]).classList.remove('invisible');
    }


</script>


<div class="skill" on:mouseenter={enter} on:mouseleave={leave}>
    <div class="icon">
        {#if !data[1].includes('fa')}
            <img class="icon-img" src="./assets/icons/{data[1]}.svg" alt="">
        {:else}
            <i class={data[1]} alt="{data[2]}"></i>
        {/if}
        
    </div>
    <div class="stars">
        {#each [...Array(star_int).keys()] as star_}
            <i class="fas fa-star star"></i>
        {/each}
        {#if star_med != 0}
            <i class="fas fa-star-half-alt star"></i>
        {/if}
        
    </div>
    <div class="alt invisible" id={data[2]}>
        {data[2]}
    </div>
</div>



<style>
    .skill {
        display: flex;
        align-items: center;
        margin: 5px 0;
        width: 150px;
        height: 45px;
    }

    .icon {
        width: 35px;
        color: var(--color-icon);
        font-size: 1.5rem;
        display: flex;
        justify-content: center; 
    }

    .stars {
        height: 24px;
    }

    .star {
        color: #FFC107;
    }

    .fa-star {
        margin-left: 3px;
    }

    .icon-img {
        /* width: 25px; */
        height: 35px;
    }

    .alt {
        position:absolute;
        background-color:var(--background2);
        padding: 10px;
        width: 100px;
        text-align: center;
        transform: translate(20px, -53px);
        font-size: 1.2rem;
        border-radius: 8px;
    }

    .alt::after {
        content: "";
        position: absolute;
        background-color: var(--background2);
        display: block;
        top: 40px;
        left: 43px;
        width: 30px;
        height: 16px;
        clip-path: polygon(50% 100%, 0 0, 100% 0);
    }

    .invisible {
        opacity: 0;
        z-index: -1;
    }
    
</style>