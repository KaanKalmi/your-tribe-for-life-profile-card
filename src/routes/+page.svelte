<script>
    import LinkedIn from '$lib/images/LinkedIn.png';
    import github from '$lib/images/github-white.png';
    import pfp from '$lib/images/pfp.jpg';
</script>

<style>
    .container{
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        background-color: rgb(31, 31, 31);
        color: white;
    }

    .businessCard{
        position: relative;
        width: 675px;
        height: 375px;
        background-image: url($lib/images/BG.png);
        border-radius: 8px;
        padding: 24px;
        display: flex;
        justify-content: center;
        margin: auto;
        box-shadow: 4px 8px 12px 8px rgba(0,0,0,0.35);

        & .leftAligned{
            position: absolute;
            left: 0;
            top: 1em;
            height: 90%;
            width: 50%;
            
            & img{
                margin: 2em;
                height: 85%;
                width: 75%;
                border-radius: 6px;
            }
        }

        & .rightAligned{
            margin-left: 6em;

        & h1{
            position: absolute;
            top: 1.2em;
            margin: .25em;
        }

        & h2{
            position: absolute;
            top: 3.25em;
            margin: .25em;
            font-size: 1.25em;
        }

        & p {
            position: absolute;
            top: 6.25em;
            margin: .25em;
        }

        & .cardContent{
            position: absolute;
            bottom: 0;

            & h3{
                text-align: center;
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
    
<div class="container">
    <article class="businessCard">
        <div class="leftAligned">
            <img src="{pfp}" alt="" height="375" width="250">
        </div>
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