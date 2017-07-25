<template>
  <div>
    <img src="../assets/logo.png" @click="onClick">
      <h1>
          {{msg}} - {{num}}
      </h1>
      <button @click="onPlusNumber">PLUS</button>
      <button @click="onMinusNumber">MINUS</button>
  </div>
</template>

<script>
export default {
  name: 'Profile',
  data () {
    return {
      msg: 'Jarn jai Yen',
      num: 1
    }
  },
  methods: {
    onClick () {
      alert('Jarn Jai Yen')
    },
    onPlusNumber () {
      this.num = this.num + 1
      this.alertfunction()
    },
    onMinusNumber () {
      this.num = this.num - 1
      this.alertfunction()
    },
    alertfunction () {
      if (this.num === 10 || this.num === -10) {
        alert('HELLO')
      }
    }
  }
}
</script>
