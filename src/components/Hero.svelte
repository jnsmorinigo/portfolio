<script>
  let mobileMenu = false;

  const triggerMobileNavItem = (sectionId) => {
    const section = document.querySelector(sectionId);
    if (section) {
      section.scrollIntoView({ behavior: 'smooth' });
      mobileMenu = false;
    }
  };
</script>

<div
  class="pointer-events-none fixed inset-0 z-70 min-h-screen bg-black bg-opacity-70 opacity-0 transition-opacity lg:hidden"
  class:opacity-100={mobileMenu}
  class:pointer-events-auto={mobileMenu}
>
  <div
    class="absolute right-0 min-h-screen w-2-3 bg-primary py-4 px-8 shadow md:w-1-3"
  >
    <button
      class="absolute top-0 right-0 mt-4 mr-4"
      on:click={() => (mobileMenu = false)}
    >
      <img src="../../public/img/icon-close.svg" class="h-10 w-auto" alt="" />
    </button>

    <ul class="mt-8 flex flex-col">
      <li class="py-2">
        <span
          on:click={() => triggerMobileNavItem('#about')}
          class="cursor-pointer pt-1-2 font-header font-semibold uppercase text-white"
        >
          About
        </span>
      </li>

      <li class="py-2">
        <span
          on:click={() => triggerMobileNavItem('#services')}
          class="cursor-pointer pt-1-2 font-header font-semibold uppercase text-white"
        >
          Services
        </span>
      </li>

      <li class="py-2">
        <span
          on:click={() => triggerMobileNavItem('#portfolio')}
          class="cursor-pointer pt-1-2 font-header font-semibold uppercase text-white"
        >
          Portfolio
        </span>
      </li>

      <li class="py-2">
        <span
          on:click={() => triggerMobileNavItem('#clients')}
          class="cursor-pointer pt-1-2 font-header font-semibold uppercase text-white"
        >
          Clients
        </span>
      </li>

      <li class="py-2">
        <span
          on:click={() => triggerMobileNavItem('#work')}
          class="cursor-pointer pt-1-2 font-header font-semibold uppercase text-white"
        >
          Work
        </span>
      </li>

      <li class="py-2">
        <span
          on:click={() => triggerMobileNavItem('#statistics')}
          class="cursor-pointer pt-1-2 font-header font-semibold uppercase text-white"
        >
          Statistics
        </span>
      </li>

      <li class="py-2">
        <span
          on:click={() => triggerMobileNavItem('#blog')}
          class="cursor-pointer pt-1-2 font-header font-semibold uppercase text-white"
        >
          Blog
        </span>
      </li>

      <li class="py-2">
        <span
          on:click={() => triggerMobileNavItem('#contact')}
          class="cursor-pointer pt-1-2 font-header font-semibold uppercase text-white"
        >
          Contact
        </span>
      </li>
    </ul>
  </div>
</div>

<style>
  .pointer-events-none {
    pointer-events: none;
  }
  .pointer-events-auto {
    pointer-events: auto;
  }
  .fixed {
    position: fixed;
  }
  .inset-0 {
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
  }
  .z-70 {
    z-index: 70;
  }
  .min-h-screen {
    min-height: 100vh;
  }
  .bg-black {
    background-color: black;
  }
  .bg-opacity-70 {
    background-color: rgba(0, 0, 0, 0.7);
  }
  .opacity-0 {
    opacity: 0;
  }
  .transition-opacity {
    transition: opacity 0.3s;
  }
  .lg:hidden {
    display: none;
  }
  @media (min-width: 1024px) {
    .lg:hidden {
      display: block;
    }
  }
  .absolute {
    position: absolute;
  }
  .right-0 {
    right: 0;
  }
  .w-2-3 {
    width: 66.666667%;
  }
  .bg-primary {
    background-color: #3490dc;
  }
  .py-4 {
    padding-top: 1rem;
    padding-bottom: 1rem;
  }
  .px-8 {
    padding-left: 2rem;
    padding-right: 2rem;
  }
  .shadow {
    box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
  }
  .md:w-1-3 {
    width: 33.333333%;
  }
  @media (min-width: 768px) {
    .md:w-1-3 {
      width: 33.333333%;
    }
  }
  .mt-4 {
    margin-top: 1rem;
  }
  .mr-4 {
    margin-right: 1rem;
  }
  .h-10 {
    height: 2.5rem;
  }
  .w-auto {
    width: auto;
  }
  .mt-8 {
    margin-top: 2rem;
  }
  .flex {
    display: flex;
  }
  .flex-col {
    flex-direction: column;
  }
  .py-2 {
    padding-top: 0.5rem;
    padding-bottom: 0.5rem;
  }
  .cursor-pointer {
    cursor: pointer;
  }
  .pt-1-2 {
    padding-top: 0.125rem;
  }
  .font-header {
    font-family: 'Header', sans-serif;
  }
  .font-semibold {
    font-weight: 600;
  }
  .uppercase {
    text-transform: uppercase;
  }
  .text-white {
    color: white;
  }
</style>
