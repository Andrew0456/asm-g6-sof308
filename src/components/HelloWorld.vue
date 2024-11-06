<template>
  <h1>{{ greeting }}</h1>
  <button :title="buttonTitle" @click="changeTitle">Click để thay đổi lời chào</button>
</template>
<script>
export default {
  data() {
    return {
      greeting: 'Xin chào bạn!',
      buttonTitle: 'Nhấn để thay đổi lời chào'
    };
  },
  methods: {
    changeTitle() {
      this.greeting = 'Hello, World!';
      this.buttonTitle = 'Lời chào mới đã được cập nhật';
    }
  }
}
</script>