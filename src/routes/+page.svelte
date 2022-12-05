<script>
  import Snow from "../components/Snow.svelte";
  import Flag from "../components/Flag.svelte";
  import "normalize.css/normalize.css"
  import { library } from '@fortawesome/fontawesome-svg-core';
  import { faMapLocationDot, faClock, faSeedling, faClipboardCheck } from '@fortawesome/free-solid-svg-icons';
  import { FontAwesomeIcon, FontAwesomeLayers, FontAwesomeLayersText } from 'fontawesome-svelte';
  let main2;
  library.add(faMapLocationDot, faClock, faSeedling, faClipboardCheck);
</script>

<svelte:head>
    <title>Epoch VT</title>
</svelte:head>
<Snow />
<Flag />
<div class="main" style="overflow: hidden">
    <div class="content" style="color: white">
        <img src="/epoch%20logo-2.png" style="margin: 3px 0 6px -10px; width: 225px" alt="Epoch VT"/>
        <h1 style="margin: 0; font-family: 'JetBrains Mono', monospace; ">Join other high <br>schoolers on <br><strong>December 30</strong> <br>
            for 10 hours of <br><strong>fun & making</strong>!<br>
        </h1>
        <h3 style="margin-bottom: 0; margin-top: 10px">(register below)</h3>
        <svg fill-rule="evenodd" clip-rule="evenodd" stroke-linejoin="round" stroke-miterlimit="1.414" xmlns="http://www.w3.org/2000/svg" aria-label="down-caret" viewBox="0 0 32 32" preserveAspectRatio="xMidYMid meet" fill="currentColor" width="50" height="50" color="white" style="cursor: pointer" on:click={() => main2.scrollIntoView({behavior: "smooth"})}><g><path d="M 0.359841 9.01822C 0.784113 9.37178 1.41467 9.31446 1.76823 8.8902C 3.14518 7.2451 6.52975 3.42464 8.25002 2.11557C 9.99919 3.44663 13.335 7.21555 14.7318 8.8902C 15.0854 9.31446 15.7159 9.37178 16.1402 9.01822C 16.5645 8.66466 16.6215 8.03371 16.2679 7.60943C 14.7363 5.76983 11.2749 1.80977 9.30351 0.408618C 8.99227 0.190441 8.64018 0 8.25002 0C 7.85987 0 7.50778 0.190441 7.19654 0.408618C 5.26486 1.78153 1.73514 5.80788 0.232849 7.60856L 0.231804 7.60982C -0.12176 8.03409 -0.0644362 8.66466 0.359841 9.01822Z" transform="translate(7.12506 20.6251) scale(1 -1)"></path></g></svg>
    </div>
    <div class="quick-info">
        <h2 style="text-align: center; font-size: 1.4em"><strong><FontAwesomeIcon icon={faMapLocationDot} /></strong> 15 Falls Road, Shelburne VT &nbsp;&nbsp;<strong>|</strong>
            <strong>&nbsp;&nbsp;<FontAwesomeIcon icon={faClock} /></strong> December 30, 10am-8pm &nbsp;&nbsp;<strong>|</strong>
            <strong>&nbsp;&nbsp;<FontAwesomeIcon icon={faSeedling} /></strong> Beginners Welcome
        </h2>
    </div>
</div>
<div class="main2" bind:this={main2}>
    <div class="quick-info mobile-only">
        <h2 style="text-align: center"><strong><FontAwesomeIcon icon={faMapLocationDot} /></strong>Hack Club HQ, Shelburne VT<br>
            <strong><FontAwesomeIcon icon={faClock} /></strong> December 30, 10am-8pm<br>
            <strong><FontAwesomeIcon icon={faSeedling} /></strong> Beginners Welcome
        </h2>
    </div>
    <div>
        <h1>Dear student,</h1>
        <p>We're inviting you to learn to code at <strong>Epoch VT</strong>, a 10-hour hackathon (social coding event) where programmers, artists, designers, and other high-schoolers from across Vermont will come together to socialize, build creative projects, and learn new skills. Whether you've never coded before or you're a seasoned developer, we'd love to have you join us!
            <br><br>It's one of several satellite events revolving around <a href="https://epoch.hackclub.com">Epoch</a>, a large high-school hackathon taking place in Dehli, India. Epoch events are organized by <a href="https://hackclub.com">Hack Club</a>, a nonprofit network of high school coding clubs and makers around the world.
            <br><br>Everything at this event is totally free, including meals, drinks, swag (hoodies & stickers!), and other goodies. Our finances are all publicly visible on <a href="https://bank.hackclub.com/epochvt">Hack Club Bank</a>.
            <br><br>If you have any questions, feel free to email Cheru Berhanu at <a href="mailto:cheru@cheru.dev">cheru@cheru.dev</a>. <br>This is going to be a ton of fun! We hope to see you there!
            <br><br>~ <a href="https://cheru.dev">Cheru Berhanu</a>, <a href="https://henrybass.github.io/">Henry Bass</a>, and <a href="https://snwy.me">Mason Meirs</a> :D<br>

        </p>
        <a href="https://register.epochvt.hackclub.com"><button style="background-color: rgba(255, 71, 148, 1);border: solid 2px white; width: 100%; min-height: 50px; font-size: 1.4rem; cursor: pointer">Interested? Register here!</button></a>
    </div>
    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2851.5632645962864!2d-73.22928398447851!3d44.38055797910306!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x4cca7df09a009e9b%3A0xd3a527022dfe1a3e!2sHack%20Club!5e0!3m2!1sen!2sus!4v1669720569531!5m2!1sen!2sus" style="border:0; width: 100%; min-height: 100%; border-radius: 10px" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>


</div>
<p style="font-size: 1.05rem;text-align: center; padding: 0 2em 0.5em 2em;
"><strong>Epoch VT</strong> is fiscally sponsored by <a href="https://hackclub.com/bank">Hack Club Bank</a>, a project by <a href="https://the.hackfoundation.org">The Hack
    Foundation</a> (d.b.a. <a href="https://hackclub.com">Hack Club</a>), a 501(c)(3) nonprofit (EIN: 81-2908499).</p>

<style>
    @import url('https://fonts.googleapis.com/css2?family=JetBrains+Mono&family=Space+Grotesk&display=swap');
    * {
        font-family: "Space Grotesk", system-ui;
        color: white;
    }
    h1 {
        font-size: 1.9em;
        line-height: 120%;
    }
    .main {
        background-image: linear-gradient(0deg, rgba(0, 0, 0,1) 1%, rgba(0, 0, 0, 0.5), rgba(0, 0, 0,0.9) 100%), url(https://epoch.hackclub.com/assemble.jpg);
        background-size: cover;
        background-position: bottom;
        min-height: 100vh;
        overflow: auto;
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
        line-height: 170%;
    }
    .main2 {
        padding: 2em 2em 1em 2em;
        display: grid;
        grid-template-columns: 3fr 2fr;
        gap: 1em;
    }
    .quick-info {
        position: absolute;
        bottom: 0;
    }
    .mobile-only {
        display: none;
    }
    @media (max-width: 768px) {
        .main2 {
            grid-template-columns: 1fr;
        }
        .quick-info {
            display: none;
        }
        .mobile-only {
            display: block;
            position: relative;
        }
    }
</style>