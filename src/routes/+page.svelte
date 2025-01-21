<script>
  import { Avatar } from "@skeletonlabs/skeleton-svelte";
  import Section from "$lib/components/Section.svelte";
  const imgSrc = 'https://images.unsplash.com/photo-1620122303020-87ec826cf70d?q=80&w=256&h=256&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D';
  const cardImgSrc = 'https://images.unsplash.com/photo-1463171515643-952cee54d42a?q=80&w=450&h=190&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D';
</script>
<div class="container h-full mx-auto flex flex-col items-start space-y-10 p-10">
    <Section title="Alerts">
        {#snippet content()}
        <div class="space-y-8">
            <div class="card preset-outlined-success-500 grid grid-cols-1 items-center gap-4 p-4 lg:grid-cols-[1fr_auto]">
              <div>
                <p class="font-bold">Success</p>
                <p class="type-scale-1 opacity-60">The task has been completed successfully.</p>
              </div>
            </div>
            <div class="card preset-outlined-warning-500 grid grid-cols-1 items-center gap-4 p-4 lg:grid-cols-[auto_1fr_auto]">
              <div>
                <p class="font-bold">Warning</p>
                <p class="type-scale-1 opacity-60">Beware of this important notice.</p>
              </div>
            </div>
            <div class="card preset-outlined-error-500 grid grid-cols-1 items-center gap-4 p-4 lg:grid-cols-[auto_1fr_auto]">
              <div>
                <p class="font-bold">Error</p>
                <p class="type-scale-1 opacity-60">Something has gone wrong.</p>
              </div>
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
            </div>
            <div class="flex gap-4">
              <div style="filter: url(#Emerald)"><Avatar src={imgSrc} name="SkeletonEmerald"/></div>
              <div style="filter: url(#GreenFall)"><Avatar src={imgSrc} name="SkeletonGreenFall"/></div>
              <div style="filter: url(#Noir)"><Avatar src={imgSrc} name="SkeletonNoir"/></div>
            </div>
            <div class="flex gap-4">
              <div style="filter: url(#NoirLight)"><Avatar src={imgSrc} name="SkeletonNoirLight"/></div>
              <div style="filter: url(#Rustic)"><Avatar src={imgSrc} name="SkeletonRustic"/></div>
              <div style="filter: url(#Summer)"><Avatar src={imgSrc} name="SkeletonSummer"/></div>
            </div>
            <div class="flex gap-4">
              <div style="filter: url(#XPro)"><Avatar src={imgSrc} name="SkeletonXPro"/></div>
              <Avatar name="John Doe"></Avatar>
            </div>
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

    <Section title="Blockquotes">
        {#snippet content()}
          <div class="space-y-4">
            <blockquote class="blockquote">
              "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nesciunt, aliquid. Molestias, odio illum voluptatibus natus dignissimos, quidem
              est unde aspernatur veniam pariatur fuga distinctio esse in quas, repellendus neque reiciendis!"
            </blockquote>
          </div>
        {/snippet}
    </Section>

    <Section title="Breadcrumbs">
        {#snippet content()}
          <ol class="flex items-center gap-4">
            <li><a class="opacity-60 hover:underline" href="#breadcrumbs">Blog</a></li>
            <li class="opacity-50" aria-hidden="true">&rsaquo;</li>
            <li><a class="opacity-60 hover:underline" href="#breadcrumbs">Category</a></li>
            <li class="opacity-50" aria-hidden="true">&rsaquo;</li>
            <li>Article</li>
          </ol>
        {/snippet}
    </Section>

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

    <Section title="Card">
        {#snippet content()}
        <a
          href="#card"
          class="card preset-filled-surface-100-900 border-[1px] border-surface-200-800 card-hover divide-surface-200-800 block max-w-md divide-y overflow-hidden"
        >
          <header>
            <img src={cardImgSrc} class="aspect-[21/9] w-full grayscale hue-rotate-90" alt="banner" />
          </header>
          <article class="space-y-4 p-4">
            <div>
              <h2 class="h6">Announcements</h2>
              <h3 class="h3">Skeleton is Awesome</h3>
            </div>
            <p class="opacity-60">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Numquam aspernatur provident eveniet eligendi cumque consequatur tempore sint
              nisi sapiente. Iste beatae laboriosam iure molestias cum expedita architecto itaque quae rem.
            </p>
          </article>
          <footer class="flex items-center justify-between gap-4 p-4">
            <small class="opacity-60">By Alex</small>
            <small class="opacity-60">On {new Date().toLocaleDateString()}</small>
          </footer>
        </a>
        {/snippet}
    </Section>

    <Section title="Code">
        {#snippet content()}
          <div class="space-y-4">
            <div><code class="code">console.log()</code></div>
          </div>
        {/snippet}
    </Section>

    <Section title="Form">
        {#snippet content()}
          <form class="mx-auto w-full max-w-md space-y-4">
            <!-- Search -->
            <input class="input" type="search" placeholder="Search..." />
            <!-- Date Picker -->
            <label class="label">
              <span class="label-text">Date</span>
              <input class="input" type="date" />
            </label>
            <!-- File Input -->
            <label class="label">
              <span class="label-text">File Input</span>
              <input class="input" type="file" />
            </label>
            <!-- Range -->
            <label class="label">
              <span class="label-text">Range</span>
              <input class="input" type="range" value="75" max="100" />
            </label>
            <!-- Progress -->
            <label class="label">
              <span class="label-text">Progress</span>
              <progress class="progress" value="50" max="100"></progress>
            </label>
            <!-- Color -->
            <!-- TODO: convert to mini-component for reactive value -->
            <div class="grid grid-cols-[auto_1fr] gap-2">
              <input class="input" type="color" value="#bada55" />
              <input class="input" type="text" value="#bada55" readonly tabindex="-1" />
            </div>
          </form>
        {/snippet}
    </Section>

    <Section title="Headings">
        {#snippet content()}
        <div class="space-y-4">
            <h1 class="h1">Heading 1</h1>
            <h2 class="h2">Heading 2</h2>
            <h3 class="h3">Heading 3</h3>
            <h4 class="h4">Heading 4</h4>
            <h5 class="h5">Heading 5</h5>
            <h6 class="h6">Heading 6</h6>
          </div>
        {/snippet}
    </Section>

    <Section title="Keyboard">
        {#snippet content()}
          <div class="space-y-4">
            <div>Press <kbd class="kbd">⌘</kbd> + <kbd class="kbd">C</kbd> to copy.</div>
          </div>
        {/snippet}
    </Section>

    <Section title="Layout">
        {#snippet content()}
          <section class="grid grid-cols-2 gap-4 md:grid-cols-4">
            <!-- Column -->
            <div class="grid gap-4">
              <img class="bg-surface-500 rounded-container" src="https://picsum.photos/220/320?random=1" alt="Random"/>
              <img class="bg-surface-500 rounded-container" src="https://picsum.photos/220/120?random=2" alt="Random" />
              <img class="bg-surface-500 rounded-container" src="https://picsum.photos/220/280?random=3" alt="Random" />
            </div>
            <!-- Column -->
            <div class="grid gap-4">
              <img class="bg-surface-500 rounded-container" src="https://picsum.photos/220/300?random=4" alt="Random" />
              <img class="bg-surface-500 rounded-container" src="https://picsum.photos/220/280?random=5" alt="Random" />
              <img class="bg-surface-500 rounded-container" src="https://picsum.photos/220/140?random=6" alt="Random" />
            </div>
            <!-- Column -->
            <div class="grid gap-4">
              <img class="bg-surface-500 rounded-container" src="https://picsum.photos/220/280?random=7" alt="Random" />
              <img class="bg-surface-500 rounded-container" src="https://picsum.photos/220/320?random=8" alt="Random" />
              <img class="bg-surface-500 rounded-container" src="https://picsum.photos/220/140?random=9" alt="Random" />
            </div>
            <!-- Column -->
            <div class="grid gap-4">
              <img class="bg-surface-500 rounded-container" src="https://picsum.photos/220/320?random=10" alt="Random" />
              <img class="bg-surface-500 rounded-container" src="https://picsum.photos/220/140?random=11" alt="Random" />
              <img class="bg-surface-500 rounded-container" src="https://picsum.photos/220/280?random=12" alt="Random" />
            </div>
          </section>
        {/snippet}
    </Section>

    <Section title="Pre-Formatted">
        {#snippet content()}
          <div class="space-y-4">
            <pre class="pre">The quick brown fox jumps over the lazy dog.</pre>
          </div>
        {/snippet}
    </Section>
</div>