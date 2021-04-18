<script>

    window.onload = setTimeout(function() {
        let loading = document.getElementById('loading');
        loading.parentNode.removeChild(loading);
        document.body.classList.remove('hiden');
    }, 2000);

</script>

<div    class="loading"
        id="loading">

    <svg 
    xmlns="http://www.w3.org/2000/svg"
    class="loading-logo"
    viewBox="0 0  83.854042 94.904541"
    role="img">

        <defs>
            <linearGradient id="Gradient" x1="0" x2="1" y1="0" y2="0">
                <stop offset="0%" stop-color="#ff1133"/>
                <stop offset="100%" stop-color="#da77ff"/>
            </linearGradient>
        </defs>

        <path
        class="loading-logo__hexagon" 
        fill="transparent"
        stroke="url(#Gradient)"
        d="M 25.476205,75.809042 9.3307461,66.290306 9.3643738,47.007162 9.3980014,27.724018 25.428046,18.669133 c 8.88255,-5.017482 16.154174,-9.0265188 16.308436,-8.9912673 0.153116,0.034989 7.606166,4.3857733 16.562334,9.6684073 l 16.28394,9.604791 -0.04157,18.973936 -0.04157,18.973938 -16.343558,9.223746 c -8.988957,5.073061 -16.386495,9.21955 -16.438974,9.21442 -0.05248,-0.0051 -7.360872,-4.292759 -16.240874,-9.528062 z"
        transform="translate(-4.120856,-2.7108133)" />

        <path 
            class="loading-logo__letter"
            fill="url(#Gradient)"
            d="m 19.822266,24.556641 2.345703,2.521484 2.59375,2.789063 v 28.427734 l -6.757813,5.179687 h 4 l 1.275391,2.294922 h 0.882812 9.826172 c 7.007974,0 12.297992,-1.348403 15.722657,-4.410156 l 0.002,-0.002 c 4.309603,-3.838906 6.378906,-9.775548 6.378906,-17.41211 0,-7.072059 -2.05755,-12.309701 -6.271485,-15.197265 -0.0073,-0.0087 -0.0025,-0.003 -0.0098,-0.01172 l -0.002,0.002 c -0.131286,-0.08972 -0.217956,-0.227455 -0.353516,-0.3125 l -0.867187,0.992188 c -0.45903,-0.474577 -0.850353,-1.009807 -1.375,-1.425781 C 44.222569,25.60426 39.882542,24.55664 34.29684,24.55664 Z m 16.070308,7.732421 c 2.051634,0 3.935724,0.416652 5.714844,1.25586 l 0.269531,-0.402344 c 1.581236,2.140241 2.509766,5.475701 2.509766,10.328125 0,6.267191 -1.337127,10.452001 -3.628907,12.775391 v 0.002 h -0.002 c -0.836,0.852078 -1.654285,1.368728 -2.46875,1.636719 -0.535959,0.165018 -1.743226,0.207831 -2.798828,0.28125 V 32.3125 c 0.113308,-0.0036 0.310596,-0.02344 0.404297,-0.02344 z"
            />
    </svg>
    
</div>


<style>
    .loading {
        width: 100vw;
        height: 100vh;
        background-color: var(--background);
        display: flex;
        position: fixed;
        top: 0;
        z-index: 99999;
        animation: dispel 2s ease;
        opacity: 0;
    }

    .loading-logo {
        margin: auto;
        width: 230px;
        animation: minimize 2.1s ease;
    }

    .loading-logo__hexagon {
        stroke-width: 5;
        stroke-linejoin:round;
        stroke-linecap:round;
        stroke-dasharray: 230;
        stroke-dashoffset: 0;
        animation: dash 1s linear alternate;
    }

    .loading-logo__letter {
        animation: letter 1.5s forwards;
    }


    @keyframes dispel {
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

    @keyframes dash {
        0% { stroke-dashoffset: 230; }
        60% { stroke-dashoffset: 0; }
    }

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

    @keyframes letter {
        0% { opacity: 0; }
        40% { opacity: 0; }
        65% { opacity: .5; }
    }




</style>