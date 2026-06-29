<script>
  import Header from './lib/components/Header.svelte';
  import Hero from './lib/components/Hero.svelte';
  import PartnerBanner from './lib/components/PartnerBanner.svelte';
  import QuickStats from './lib/components/QuickStats.svelte';
  import About from './lib/components/About.svelte';
  import Learning from './lib/components/Learning.svelte';
  import Audience from './lib/components/Audience.svelte';
  import Requirements from './lib/components/Requirements.svelte';
  import Schedule from './lib/components/Schedule.svelte';
  import Timeline from './lib/components/Timeline.svelte';
  import Benefits from './lib/components/Benefits.svelte';
  import Project from './lib/components/Project.svelte';
  import Selection from './lib/components/Selection.svelte';
  import FAQ from './lib/components/FAQ.svelte';
  import CTASection from './lib/components/CTASection.svelte';
  import Contact from './lib/components/Contact.svelte';

  let scrolled = $state(false);
</script>

<Header bind:scrolled />

<main>
  <Hero />
  <PartnerBanner variant="light" />
  <QuickStats />
  <About />
  <Learning />
  <Audience />
  <Requirements />
  <Schedule />
  <Timeline />
  <Benefits />
  <Project />
  <Selection />
  <FAQ />
  <CTASection />
  <Contact />
</main>

<style>
  main {
    overflow-x: hidden;
  }
</style>
