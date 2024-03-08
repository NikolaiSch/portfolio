<script lang="ts">
    export let project: {
        name: string;
        description: string;
        img: string;
        link: string;
    }
</script>

<div class="w-80">
    <h1 class="text-2xl font-bold py-2">{project.name}</h1>
    <img src={project.img} alt={project.name} class="mx-auto py-2 w-20"/>
    <p class="py-2">{project.description}</p>
    <a href={project.link} class="py-2 text-blue-900 underline">Link</a>
</div>