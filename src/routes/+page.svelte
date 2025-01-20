<script>
    import { Avatar } from "@skeletonlabs/skeleton-svelte";
  import Section from "$lib/components/Section.svelte";
  const imgSrc = 'https://images.unsplash.com/photo-1620122303020-87ec826cf70d?q=80&w=256&h=256&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D';
</script>
<div class="container h-full mx-auto flex flex-col items-start space-y-10 p-10">
    
    <Section title="Button">
        {#snippet content()}
        <div class="flex gap-4">
            <button type="button" class="btn preset-filled-primary-500">Button</button>
            <button type="button" class="btn preset-tonal-primary">Button</button>
            <button type="button" class="btn preset-outlined-primary-500">Button</button>
          </div>
          <div class="flex gap-4">
            <button type="button" class="btn preset-filled-secondary-500">Button</button>
            <button type="button" class="btn preset-tonal-secondary">Button</button>
            <button type="button" class="btn preset-outlined-secondary-500">Button</button>
          </div>
          <div class="flex gap-4">
            <button type="button" class="btn preset-filled-tertiary-500">Button</button>
            <button type="button" class="btn preset-tonal-tertiary">Button</button>
            <button type="button" class="btn preset-outlined-tertiary-500">Button</button>
          </div>
          <div class="flex gap-4">
            <button type="button" class="btn preset-filled-success-500">Button</button>
            <button type="button" class="btn preset-tonal-success">Button</button>
            <button type="button" class="btn preset-outlined-success-500">Button</button>
          </div>
          <div class="flex gap-4">
            <button type="button" class="btn preset-filled-warning-500">Button</button>
            <button type="button" class="btn preset-tonal-warning">Button</button>
            <button type="button" class="btn preset-outlined-warning-500">Button</button>
          </div>
          <div class="flex gap-4">
            <button type="button" class="btn preset-filled-error-500">Button</button>
            <button type="button" class="btn preset-tonal-error">Button</button>
            <button type="button" class="btn preset-outlined-error-500">Button</button>
          </div>
          <div class="flex gap-4">
            <button type="button" class="btn preset-filled-surface-500">Button</button>
            <button type="button" class="btn preset-tonal-surface">Button</button>
            <button type="button" class="btn preset-outlined-surface-500">Button</button>
          </div>
        {/snippet}
    </Section>
   
    <Section title="Badge">
        {#snippet content()}
        <div class="space-y-4">
            <div class="flex gap-4">
              <span class="badge preset-filled-primary-500">Badge</span>
              <span class="badge preset-tonal-primary">Badge</span>
              <span class="badge preset-outlined-primary-500">Badge</span>
            </div>
            <div class="flex gap-4">
              <span class="badge preset-filled-secondary-500">Badge</span>
              <span class="badge preset-tonal-secondary">Badge</span>
              <span class="badge preset-outlined-secondary-500">Badge</span>
            </div>
            <div class="flex gap-4">
              <span class="badge preset-filled-tertiary-500">Badge</span>
              <span class="badge preset-tonal-tertiary">Badge</span>
              <span class="badge preset-outlined-tertiary-500">Badge</span>
            </div>
            <div class="flex gap-4">
              <span class="badge preset-filled-success-500">Badge</span>
              <span class="badge preset-tonal-success">Badge</span>
              <span class="badge preset-outlined-success-500">Badge</span>
            </div>
            <div class="flex gap-4">
              <span class="badge preset-filled-warning-500">Badge</span>
              <span class="badge preset-tonal-warning">Badge</span>
              <span class="badge preset-outlined-warning-500">Badge</span>
            </div>
            <div class="flex gap-4">
              <span class="badge preset-filled-error-500">Badge</span>
              <span class="badge preset-tonal-error">Badge</span>
              <span class="badge preset-outlined-error-500">Badge</span>
            </div>
            <div class="flex gap-4">
              <span class="badge preset-filled-surface-500">Badge</span>
              <span class="badge preset-tonal-surface">Badge</span>
              <span class="badge preset-outlined-surface-500">Badge</span>
            </div>
          </div>
        {/snippet}
    </Section>

    <Section title="Avatar">
        {#snippet content()}
        <div class="space-y-4">
            <div class="flex gap-4">
              <Avatar src={imgSrc} name="Skeleton"/>
              <div style="filter: url(#Apollo)"><Avatar src={imgSrc} name="SkeletonApollo"/></div>
              <div style="filter: url(#BlueNight)"><Avatar src={imgSrc} name="SkeletonBlueNight"/></div>
              <div style="filter: url(#Emerald)"><Avatar src={imgSrc} name="SkeletonEmerald"/></div>
              <div style="filter: url(#GreenFall)"><Avatar src={imgSrc} name="SkeletonGreenFall"/></div>
              <div style="filter: url(#Noir)"><Avatar src={imgSrc} name="SkeletonNoir"/></div>
              <div style="filter: url(#NoirLight)"><Avatar src={imgSrc} name="SkeletonNoirLight"/></div>
              <div style="filter: url(#Rustic)"><Avatar src={imgSrc} name="SkeletonRustic"/></div>
              <div style="filter: url(#Summer)"><Avatar src={imgSrc} name="SkeletonSummer"/></div>
              <div style="filter: url(#XPro)"><Avatar src={imgSrc} name="SkeletonXPro"/></div>
              <Avatar name="John Doe"></Avatar>
            </div>
        </div>
        {/snippet}
    </Section>
</div>