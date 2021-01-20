<script>

    import { fly, fade } from 'svelte/transition';

    let seconds = 1;

    const interval = setInterval(() => seconds += 1, 1000);

</script>

<main class="flexbox" style="opacity: {seconds > 0 ? 1 : 0}">
    {#if seconds > 1}
        <article in:fly="{{ y: 100, duration: 1000 }}" class="leftBox">
            <div style="text-align: left">
                <img class="logo" src="img/logo.svg" alt="logo_Qovery">
            </div>
            <div style="margin-top: 40%">
                    <h1 style="text-align: left" >Qovery Engine</h1> 
                    <!-- <a class="github-button" href="https://github.com/ntkme/github-buttons" data-icon="octicon-star" aria-label="Star ntkme/github-buttons on GitHub">Star</a></h1> -->

                <h3 style="text-align: left" >Abstraction layer to deploy microservices applications on any Cloud provider.</h3>
            </div>
            <div>
                <p  style="text-align: left" class="colorDarkGray">Qovery Engine is an open-source abstraction layer product that turns easy apps deployment on AWS, GCP, Azure and others Cloud providers. </p>
            </div>
            <div style="display: flex; margin: auto -5px; justify-content: start;">
                <div class="buttonLink">
                    <img src="img/discord.svg" alt="">
                </div>
                <div class="buttonLink">
                    <img src="img/discord.svg" alt="">
                </div>
            </div>
        </article>
        {/if}

        <article>
            <div class="intro" style="display: flex; flex-direction: column">    
                {#if seconds > 2}
                    <img in:fly="{{ y: 100, duration: 1000 }}" class="top-hero-illu imgResponsive" src="img/top-hero-illu.svg" alt="illustration">
                {/if}
                {#if seconds > 3}
                    <img in:fly="{{ y: 100, duration: 1000 }}" class="middle-hero-illu imgResponsive" src="img/middle-hero-illu.svg" alt="illustration">
                {/if}
                {#if seconds > 4}
                    <img in:fly="{{ y: 100, duration: 1000 }}" class="bottom-hero-illu imgResponsive" src="img/bottom-hero-illu.svg" alt="illustration">
                {/if}
                {#if seconds > 5}
                <img in:fly="{{ y: 100, duration: 1000 }}" class="dashes imgResponsive" src="img/dashes.svg" alt="illustration">
                {/if}
            </div>
            <img in:fly="{{ y: 100, duration: 1000 }}" class="bottom-hero-illu imgResponsive" src="img/bottom-hero-illu.svg" alt="illustration" style="visibility: hidden">
        </article>
</main>

<style>
   .colorDarkGray{
        color: #8686B2;
    }
    .buttonLink{
        width: 150px;
        height: 60px;
    }
    .top-hero-illu {
    z-index: 9;
    }

    .leftBox{
            width: 30%;
        }


        .intro{
            margin-top: -10px;
        }

@media screen and (max-width: 2200px) {
    
        .flexbox{
            display: flex;
            justify-content: space-evenly;
            padding-top: 5%;
        }

        h1{
            font-size: 2vw;
        }

        .middle-hero-illu {
        margin-top: -100px;
        }

        .bottom-hero-illu {
            margin-top: -83px;
        }

        .dashes{
            margin-top: -802px;
        }
    }

    @media screen and (max-width: 800px) {
        
    .middle-hero-illu {
        margin-top: -68px;
    }

    .bottom-hero-illu {
        margin-top: -56px;
    }

    .dashes{
        margin-top: -802px;
    }
    
    }

    @media screen and (max-width: 610px) {

    main{
        background-color: pink;
        width: 100%;
        height: 1200px;
        margin: 0 auto;
        flex-wrap: wrap;
        justify-content: center;
        color: white;
        
    }

    .flexbox{
    display: flex;
    justify-content: space-evenly;
    padding-top: 5%;
    }
    
    h1{
        font-size: 8vw;
    }

    .top-hero-illu{
        width: 76%;
    }

    .middle-hero-illu {
            width: 76%;
        margin-top: -68px;
    }

    .bottom-hero-illu {
        width: 76%;
        margin-top: -56px;
    }

        .dashes{
            width: 76%;
        margin-top: -600px;
    }

    }


    

</style>