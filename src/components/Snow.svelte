<script>
  import { loadFull } from "tsparticles";
  import {onMount} from "svelte";
  import Particles from "svelte-particles";
  import "./main.css"


const options = {
  fullScreen: {
    enable: false
  },
  particles: {
  move: {
  direction: "bottom",
  enable: true,
  random: false,
  straight: false,
},
  opacity: {
  value: { min: 0.1, max: 0.5 },
},
  size: {
  value: { min: 0.1, max: 3 },
},
  wobble: {
  distance: 20,
  enable: true,
  speed: {
  min: -5,
  max: 5,
},
},
},
};

  const particlesInit = async (main) => {
  // you can initialize the tsParticles instance (main) here, adding custom shapes or presets
  // this loads the tsparticles package bundle, it's the easiest method for getting everything ready
  // starting from v2 you can add only the features you need reducing the bundle size
  await loadFull(main);
};

</script>

<Particles
        id="tsParticles"
        options="{options}"
        particlesInit="{particlesInit}"
/>