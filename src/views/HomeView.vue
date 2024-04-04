<template>
  <div>
    <div
      class="hero min-h-screen"
      style="
        background-image: url(https://daisyui.com/images/stock/photo-1507358522600-9f71e620c44e.jpg);
      "
    >
      <div class="hero-overlay bg-opacity-60"></div>
      <div class="hero-content text-center text-neutral-content">
        <div class="max-w-md">
          <h1 class="mb-5 text-5xl font-bold">
            Innovate with Confidence: SIA, Your Trusted Technology Partner.
          </h1>
          <button class="btn bg-[#32d316] text-white font-extrabold">
            GET STARTED
          </button>
        </div>
      </div>
    </div>
    <div class="py-16 px-4 text-center bt-8">
      <h2 class="text-[72px] font-bold pb-8">WHO WE ARE?</h2>
      <h5 class="font-bold mx-auto max-w-2xl">
        At SIA, we are a forward-thinking software development company committed
        to transforming ideas into impactful digital solutions. Our team of
        seasoned professionals combines innovation, expertise, and a
        client-centric approach to deliver tailored software that drives
        business success. With a passion for excellence and a focus on
        collaboration, we stand as a reliable partner for those seeking
        cutting-edge technology solutions. At the core of our identity is a
        dedication to crafting meaningful software experiences that not only
        meet but exceed the expectations of our clients, propelling them
        confidently into the digital future.
      </h5>
    </div>
    <div class="bg-[#101820] rounded-t-[96px]">
      <div class="py-16 px-4 text-center bt-8 text-white">
        <h2 class="text-[72px] font-bold pb-8">Our Points</h2>
        <h5 class="font-bold">
          Lorem, ipsum dolor sit amet consectetur adipisicing elit.
        </h5>
      </div>
      <!-- Kartu Kartu -->

      <div class="flex justify-center space-x-12">
        <!-- Kartu 1 -->
        <div class="card w-96 bg-base-100 shadow-xl">
          <div class="card-body">
            <h2 class="card-title">Cost-Effective Solutions</h2>
            <p>
              While maintaining high quality, we strive to provide
              cost-effective solutions, offering excellent value for our
              clients' investments in software development.
            </p>
            <div class="card-actions justify-end">
              <button class="btn bg-[#32d316] text-white font-extrabold">
                READ MORE
              </button>
            </div>
          </div>
        </div>

        <!-- Kartu 2 -->
        <div class="card w-96 bg-base-100 shadow-xl">
          <div class="card-body">
            <h2 class="card-title">Innovative Solutions</h2>
            <p>
              We pride ourselves on our ability to deliver cutting-edge and
              innovative software solutions tailored to meet the unique needs of
              our clients.
            </p>
            <div class="card-actions justify-end">
              <button class="btn bg-[#32d316] text-white font-extrabold">
                READ MORE
              </button>
            </div>
          </div>
        </div>

        <!-- Kartu 3 -->
        <div class="card w-96 bg-base-100 shadow-xl">
          <div class="card-body">
            <h2 class="card-title">Experienced Team</h2>
            <p>
              Our team of seasoned developers brings a wealth of experience and
              expertise to the table, ensuring the successful execution of even
            </p>
            <div class="card-actions justify-end">
              <button class="btn bg-[#32d316] text-white font-extrabold">
                READ MORE
              </button>
            </div>
          </div>
        </div>
      </div>
      <div><h2 class="text-[72px] font-bold pb-8">Our Points</h2></div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      imageUrl: "https://cdn-site.gojek.com/uploads/hero_b18c33ed07.jpg",
      bannerText:
        "Innovate with Confidence: SIA, Your Trusted Technology Partner.",
    };
  },
};
</script>

<style scoped>
* {
  font-family: "Poppins", sans-serif; /* Menggunakan font Poppins untuk semua teks */
}
.banner {
  position: relative;
  width: 100%;
  height: 100vh;
  overflow: hidden;
}

.banner-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.banner-text {
  position: absolute;
  top: 50%;
  left: 0;
  transform: translateY(-50%);
  color: white;
  text-align: left; /* Align text to the left */
  width: 100%;
  z-index: 1;
}

.banner-text h1 {
  margin-bottom: 10px; /* Menambahkan margin bawah agar teks kedua berada di bawah teks pertama */
}
</style>
