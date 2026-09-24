<script>
    import image1 from "$lib/assets/image-x1.webp";
    import ProjectLink from "./ProjectLink.svelte";
</script>

<article>
    <h2>Uitgelicht project</h2>
    <h3>Snappthis</h3>
    <p>
        Een mobiele web applicatie waarbij gebruikers foto's met elkaar delen
        binnen 'snappmaps'.
    </p>

    <ul>
        <li>Liquid</li>
        <li>NodeJS</li>
        <li>PE</li>
    </ul>

    <picture>
        <img src={image1} alt="screenshot of the snappthis app" />
    </picture>

    <ProjectLink
        content="Bekijk dit project"
        href="https://github.com/MathijsN/pleasurable-ui"
        classes="this-project"
    />
</article>

<style>
    ul {
        display: flex;
        flex-wrap: wrap;
        gap: 1rem;
        li {
            width: max-content;
            list-style: none;
            padding-inline: 0.75rem;
        }

        li:nth-of-type(1) {
            background-color: #ff31317d;
        }
        li:nth-of-type(2) {
            background-color: #ffb6c19f;
        }
        li:nth-of-type(3) {
            background-color: #0095ff5d;
        }
    }

    h2 {
        font-weight: 300;
    }

    h3 {
        font-weight: 600;
    }

    article {
        margin-block: 3rem;

        @media (width > 1030px) {
            grid-column: 3/-1;
        }
        @media (width > 1550px) {
            grid-column: 6/-1;
        }
    }

    picture {
        img {
            margin-block: 1rem;
            width: 10rem;
            height: 20rem;
        }
    }

    a {
        display: block;
    }
</style>
