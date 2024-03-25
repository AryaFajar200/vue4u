<template>
  <nav class="bg-white p-4 flex justify-between items-center">
    <!-- Logo di kiri -->
    <div class="flex items-center">
      <img src="https://cdn.discordapp.com/attachments/1161941560070516750/1171657532876529685/image.png?ex=660cd19c&is=65fa5c9c&hm=f8b0629722c3fbda59978bc4f25e524e0a09e97a82d2f3d9f4f062b844695a43&"
           alt="Logo" class="h-8 mr-2">
      <span class="text-lg font-semibold font-poppins">Nama Situs</span>
    </div>

    <!-- List menu di tengah -->
    <ul class="flex justify-center space-x-4">
      <RouterLink to="/" class="nav-item nav-link hover:text-[#32D316] font-poppins nav-link" :class="{ active: $route.path === '/' }">Home</RouterLink>
      <RouterLink to="/about" class="nav-item nav-link hover:text-[#32D316] font-poppins nav-link" :class="{ active: $route.path === '/about' }">About</RouterLink>

    </ul>

    <!-- Tombol "Read More" di kanan -->
    <button class="bg-[#32D316] hover:bg-blue-700 text-white font-bold py-2 px-4 rounded font-poppins">
      Read More
    </button>
  </nav>
  <hr>
  <RouterView />
</template>

<style scoped>
  /* Styling tambahan sesuai kebutuhan */
  .font-poppins {
    font-family: 'Poppins', sans-serif;
  }

  .nav-link {
    /* Warna teks link */
    transition: border-bottom-color 0.3s;
    /* Efek transisi perubahan garis bawah */
    border-bottom: 2px solid transparent; /* Garis bawah awalnya transparan */
  }

  .nav-link:hover, .nav-link.active {
    border-bottom-color: black; /* Garis bawah akan berwarna hitam saat dihover atau aktif */
  }
</style>
