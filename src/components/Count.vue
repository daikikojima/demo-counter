<template>
  <div>
    <h1>Count</h1>
    <h2>{{ count }}</h2>
    <div class="button-box">
      <button class="add" @click="add">+</button>
      <button class="minus" @click="minus">-</button>
    </div>
  </div>
</template>
<script>
export default {
  name: "Count",
  data() {
    return {
      count: 0
    };
  },
  methods: {
    add() {
      this.count += 1;
    },
    minus() {
      this.count -= 1;
    }
  }
};
</script>
<style scoped>
h1 {
  font-size: 8em;
}

h2 {
  font-size: 7.5em;
}
.button-box {
  display: flex;
  height: 100px;
  justify-content: space-around;
}
button {
  color: white;
  font-size: 5em;
  height: 100%;
  width: 40%;
}

.add {
  background: #26f;
}

.minus {
  background: #f26;
}
</style>
