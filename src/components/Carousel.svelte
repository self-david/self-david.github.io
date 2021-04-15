<script>
	// export let cssVar;
    const images = [
        {
            'src' : './assets/logo.svg',
            'href' : './'
        },
        {
            'src' : 'https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse3.mm.bing.net%2Fth%3Fid%3DOIP.uxUpNscn5gdxHX6idsvG0wHaHS%26pid%3DApi&f=1',
            'href' : './'
        },
        {
            'src' : 'https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse4.mm.bing.net%2Fth%3Fid%3DOIP.Q81O3YYo0PPH_7oWQc94IQHaGU%26pid%3DApi&f=1',
            'href' : './'
        },
        {
            'src' : 'https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse4.mm.bing.net%2Fth%3Fid%3DOIP.Q81O3YYo0PPH_7oWQc94IQHaGU%26pid%3DApi&f=1',
            'href' : './'
        }
        
    ];
</script>

<div class="gallery js-flickity"
    data-flickity-options='&#123; "wrapAround": true &#125;'>

    {#each images as image}
        <div class="gallery-cell">
            <div class="box">
            <img class="photo" src={image.src} alt="">
            <a class="btn" href={image.href}>ver proyecto</a>
            </div>
        </div>
    {/each}
    
</div>



<style>
    


.gallery {
  background: transparent;
  margin: 0 1.5rem;
  /* background: chocolate; */
}

.gallery-cell {
  width: 230px;
  height: 230px;
  margin-right: 25px;
  /* background: red; */
  /* counter-increment: gallery-cell; */
 

    display: flex;
  align-items: center;
  justify-content: center;
}

.box {
  width: 220px;
  height: 220px;
  background: var(--background);
  box-shadow: 3px 3px 8px #000;
  border-radius: 8px;
    display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}



.photo {
    width: auto;
    height: 80%;
    margin-bottom: .5rem;
}

.btn:link, .btn:active, .btn:visited {
    color: #fff;
    text-decoration: none;
    width: 120px;
    height: 20px;
    border-radius: 5px;
    background: var(--background2);
    text-align: center;
    font-size: 1rem;
}
</style>