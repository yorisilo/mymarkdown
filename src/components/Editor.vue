<template>
<div class="editor">
  <h1>Editor UI</h1>
  <span>{{ user.displayName }}</span>
  <button @click="logout">logout</button>
</div>
</template>

<script>
export default {
  name: "editor",
  props: ["user"],
  data() {
    return {}
  },
  methods: {
    logout: function() {
      firebase.auth().signOut()
    }
  }
}
</script>
