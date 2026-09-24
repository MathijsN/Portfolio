<script>
    import ProjectCard from "$lib/components/ProjectCard.svelte";
    import HeroInfo from "$lib/components/HeroInfo.svelte";
    import AboutText from "$lib/components/AboutText.svelte";
    import SocialLinks from "$lib/components/SocialLinks.svelte";
    import ProjectLink from "$lib/components/ProjectLink.svelte";
    import Background from "$lib/components/Background.svelte";
</script>

<main>
    <Background />
    <HeroInfo />
    <AboutText />
    <ProjectCard />
    <ProjectLink content="Zie alle projecten" href="#" classes="all-projects" />
    <SocialLinks />
</main>

<style>
    main {
        padding-bottom: 10rem;
        min-height: 100vh;
        position: relative;

        @media (width > 1030px) {
            display: grid;
            grid-template-columns: repeat(12, 1fr);
            margin-bottom: 0;
        }
    }
</style>
