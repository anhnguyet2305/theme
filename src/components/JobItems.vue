<template>
  <div class="job-item">
    <a href="#">
      <section class="job-logo-container">
        <img src="https://devjobs-web-app-5toyf4pub-david-maillard.vercel.app/assets/logos/scoot.svg" alt="Scoot"
             class="job-logo">
      </section>
      <section class="job-info">
        <p class="job-post"><span>5h ago</span><span>Full Time</span></p>
        <p class="job-title">Senior Software Engineer</p>
        <p class="job-company">Scoot</p>
      </section>
      <p class="job-country">United Kingdom</p>
    </a>
  </div>
</template>

<script>
export default {
  name: "JobItems"
}
</script>

<style scoped>
.job-item {
  position: relative;
  width: calc((1200px - 252px) / 3);
  margin-right: 30px;
  margin-top: 25px;
  background: #ffffff;
  border-radius: 6px;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  min-height: 160px;
  padding: 50px 32px 32px;
  margin-bottom: 40px;
  text-decoration: none;
}
.job-item:nth-child(3n+3){
  margin-right: 0;
}
.job-item a{
  text-decoration: none;
}

.job-logo-container {
  width: 50px;
  height: 50px;
  position: absolute;
  left: 32px;
  top: -25px;
  border-radius: 15px;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #5964e0;
}

.job-logo {
  max-width: calc(100% - 10px);
  max-height: 20px;
}
.job-info{
  flex: 1;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  margin-bottom: 50px;
}
.job-post{
  display: flex;
  align-items: center;
  margin: 0 0 16px;
}
.job-post span{
  display: flex;
  align-items: center;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 16px;
  color: #6E8098;
}
.job-post:first-child:after{
  content: '';
  display: flex;
  margin: 0 12px;
  width: 4px;
  height: 4px;
  border-radius: 4px;
  background-color: #6E8098;
}
.job-title {
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
  line-height: 20px;
  color: #19202D;
  margin: 0 0 16px;
}
.job-company {
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 16px;
  color: #6E8098;
  margin: 0;
}
.job-country {
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
  line-height: 14px;
  color: #5964e0;
}
</style>