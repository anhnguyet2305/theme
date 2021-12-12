<template>
  <section class="job-list-container">
    <section class="job-list">
      <JobItems/>
      <JobItems/>
      <JobItems/>
      <JobItems/>
    </section>
    <button  class="job-list-button" >Load More</button>
  </section>
</template>

<script>
import JobItems from "@/components/JobItems";
export default {
  name: "JobsList",
  components: {JobItems}
}
</script>

<style scoped>
  .job-list-container{
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-bottom: 100px;
  }
  .job-list {
    width: 100%;
    display: flex;
    flex-wrap: wrap;
    margin-bottom: 16px;
  }
  .job-list-button{
    font-style: normal;
    font-weight: bold;
    font-size: 16px;
    line-height: 16px;
    text-align: center;
    color: white;
    background-color: #5964e0;
    border-radius: 5px;
    padding: 16px 20px;
    min-width: 141px;
    cursor: pointer;
    appearance: none;
    border: none;
    outline: none;
    transition: background-color ease-out .2s;
    text-decoration: none;
  }
  .job-list-button:hover{
    background-color: #939BF4;
  }
</style>