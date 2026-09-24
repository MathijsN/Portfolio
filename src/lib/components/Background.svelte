<script></script>

<div class="background"></div>

<style>
    .background {
        background-color: var(--color-secondary);
        position: absolute;
        inset: 0;

        display: grid;
        width: 100vw;

        grid-template-rows: repeat(25, 1fr);
        grid-template-columns: 1fr;
        row-rule: 2px dashed rgb(230, 230, 230);
        z-index: -1;
    }
</style>
