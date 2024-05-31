<script>
  export let mobileMenu;
  export let triggerNavItem;
</script>

<div class="w-full z-50 top-0 py-3 sm:py-5 absolute">
  <div class="container flex items-center justify-between">
    <div>
      <a href="/">
        <img src="../../public/img/logo.svg" class="w-24 lg:w-48" alt="logo image" />
      </a>
    </div>
    <div class="hidden lg:block">
      <ul class="flex items-center">
        <li class="group pl-6">
          <button
            on:click={() => triggerNavItem('#about')}
            on:keydown={(e) => (e.key === 'Enter' || e.key === ' ') && triggerNavItem('#about')}
            class="cursor-pointer pt-0.5 font-header font-semibold uppercase text-white"
            aria-label="About"
          >
            About
          </button>
          <span class="block h-0.5 w-full bg-transparent group-hover:bg-yellow"></span>
        </li>

        <li class="group pl-6">
          <button
            on:click={() => triggerNavItem('#services')}
            on:keydown={(e) => (e.key === 'Enter' || e.key === ' ') && triggerNavItem('#services')}
            class="cursor-pointer pt-0.5 font-header font-semibold uppercase text-white"
            aria-label="Services"
          >
            Services
          </button>
          <span class="block h-0.5 w-full bg-transparent group-hover:bg-yellow"></span>
        </li>

        <li class="group pl-6">
          <button
            on:click={() => triggerNavItem('#portfolio')}
            on:keydown={(e) => (e.key === 'Enter' || e.key === ' ') && triggerNavItem('#portfolio')}
            class="cursor-pointer pt-0.5 font-header font-semibold uppercase text-white"
            aria-label="Portfolio"
          >
            Portfolio
          </button>
          <span class="block h-0.5 w-full bg-transparent group-hover:bg-yellow"></span>
        </li>

        <li class="group pl-6">
          <button
            on:click={() => triggerNavItem('#clients')}
            on:keydown={(e) => (e.key === 'Enter' || e.key === ' ') && triggerNavItem('#clients')}
            class="cursor-pointer pt-0.5 font-header font-semibold uppercase text-white"
            aria-label="Clients"
          >
            Clients
          </button>
          <span class="block h-0.5 w-full bg-transparent group-hover:bg-yellow"></span>
        </li>

        <li class="group pl-6">
          <button
            on:click={() => triggerNavItem('#work')}
            on:keydown={(e) => (e.key === 'Enter' || e.key === ' ') && triggerNavItem('#work')}
            class="cursor-pointer pt-0.5 font-header font-semibold uppercase text-white"
            aria-label="Work"
          >
            Work
          </button>
          <span class="block h-0.5 w-full bg-transparent group-hover:bg-yellow"></span>
        </li>

        <li class="group pl-6">
          <button
            on:click={() => triggerNavItem('#statistics')}
            on:keydown={(e) => (e.key === 'Enter' || e.key === ' ') && triggerNavItem('#statistics')}
            class="cursor-pointer pt-0.5 font-header font-semibold uppercase text-white"
            aria-label="Statistics"
          >
            Statistics
          </button>
          <span class="block h-0.5 w-full bg-transparent group-hover:bg-yellow"></span>
        </li>

        <li class="group pl-6">
          <button
            on:click={() => triggerNavItem('#blog')}
            on:keydown={(e) => (e.key === 'Enter' || e.key === ' ') && triggerNavItem('#blog')}
            class="cursor-pointer pt-0.5 font-header font-semibold uppercase text-white"
            aria-label="Blog"
          >
            Blog
          </button>
          <span class="block h-0.5 w-full bg-transparent group-hover:bg-yellow"></span>
        </li>

        <li class="group pl-6">
          <button
            on:click={() => triggerNavItem('#contact')}
            on:keydown={(e) => (e.key === 'Enter' || e.key === ' ') && triggerNavItem('#contact')}
            class="cursor-pointer pt-0.5 font-header font-semibold uppercase text-white"
            aria-label="Contact"
          >
            Contact
          </button>
          <span class="block h-0.5 w-full bg-transparent group-hover:bg-yellow"></span>
        </li>
      </ul>
    </div>
    <div class="block lg:hidden">
      <button on:click={() => (mobileMenu = true)} aria-label="Open menu">
        <i class="bx bx-menu text-4xl text-white"></i>
      </button>
    </div>
  </div>
</div>
