<script lang="ts">
    import DownArrow from "./DownArrow.svelte";

    function handleAnchorClick (event: MouseEvent) {
        event.preventDefault()
        const link = event.currentTarget
        const anchorId = new URL(link.href).hash.replace('#', '')
        const anchor = document.getElementById(anchorId)
        window.scrollTo({
            top: anchor.offsetTop,
            behavior: 'smooth'
        })
    }
</script>

<main class="">
    <div class="flex flex-row mx-auto w-[800px] mt-20 gap-52">
        <div>
            <!-- todo ADD MY IMAGE -->
            <div class="bg-red-900 rounded-full w-64 h-64"></div>
        </div>

        <div class="text-center mt-12">
            <h1 class="font-bold text-4xl">My Name is Nikolai</h1>
            <h2 class="text-xl font-light">lorem...</h2>
        </div>
    </div>

    <div>
<!--        <h1 class="text-4xl font-bold text-center mt-20">My Projects</h1>-->
        <a href="#projects" class="w-full py-20" on:click={handleAnchorClick}>
            <DownArrow />
        </a>
    </div>
</main>