<template>
  <div>
    <Header/>
    <div class="container">
      <JobsList/>
    </div>
  </div>
</template>

<script>
import '@fortawesome/fontawesome-free/css/all.css'
import '@fortawesome/fontawesome-free/js/all.js'
import Header from "@/components/Header";
import JobsList from "@/components/JobsList";

export default {
  name: "Home",
  components: {JobsList, Header}
}

</script>
<style scoped>

</style>