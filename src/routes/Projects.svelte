<script lang="ts">
    import Project from "./Project.svelte";

    let projects: {
        name: string,
        description: string,
        link: string,
        img: string
    }[] = [
        {
            name: "Building Health Ltd Website",
            description: "Rebuilt the website from scratch as a freelancer, using SvelteKit and TailwindCSS. The website is fully responsive and is hosted on Vercel. The client was very happy with the result and the website is now live.",
            link: "https://buildinghealth.co.uk",
            img: "buildinghealth.avif"
        },
        {
            name: "Project 2",
            description: "This is a project",
            link: "https://www.google.com",
            img: "https://via.placeholder.com/150"
        },
        {
            name: "Project 3",
            description: "This is a project",
            link: "https://www.google.com",
            img: "https://via.placeholder.com/150"
        }
    ]
</script>

<div class="grid grid-cols-3 mx-auto mt-96 gap-4 justify-items-center text-center" id="projects">
    {#each projects as project}
        <Project {project}/>
    {/each}
</div>