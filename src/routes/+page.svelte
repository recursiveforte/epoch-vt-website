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
            for 10 hours of <br>fun & making at <br>
            <strong>Epoch VT!</strong> </h1>
        <svg fill-rule="evenodd" clip-rule="evenodd" stroke-linejoin="round" stroke-miterlimit="1.414" xmlns="http://www.w3.org/2000/svg" aria-label="down-caret" viewBox="0 0 32 32" preserveAspectRatio="xMidYMid meet" fill="currentColor" width="50" height="50" color="white" style="cursor: pointer" on:click={() => main2.scrollIntoView({behavior: "smooth"})}><g><path d="M 0.359841 9.01822C 0.784113 9.37178 1.41467 9.31446 1.76823 8.8902C 3.14518 7.2451 6.52975 3.42464 8.25002 2.11557C 9.99919 3.44663 13.335 7.21555 14.7318 8.8902C 15.0854 9.31446 15.7159 9.37178 16.1402 9.01822C 16.5645 8.66466 16.6215 8.03371 16.2679 7.60943C 14.7363 5.76983 11.2749 1.80977 9.30351 0.408618C 8.99227 0.190441 8.64018 0 8.25002 0C 7.85987 0 7.50778 0.190441 7.19654 0.408618C 5.26486 1.78153 1.73514 5.80788 0.232849 7.60856L 0.231804 7.60982C -0.12176 8.03409 -0.0644362 8.66466 0.359841 9.01822Z" transform="translate(7.12506 20.6251) scale(1 -1)"></path></g></svg>
        </div>
</div>
<div class="main2" bind:this={main2}>
    <div>
    <h1>The Rundown:</h1>
    <p><strong>Epoch VT</strong> is a 10-hour hackathon (social coding event) where teens come together to discover the joy of code, build creative projects, and build connections with one another. It's taking place at <strong><a href="https://goo.gl/maps/6GnAJgtejh7qqH726">Hack Club HQ</a></strong> (15 Falls Road, Shelburne) from 10AM to 8PM on December 30, 2022.
        <br><br>It's one of many regional events surrounding <a href="https://epoch.hackclub.com">Epoch</a>, a large high-school hackathon taking place in Dehli, India, which is organized by <a href="https://hackclub.com">Hack Club</a>.
    <br><br>Throughout the day, we'll be working on projects together, learning new skills, collecting cool swag (hoodies & stickers!), and meeting new people. Whether you've never coded before or you're a seasoned developer, you're welcome to join us!
        <br><br>Everything at this event is totally free, including lunch, dinner, swag, and other goodies. Our finances are all publicly visible on <a href="https://bank.hackclub.com/epochvt">Hack Club Bank</a>.
        <br><br>If you have any questions, feel free to email Cheru Berhanu at <a href="mailto:cheru@cheru.dev">cheru@cheru.dev</a>. <br>This is going to be a ton of fun! We hope to see you there!
        <br><br>- <a href="https://cheru.dev">Cheru Berhanu</a>, <a href="https://henrybass.github.io/">Henry Bass</a>, and <a href="https://snwy.me">Mason Meirs</a> :D

    </p>
        <a href="https://register.epochvt.hackclub.com"><button style="background-color: rgba(255, 71, 148, 1); width: 100%; min-height: 50px; font-size: 1.4rem; cursor: pointer">Interested? Register here!</button></a>
    </div>
    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2851.5632645962864!2d-73.22928398447851!3d44.38055797910306!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x4cca7df09a009e9b%3A0xd3a527022dfe1a3e!2sHack%20Club!5e0!3m2!1sen!2sus!4v1669720569531!5m2!1sen!2sus" style="border:0; width: 100%; min-height: 100%; border-radius: 10px" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
<div class="faq-container">
    <h1>FAQ:</h1>
    <div class="faq">
        <div>
    <h2>So... What exactly is a hackathon?</h2>
            <p>TODO lol</p>

        </div>
            <div>
    <h2>Hacking? Isn't that dangerous?</h2>
                <p>TODO lol</p>
            </div>
                <div>
    <h2>Who can attend Epoch VT?</h2>
                    <p>TODO lol</p>

                </div>
        <div>
            <h2>I don't know how to code; can I still join?</h2>
            <p>TODO lol</p>

        </div>

        <div>
            <h2>What can I make here?</h2>
            <p>TODO lol</p>

        </div>
        <div>
            <h2>My parents are worried! What should I do?</h2>                <p>TODO lol</p>


        </div>

    </div>
</div>
</div>

<p style="font-size: 1rem;text-align: center; padding: 0 4em 0.5em 4em;
"><strong>Epoch VT</strong> is fiscally sponsored by <a href="http://hackclub.com/bank">Hack Club Bank</a>, a project by <a href="https://the.hackfoundation.org">The Hack
    Foundation</a> (d.b.a. <a href="https://hackclub.com">Hack Club</a>), a 501(c)(3) nonprofit (EIN: 81-2908499).</p>
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
        padding: 4em 4em 1em 4em;
        display: grid;
        grid-template-columns: 3fr 2fr;
        gap: 1em;
    }

    .faq {
        display: grid; grid-template-columns: 1fr 1fr;
    }

    .faq-container {
        grid-column: span 2    }

    @media (max-width: 768px) {
        .faq {
            grid-template-columns: 1fr;
        }
        .main2 {
            grid-template-columns: 1fr;
        }
        .faq-container {
            grid-column: span 1;
        }
    }
</style>