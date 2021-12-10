<template>
  <div>
    <v-item-group active-class="primary">
      <v-container>
        <v-row>
          <v-col cols="6">
            {{first}}
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 792.452 399.043"
            >
              <v-item v-slot="{ active, toggle }">
                <path
                  id="Path_1"
                  data-name="Path 1"
                  @click="toggle"
                  :fill="first && !active ? '#999' : 'red'"
                  d="M802.781,515.47,873.2,482.607l56.335,85.442L848.788,619.69Z"
                  transform="translate(-553.027 -426.272)"
                />
              </v-item>
              <v-item v-slot="{ active, toggle }">
                <path
                  id="Path_2"
                  data-name="Path 2"
                  @click="toggle"
                  :fill="!active ? '#999' : 'red'"
                  d="M888.223,477.913l63.847,91.076,97.648-17.84-30.985-102.343Z"
                  transform="translate(-553.027 -426.272)"
                />
              </v-item>
              <v-item v-slot="{ active, toggle }">
                <path
                  id="Path_3"
                  data-name="Path 3"
                  @click="toggle"
                  :fill="!active ? '#999' : 'red'"
                  d="M1060.046,453.5l16.9,92.954,121.121,7.511-7.511-127.694-130.51,5.634Z"
                  transform="translate(-553.027 -426.272)"
                />
              </v-item>
              <v-item v-slot="{ active, toggle }">
                <path
                  id="Path_4"
                  data-name="Path 4"
                  @click="toggle"
                  :fill="!active ? '#999' : 'red'"
                  d="M1239.381,430.028l-6.572,125.816L1328.578,615l16.9-142.717Z"
                  transform="translate(-553.027 -426.272)"
                />
              </v-item>
              <v-item v-slot="{ active, toggle }">
                <path
                  id="Path_5"
                  data-name="Path 5"
                  @click="toggle"
                  :fill="!active ? '#999' : 'red'"
                  d="M787.758,531.431,676.026,601.851l62.908,104.221,95.77-71.358Z"
                  transform="translate(-553.027 -426.272)"
                />
              </v-item>
              <v-item v-slot="{ active, toggle }">
                <path
                  id="Path_6"
                  data-name="Path 6"
                  @click="toggle"
                  :fill="!active ? '#999' : 'red'"
                  d="M662.881,615l-109.854,78.87,92.015,131.449,86.381-94.831Z"
                  transform="translate(-553.027 -426.272)"
                />
              </v-item>
            </svg>
          </v-col>
          <v-col>
            <v-text-field v-model="value" solo></v-text-field>
            <v-text-field v-model="value" solo></v-text-field>
            <v-text-field v-model="value" solo></v-text-field>
            <v-text-field v-model="value" solo></v-text-field>
          </v-col>
        </v-row>
      </v-container>
    </v-item-group>
  </div>
</template>

<script>
export default {
  components: {},
  methods: {
    openTest(val) {
      this.value = val
    },
  },
  data: () => ({
    items: [
      { title: "Click Me" },
      { title: "Click Me" },
      { title: "Click Me" },
      { title: "Click Me 2" },
    ],
    value: null,
    first: false
  }),
};
</script>
