<script>
  let visible = false;

  function toggleVisibility() {
    visible = !visible;
  }
</script>

<nav class="flex sticky p-4">
  <div class="h-8 flex w-1/3">
    <img src="../../numbers/2-solid.svg" alt="number two" />
    <img src="../../numbers/1-solid.svg" alt="number two" />
  </div>
  <!-- Desktop View -->
  <ul class="md:flex w-2/3 justify-end items-center hidden">
    <li class="mr-20"><a href="#about">About</a></li>
    <li class="mr-20"><a href="#experience">Experience</a></li>
    <li class="mr-20"><a href="#projects">Projects</a></li>
  </ul>
  <div class="flex w-2/3 md:hidden justify-end">
    {#if visible == false}
      <button on:click={toggleVisibility}>
        <img
          class="h-8 w-8"
          src="../../navigation/bars-solid.svg"
          alt="show menu"
        />
      </button>
    {:else if visible == true}
      <button class="block" on:click={toggleVisibility}>
        <img
          class="h-8 w-8"
          src="../../navigation/xmark-solid.svg"
          alt="show menu"
        />
      </button>
    {/if}
  </div>
</nav>

{#if visible == true}
  <nav class="flex p-4 z-10">
    <ul>
      <li class="mr-20"><a href="#about">About</a></li>
      <li class="mr-20"><a href="#experience">Experience</a></li>
      <li class="mr-20"><a href="#projects">Projects</a></li>
    </ul>
  </nav>
{/if}
