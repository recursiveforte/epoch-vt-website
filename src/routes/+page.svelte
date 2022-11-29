<script>
  import Snow from "../components/Snow.svelte";
  import Flag from "../components/Flag.svelte";

  import { library } from '@fortawesome/fontawesome-svg-core';
  import { faMapLocationDot } from '@fortawesome/free-solid-svg-icons';
  import { FontAwesomeIcon, FontAwesomeLayers, FontAwesomeLayersText } from 'fontawesome-svelte';

  let main2;

  library.add(faMapLocationDot);
</script>

<svelte:head>
    <title>Epoch VT</title>
</svelte:head>
<Snow />
<Flag />
<div class="main">
    <div class="content" style="color: white">
        <h1 style="margin: 0">Join other high <br>schoolers on <br><strong>December 30</strong> <br>
            for 10 hours of <br>fun & code at <br>
            <strong>Epoch VT!</strong> </h1>
        <svg fill-rule="evenodd" clip-rule="evenodd" stroke-linejoin="round" stroke-miterlimit="1.414" xmlns="http://www.w3.org/2000/svg" aria-label="down-caret" viewBox="0 0 32 32" preserveAspectRatio="xMidYMid meet" fill="currentColor" width="50" height="50" color="white" style="cursor: pointer" on:click={() => main2.scrollIntoView({behavior: "smooth"})}><g><path d="M 0.359841 9.01822C 0.784113 9.37178 1.41467 9.31446 1.76823 8.8902C 3.14518 7.2451 6.52975 3.42464 8.25002 2.11557C 9.99919 3.44663 13.335 7.21555 14.7318 8.8902C 15.0854 9.31446 15.7159 9.37178 16.1402 9.01822C 16.5645 8.66466 16.6215 8.03371 16.2679 7.60943C 14.7363 5.76983 11.2749 1.80977 9.30351 0.408618C 8.99227 0.190441 8.64018 0 8.25002 0C 7.85987 0 7.50778 0.190441 7.19654 0.408618C 5.26486 1.78153 1.73514 5.80788 0.232849 7.60856L 0.231804 7.60982C -0.12176 8.03409 -0.0644362 8.66466 0.359841 9.01822Z" transform="translate(7.12506 20.6251) scale(1 -1)"></path></g></svg>
        </div>
</div>
<div class="main2" bind:this={main2}>
    <div>
    <h1>The Rundown:</h1>
    <p><strong>Epoch VT</strong> is a 10-hour hackathon (social coding event) taking place at <strong><a href="/a">Hack Club HQ</a></strong> (15 Falls Road, Shelburne) from 10AM to 8PM.
        <br>Wel'll be </p>
    </div>
    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2851.5632645962864!2d-73.22928398447851!3d44.38055797910306!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x4cca7df09a009e9b%3A0xd3a527022dfe1a3e!2sHack%20Club!5e0!3m2!1sen!2sus!4v1669720569531!5m2!1sen!2sus" style="border:0; width: 100%; min-height: 500px" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
</div>
<style>
    * {
        font-family: "JetBrains Mono", monospace;
        color: white;
    }
    .main {
        background-image: linear-gradient(0deg, rgba(0, 0, 0, 0.6), rgba(0, 0, 0,0.9) 100%), url(https://epoch.hackclub.com/assemble.jpg);
        background-size: cover;
        background-position: bottom;
        height: 100vh;
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
    }

    .content {
        margin: 2em;
    }

    strong, a {
        color: rgba(255, 71, 148, 1);
    }

    p {
        font-size: 1.3rem;
    }

    .main2 {
        padding: 4em;
        display: grid;
        grid-template-columns: 3fr 2fr;
        gap: 1em;
    }
    @media (max-width: 768px) {
        .main2 {
            grid-template-columns: 1fr;
        }
    }
</style>