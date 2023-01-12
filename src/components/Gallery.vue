<template>
  <div class="container mx-auto">
    <h2>
      Packer pen Gallery
    </h2>


    <div class="grid items-center grid-flow-col grid-cols-3 grid-rows-1 gap-3 hidden md:flex">
      <div>
        <img class="my-3" src="../assets/img/gallery/Rectangle23.png" alt="image" />
        <img class="my-3" src="../assets/img/gallery/Rectangle25.png" alt="image" />
      </div>
      <div class="col-span-2">
        <img class="my-3" src="../assets/img/gallery/Rectangle21.png" alt="image" />
        <img class="my-3" src="../assets/img/gallery/Rectangle24.png" alt="image" />
      </div>
      <div>
        <div>

          <img class="my-3" src="../assets/img/gallery/Rectangle26.png" alt="image" />
          <img class="my-3" src="../assets/img/gallery/Rectangle27.png" alt="image" />
          <img class="my-3" src="../assets/img/gallery/Rectangle28.png" alt="image" />
        </div>
      </div>
    </div>

    <div class=" md:hidden">
      <div class="grid  grid-cols-2">
        <div>
          <img class="mb-2" src="../assets/img/gallery/Rectangle23_mb.png" alt="image" />
          <img class="mb-2" src="../assets/img/gallery/Rectangle27_mb.png" alt="image" />

        </div>
        <img class="mb-2" src="../assets/img/gallery/Rectangle25_mb.png" alt="image" />

      </div>
      <div class="col-span-2">

        <img class="mb-2" src="../assets/img/gallery/Rectangle24_mb.png" alt="image" />

        <img class="mb-2" src="../assets/img/gallery/Rectangle21_mb.png" alt="image" />
      </div>
      <div>
        <div class="grid  grid-cols-2">
          <img class="mb-2" src="../assets/img/gallery/Rectangle28_mb.png" alt="image" />
          <img class="mb-2" src="../assets/img/gallery/Rectangle26_mb.png" alt="image" />


        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "TheGallery",
  data() {
    return {};
  },
};
</script>

<style scoped>
h2 {
  font-family: 'Poppins', sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 45px;
  line-height: 68px;

  text-align: center;
  text-transform: uppercase;

  color: #121212;

  margin-bottom: 40px;
}

@media(max-width: 767px) {
  h2 {
    font-style: normal;
    font-weight: 700;
    font-size: 30px;
  }
}
</style>