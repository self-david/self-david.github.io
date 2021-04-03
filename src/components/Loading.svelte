<script>
    
    window.onload = setTimeout(function() {
        let loading = document.getElementById('loading');
        loading.parentNode.removeChild(loading);
        document.body.classList.remove('hiden');
    }, 200);

</script>

<div class="loading" id="loading">
    <svg class="loading-logo" xmlns="http://www.w3.org/2000/svg" role="img" viewBox="-3 -3 84 96">
        <title>Logo</title>
        <polygon class="loading-logo__hexagon" points="39 0 0 22 0 67 39 90 78 68 78 23"></polygon>
        <text class="loading-logo__letter"  x="24" y="61">D</text>
    </svg>
</div>

<style>
    .loading {
        width: 100vw;
        height: 100vh;
        background-color: #123;
        display: flex;
        position: fixed;
        top: 0;
        z-index: 99999;
        animation: delete 2s ease;
        opacity: 0;

        @keyframes delete {
            0% {
                opacity: 1;
            }
            84% {
                opacity: 1;
            }
            85% {
                opacity: .5;
            }
            100% {
                opacity: 0;
            }
        }
    }

    .loading-logo {
        margin: auto;
        width: 130px;
        background-color: transparent;
        animation: minimize 2.1s ease;

        @keyframes minimize {
            75% {
                transform: scale(1);
                opacity: 1;
            }
            90% {
                transform: scale(0.5);
            }
            100% {
                transform: scale(0);
            }
        }
    }

    .loading-logo__hexagon {
        fill: #123;
        stroke: #f50;
        stroke-width: 5;
        stroke-linejoin:round;
        stroke-linecap:round;
        stroke-dasharray: 270;
        stroke-dashoffset: 0;
        animation: draw 1s ease-in-out forwards;

        @keyframes draw {
            0% { stroke-dashoffset: -270; }
            60% { stroke-dashoffset: 0; }
        }
    }

    .loading-logo__letter {
        fill: #f50;
        stroke: #f50;
        stroke-width: 3;
        font-family: sans-serif;
        font-size: 45px;
        animation: 0.3s;
        animation: letter 1s forwards;


        @keyframes letter {
            0% { opacity: 0; }
            59% { opacity: 0; }
            60% { fill: #ff0; stroke: #ff0; }
            100% {  fill: #f50; stroke: #f50; }
        }
    }





</style>