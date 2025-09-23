<script>
  import { onMount } from "svelte";
  import { gsap } from "gsap";
  import { SplitText } from "gsap/SplitText";

  gsap.registerPlugin(SplitText);

  onMount(() => {

    SplitText.create("#agency-name", {
      type: "chars",
      mask: "lines",
      autoSplit: true,
      onSplit(self) {
        return gsap.from(self.chars, {
          y: 20,
          opacity: 0,
          stagger: 0.05,
          delay: 0.2,
          duration: 0.5,
          ease: "power2.out",
        });
      },
    });

    gsap.to("#agency-name", {
      opacity: 1,
      duration: 1,
    });
  });
</script>

<header>
  <h1 id="agency-name" style="opacity: 0;">APRICITY AGENCY</h1>
</header>

<style>
  header {
    background-color: rgb(6, 26, 50);
    text-align: center;
  }

  #agency-name {
    color: transparent;
    text-shadow:
      0.15vw 0.17vw 0.8vw rgb(0, 0, 0, 0.8),
      0 0 0 #e2a243;
    font-size: 7vw;
    font-weight: 300;
    font-family: "Title";
    letter-spacing: 0.01em;
  }

  @media (max-width: 480px) {
    header {
      margin-top: 20vw;
    }
  }
</style>
