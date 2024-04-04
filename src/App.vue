<template>
  <div class="navbar bg-base-100 sticky border-b-2 border-grey-200">
    <div class="navbar-start">
      <div class="dropdown">
        <div tabindex="0" role="button" class="btn btn-ghost lg:hidden">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-5 w-5"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M4 6h16M4 12h8m-8 6h16"
            />
          </svg>
        </div>
        <ul
          tabindex="0"
          class="menu menu-sm dropdown-content mt-3 z-[1] p-2 shadow bg-base-100 rounded-box w-52"
        >
          <RouterLink
            to="/"
            class="nav-item nav-link hover:text-[#32D316] font-poppins nav-link"
            :class="{ active: $route.path === '/' }"
            >Home</RouterLink
          >
          <RouterLink
            to="/about"
            class="nav-item nav-link hover:text-[#32D316] font-poppins nav-link"
            :class="{ active: $route.path === '/about' }"
            >About</RouterLink
          >
        </ul>
      </div>
      <img
        src="@/assets/images/SIA LOGO MEDIUM.svg"
        alt="DaisyUI Logo"
        class="btn btn-ghost text-xl"
      />
    </div>
    <div class="navbar-center hidden lg:flex">
      <ul class="menu menu-horizontal px-8 space-x-4">
        <RouterLink
          to="/"
          class="nav-item nav-link hover:text-[#32D316] font-poppins nav-link px-4"
          :class="{ active: $route.path === '/' }"
          >Home</RouterLink
        >

        <RouterLink
          to="/about"
          class="nav-item nav-link hover:text-[#32D316] font-poppins nav-link px-4"
          :class="{ active: $route.path === '/about' }"
          >About</RouterLink
        >
      </ul>
    </div>
    <div class="navbar-end">
      <a class="btn bg-[#32d316] text-white font-extrabold">MORE</a>
    </div>
  </div>
  <RouterView />
</template>
sc
<style scoped>
/* Styling tambahan sesuai kebutuhan */
.font-poppins {
  font-family: "Poppins", sans-serif;
}

.nav-link {
  /* Warna teks link */
  transition: border-bottom-color 0.3s;
  /* Efek transisi perubahan garis bawah */
  border-bottom: 2px solid transparent; /* Garis bawah awalnya transparan */
}

.nav-link:hover,
.nav-link.active {
  border-bottom-color: black; /* Garis bawah akan berwarna hitam saat dihover atau aktif */
}

.sticky {
  position: fixed;
  width: 100%;
  top: 0;
  left: 0;
  z-index: 1000;
}
</style>
