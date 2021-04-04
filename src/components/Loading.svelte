<script>
    
    window.onload = setTimeout(function() {
        let loading = document.getElementById('loading');
        loading.parentNode.removeChild(loading);
        document.body.classList.remove('hiden');
    }, 2000);

</script>

<div class="loading" id="loading">
    <svg
    xmlns="http://www.w3.org/2000/svg"
    class="loading-logo"
    role="img"
    viewBox="-3 -3 83.999999 96.000115">
        <path
            class="loading-logo__hexagon" 
            d="M 38.693477,3.3013557 C 26.591304,10.128223 14.489132,16.95509 2.3869585,23.781958 c 0,13.964046 0,27.928092 0,41.892138 C 14.489132,72.811275 26.591304,79.948455 38.693477,87.085631 50.79565,80.258766 62.897824,73.4319 74.999997,66.605032 c 0,-13.964046 0,-27.928093 0,-41.892139 C 62.897824,17.575714 50.79565,10.438535 38.693477,3.3013557 Z" />
        <g
            aria-label="D"
            id="text6"
            style="font-size:57.3333px;font-family:sans-serif;fill:#ff5500;stroke:#ff5500;stroke-width:3">
            <path
            class="loading-logo__letter"
            d="m 23.266129,26.05714 h 11.029942 q 8.09049,0 11.981764,3.10742 5.794918,4.591144 5.794918,14.389315 0,10.162104 -5.067054,14.697258 -2.295572,2.043618 -5.151039,2.883462 -2.827472,0.839843 -7.530595,0.839843 H 22.426285 L 26.26157,59.034987 V 29.27654 Z m 8.482417,2.351561 V 59.81884 h 1.539713 V 30.256357 q 1.455728,-0.223959 2.659503,-0.223959 2.295572,0 3.611326,0.475912 1.34375,0.447916 2.687499,1.679686 -2.967446,-1.399739 -6.354814,-1.399739 -0.727864,0 -1.903645,0.11198 V 59.81884 q 3.135415,0 4.759112,-0.503906 1.623697,-0.5319 3.079425,-2.015624 4.059243,-4.115232 4.059243,-13.829419 0,-9.490229 -4.39518,-12.961581 Q 38.831224,28.408701 33.0643,28.408701 Z M 24.161962,64.27001 23.74204,63.514151 h 10.246088 q 7.55859,0 11.477858,-2.099608 8.426428,-4.479165 8.426428,-17.328767 0,-8.594396 -3.779295,-12.765618 l -1.119791,-1.23177 q -0.05599,-0.05599 -0.335937,-0.391927 5.934892,3.723305 5.934892,14.249341 0,11.057937 -5.878903,16.29296 -4.507159,4.031248 -14.725252,4.031248 z"
            style="font-style:normal;font-variant:normal;font-weight:normal;font-stretch:normal;font-size:57.3333px;font-family:Algerian;-inkscape-font-specification:Algerian"
            id="path876" />
        </g>
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
        animation: dispel 2s ease;
        opacity: 0;
    }

    .loading-logo {
        margin: auto;
        width: 130px;
        animation: minimize 2.1s ease;
    }

    .loading-logo__hexagon {
        fill: transparent;
        stroke: #f50;
        stroke-width: 5;
        stroke-linejoin:round;
        stroke-linecap:round;
        stroke-dasharray: 250;
        stroke-dashoffset: 0;
        animation: dash 1.5s linear alternate;
    }

    .loading-logo__letter {
        animation: letter 1s forwards;
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
        0% { stroke-dashoffset: -250; }
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
        59% { opacity: 0; }
        60% { fill: #ff0; stroke: #ff0; }
        100% {  fill: #f50; stroke: #f50; }
    }




</style>