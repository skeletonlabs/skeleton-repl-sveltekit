<script lang="ts">
    let { title, content } = $props();
</script>

<div class="space-y-2">
    <a href="{"#" + title.toLowerCase()}" class="h3">{title}</a>
    <div class="space-y-4 card-enhanced justify-center items-center p-8">
        {@render content?.()}
    </div>
</div>