<script>
    import LinkedIn from '$lib/images/LinkedIn.png';
    import github from '$lib/images/github-white.png';
    import pfp from '$lib/images/pfp.jpg';
    import figure from '$lib/images/figure.png';

    import {breakpoint, platform} from '../mediaquery.svelte';
</script>

{#if $breakpoint == "xs"}
<style>
    .container{
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        background-color: rgb(31, 31, 31);
        color: rgb(145, 213, 240);
    }

    .businessCard{
        position: relative;
        width: 90%;
        height: 300px;
        background-color: #252525;
        border-radius: 8px;
        border: 2px solid #91d5f025;
        display: flex;
        justify-content: center;
        margin: auto;
        box-shadow: 4px 8px 12px 8px rgba(0,0,0,0.35);

        & .leftAligned{
            position: absolute;
            left: 0;
            height: 100%;
            width: 50%;
            
            & img{
                height: 100%;
                width: 100%;
                border-radius: 8px 0 0 8px; 
                border-right: 1px solid #42C9FF;
            }
        }

        & .figure{
            Display: none;
        }
        & .rightAligned{
            margin-left: 1em;

        & h1{
            position: absolute;
            top: 1em;
            margin: .2em;
            color: #42C9FF;
            font-size: 1em;
        }

        & h2{
            position: absolute;
            top: 3em;
            margin: .2em;
            font-size: 1em;
            color: #91D5F0;
        }

        & p {
            position: absolute;
            top: 5.5em;
            margin: .2em;
            color: #FFFFFF;
        }

        & .cardContent{
            position: absolute;
            bottom: 0;

            & h3{
                text-align: center;
                color: #FFFFFF;
            }

            & ul{
                list-style-type: none;
                padding: 0;
                line-height: 1.6em;
                display: flex;
                flex-direction: row;

                & li{
                    margin: 0 1em;

                & a{
                    text-decoration: none;
                    color: black;
                }
            }
            }
        }
    }
    }
</style>
{/if}  
{#if $breakpoint == "s"}
<style>
    .container{
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        background-color: rgb(31, 31, 31);
        color: rgb(145, 213, 240);
    }

    .businessCard{
        position: relative;
        width: 90%;
        height: 300px;
        background-color: #252525;
        border-radius: 8px;
        border: 2px solid #91d5f025;
        display: flex;
        justify-content: center;
        margin: auto;
        box-shadow: 4px 8px 12px 8px rgba(0,0,0,0.35);

        & .leftAligned{
            position: absolute;
            left: 0;
            height: 100%;
            width: 45%;
            
            & img{
                height: 100%;
                width: 100%;
                border-radius: 8px 0 0 8px; 
                border-right: 1px solid #42C9FF;
            }
        }

        & .figure{
            Display: none;
        }
        & .rightAligned{
            margin-left: 1em;

        & h1{
            position: absolute;
            top: 1em;
            margin: .2em;
            color: #42C9FF;
        }

        & h2{
            position: absolute;
            top: 3em;
            margin: .2em;
            font-size: 1.2em;
            color: #91D5F0;
        }

        & p {
            position: absolute;
            top: 5.5em;
            margin: .2em;
            color: #FFFFFF;
        }

        & .cardContent{
            position: absolute;
            bottom: 0;

            & h3{
                text-align: center;
                color: #FFFFFF;
            }

            & ul{
                list-style-type: none;
                padding: 0;
                line-height: 1.6em;
                display: flex;
                flex-direction: row;

                & li{
                    margin: 0 1em;

                & a{
                    text-decoration: none;
                    color: black;
                }
            }
            }
        }
    }
    }
</style>
{/if}  

{#if $breakpoint == "m"}
<style>
    .container{
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        background-color: rgb(31, 31, 31);
        color: rgb(145, 213, 240);
    }

    .businessCard{
        position: relative;
        width: 700px;
        height: 400px;
        background-color: #252525;
        border-radius: 8px;
        border: 2px solid #91d5f025;
        display: flex;
        justify-content: center;
        margin: auto;
        box-shadow: 4px 8px 12px 8px rgba(0,0,0,0.35);

        & .leftAligned{
            position: absolute;
            left: 0;
            height: 100%;
            width: 45%;
            
            & img{
                height: 100%;
                width: 100%;
                border-radius: 8px 0 0 8px; 
                border-right: 1px solid #42C9FF;
            }
        }

        & .figure{
            position: absolute;
            bottom: 0;
            z-index: 1;
        }
        & .rightAligned{
            margin-left: 10em;

        & h1{
            position: absolute;
            top: 1.2em;
            margin: .25em;
            color: #42C9FF;
        }

        & h2{
            position: absolute;
            top: 3.25em;
            margin: .25em;
            font-size: 1.25em;
            color: #91D5F0;
        }

        & p {
            position: absolute;
            top: 6.25em;
            margin: .25em;
            color: #FFFFFF;
        }

        & .cardContent{
            position: absolute;
            bottom: 0;

            & h3{
                text-align: center;
                color: #FFFFFF;
            }

            & ul{
                list-style-type: none;
                padding: 0;
                line-height: 1.6em;
                display: flex;
                flex-direction: row;

                & li{
                    margin: 0 1em;

                & a{
                    text-decoration: none;
                    color: black;
                }
            }
            }
        }
    }
    }
</style>
{/if}    
<div class="container">
    <article class="businessCard">
        <div class="leftAligned">
            <img src="{pfp}" alt="" height="375" width="250">
        </div>
        <img src="{figure}" alt="" class="figure">
        <div class="rightAligned">
        <h1>Kaan Kalmioglu</h1>
        <h2>Frontend Developer</h2>
        <p> Squad 2D</p>
        <div class="cardContent">
            <h3>Socials</h3>
            <ul>
                <li> <a href="https://github.com/KaanKalmi"> <img src="{github}" alt="" height="50" width="50"> </a> </li>
                <li> <a href="https://www.linkedin.com/in/kaan-kalmioglu-6a9bab26b/"> <img src="{LinkedIn}" alt="" height="50" width="55"> </a> </li>
            </ul>
        </div>
    </div>
    </article>
</div>