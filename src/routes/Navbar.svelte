<script>
    import Logo from "./Logo.svelte";
</script>

<nav class="flex flex-row justify-between px-4 py-2">
    <a href="/">
        <Logo />
    </a>

    <div class="flex flex-row gap-2 text-lg my-auto">
        <a href="/about" class="p-2">
            About
        </a>
        <a href="/contact" class="p-2">
            Contact
        </a>
        <a href="/resume" class="border-2 border-green-600/50 p-2 rounded-lg">
            Resume
        </a>
    </div>
</nav>