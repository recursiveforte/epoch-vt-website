<a
        title="Hack Club"
        href="https://hackclub.com/"
        class="nav-flag"
></a>
    <style>
    a {
        display: inline-block;
        height: 96px;
        background-image: url(https://assets.hackclub.com/flag-orpheus-left.svg);
        background-repeat: no-repeat;
        background-position: top left;
        background-size: contain;
        cursor: pointer;
        flex-shrink: 0;
        width: 149px;
        position: absolute;
        top: 32px;
        left: 0;
        z-index: 999;
    }
    @media (prefers-reduced-motion: no-preference) {
        a {
            transition: 0.1875s cubic-bezier(0.375, 0, 0.675, 1) transform;
            transform-origin: top left;
        }
        a:hover,
        a:focus {
            animation: waveFlag 0.5s linear infinite alternate;
        }
    }
    @keyframes waveFlag {
        from {
            transform: rotate(0deg);
        }
        to {
            transform: rotate(-5deg);
        }
    }</style>