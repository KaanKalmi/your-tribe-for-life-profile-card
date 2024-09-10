<script>
    import LinkedIn from '$lib/images/LinkedIn.png';
    import github from '$lib/images/github-white.png';
</script>

<style>
    .container{
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        background-color: rgb(145, 158, 158);
    }

    .businessCard{
        position: relative;
        width: 675px;
        height: 375px;
        background: url($lib/images/BG.jpg);
        background-size: 150px;
        border-radius: 8px;
        padding: 20px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin: auto;

        & h1{
            position: absolute;
            top: 0;
            margin: .25em;
        }

        & p{
            position: absolute;
            top: 2em;
            margin: .5em;
            border-bottom: 1px solid black;
        }

        & .cardContent{
            position: absolute;
            bottom: 0;

            & h2{
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

</style>
    
<div class="container">
    <article class="businessCard">
        <h1>Kaan Kalmioglu</h1>
        <p>Frontend Developer</p>
        <div class="cardContent">
            <h2>Socials</h2>
            <ul>
                <li> <a href="https://github.com/KaanKalmi"> <img src="{github}" alt="" height="50" width="50"> </a> </li>
                <li> <a href="https://www.linkedin.com/in/kaan-kalmioglu-6a9bab26b/"> <img src="{LinkedIn}" alt="" height="50" width="55"> </a> </li>
            </ul>
        </div>
    </article>
</div>