<template>
  <h1>Vue クイズ</h1>
  <div class="app">
    <h2>Q. {{ "私たちのグループ名は？" }}</h2>
    <img
      class="quiz-image"
      src="https://via.placeholder.com/300x300"
      alt="クイズタイトル"
    />
    <div class="container">
      <button>
        {{ choice1 }}
      </button>
      <button>
        {{ "愉快な腹減り" }}
      </button>
      <button>
        {{ "ばりばりきゃりーん" }}
      </button>
    </div>
    <div>{{ "ばりばりきゃりーん" }}</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      choice1: "きゃいーん",
    }
  },
}
</script>

<style>
.app {
  display: flex;
  width: 100%;
  flex-direction: column;
  align-items: center;
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}

.quiz-image {
  height: 300px;
  width: 300px;
  object-fit: contain;
}

.container {
  display: flex;
  height: 2em;
  width: 300px;
  padding: 1em;
  justify-content: space-around;
}
</style>
