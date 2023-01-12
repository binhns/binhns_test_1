<template>
  <div class="w-full">
    <ul class="flex mb-0 list-none flex-wrap flex-row">
      <li>
        <a class="toggler" v-on:click="toggleTabs(1)" v-bind:class="{
          '': openTab !== 1,
          'active': openTab === 1,
        }">
          <div class="wrapper">

            <img src="../assets/img/tabs/icon_pencils.png" alt="" />

            <div class="text">Pencils</div>
          </div>
        </a>
        <div class="tab-content md:hidden" v-bind:class="{ hidden: openTab !== 1, block: openTab === 1 }">
          <Tab1 />
        </div>
      </li>
      <li>
        <a class="toggler" v-on:click="toggleTabs(2)" v-bind:class="{
          '': openTab !== 2,
          'active': openTab === 2,
        }">
          <div class="wrapper">

            <img src="../assets/img/tabs/icon_marker.png" alt="" />

            <div class="text">Markers</div>
          </div>
        </a>
        <div class="tab-content md:hidden" v-bind:class="{ hidden: openTab !== 2, block: openTab === 2 }">
          This is Tab 2: Markers
        </div>
      </li>
      <li>
        <a class="toggler" v-on:click="toggleTabs(3)" v-bind:class="{
          '': openTab !== 3,
          'active': openTab === 3,
        }">
          <div class="wrapper">

            <img src="../assets/img/tabs/icon_drawingcolors.png" alt="" />

            <div class="text">Drawing Colors</div>
          </div>
        </a>
        <div class="tab-content md:hidden" v-bind:class="{ hidden: openTab !== 3, block: openTab === 3 }">
          This is Tab 3: Drawing Colors
        </div>
      </li>
      <li>
        <a class="toggler" v-on:click="toggleTabs(4)" v-bind:class="{
          '': openTab !== 4,
          'active': openTab === 4,
        }">
          <div class="wrapper">

            <img src="../assets/img/tabs/icon_notebook.png" alt="" />

            <div class="text">Notebooks</div>
          </div>
        </a>
        <div class="tab-content md:hidden" v-bind:class="{ hidden: openTab !== 4, block: openTab === 4 }">
          This is Tab 4: Notebooks
        </div>
      </li>
    </ul>

    <div class="tab-content tab-space hidden md:block">
      <div v-bind:class="{ hidden: openTab !== 1, block: openTab === 1 }">
        <Tab1 />
      </div>
      <div v-bind:class="{ hidden: openTab !== 2, block: openTab === 2 }">
        This is Tab 2: Markers
      </div>
      <div v-bind:class="{ hidden: openTab !== 3, block: openTab === 3 }">
        This is Tab 3: Drawing Colors
      </div>
      <div v-bind:class="{ hidden: openTab !== 4, block: openTab === 4 }">
        This is Tab 4: Notebooks
      </div>
    </div>
  </div>

</template>

<script>
import Tab1 from "./Tab1.vue";

export default {
  name: "TheTabs",
  data() {
    return {
      openTab: 1,
    };
  },
  components: {
    Tab1
  },

  methods: {
    toggleTabs: function (tabNumber) {
      this.openTab = tabNumber;
    },
  },
};
</script>

<style scoped>
.toggler {

  border-radius: 25px 25px 0px 0px;
  display: block;
  padding: 32px 31px 28px 34px;

  font-family: 'Poppins', sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 21px;
  line-height: 32px;

  text-align: center;

  color: #181818;
  transition: all 0.5;
  background-color: #fff;

}

.toggler .wrapper {
  width: 235px;
  height: 140px;
  margin: auto;
  background: #FFFFFF;
  box-shadow: 0px 0px 27px rgba(0, 0, 0, 0.05);
  border-radius: 10px;
  padding: 23px 0;
  text-align: center;
  cursor: pointer;
}

.toggler .wrapper img {
  margin: auto;
  margin-bottom: 4px;
  width: 58px;
  height: 58px;
  object-fit: scale-down;

  border-radius: 100%;
  background: #F4F4F4;
}

.toggler.active {
  background-color: #F4F4F4;
}


.tab-content {
  background: #F4F4F4;
  border-radius: 0px 0px 25px 25px;

  padding: 40px 50px;
}

@media (max-width: 767px) {
  ul.flex li {
    margin-bottom: 10px;
  }

  .toggler {
    padding: 11px;
    background: #F4F4F4;
    border-radius: 18px;
  }

  .toggler.active {
    border-radius: 18px 18px 0 0;
  }

  .toggler .wrapper {
    width: 368px;
    height: 80px;
    display: flex;
    justify-content: flex-start;
    align-items: center;
    padding: 20px 30px;

    font-family: 'Poppins', sans-serif;
    font-style: normal;
    font-weight: 700;
    font-size: 21px;
    line-height: 32px;
  }

  .toggler .wrapper img {
    margin: initial;
    margin-right: 20px;
  }

  .tab-content {
    padding: 11px 21px;
  }
}
</style>
