<template>
  <main class="container">
    <code-checker>
      <template #start>
        <start />
      </template>
      <template #loggedIn>
        <landing />
      </template>
    </code-checker>
  </main>
</template>

<script>
import CodeChecker from '../components/CodeChecker'
import Start from '../components/Start'
import Landing from '../components/Landing'
export default {
  components: { Landing, Start, CodeChecker },
  data() {
    return {
      name: '',
    }
  },
  methods: {},
}
</script>
