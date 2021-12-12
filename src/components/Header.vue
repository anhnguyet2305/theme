<template>
  <div class="Header">
    <div class="container">
      <a href="/" class="logo">
        devJobs
      </a>
      <div class="header-filters">
        <input type="search" placeholder="Filter by title, companies, expertise…" class="search-input">
        <select class="location-input">
          <option value="false">Filter by location…</option>
          <option value="Germany">Germany</option>
          <option value="Japan">Japan</option>
          <option value="New Zealand">New Zealand</option>
          <option value="Russia">Russia</option>
          <option value="Singapore">Singapore</option>
          <option value="United Kingdom">United Kingdom</option>
          <option value="United States">United States</option>
        </select>
        <label class="type-filter-container">
          <input type="checkbox">
          <span>Full Time Only</span>
          <button class="filter-button"><p>Search</p></button>
        </label>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header"
}
</script>

<style scoped>

.Header {
  margin-bottom: 100px;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
  width: 100%;
  flex-direction: column;
  min-height: 122px;
  padding-top: 55px;
  background-image: url("https://devjobs-web-app-5toyf4pub-david-maillard.vercel.app/img/bg-pattern-header.549c5470.svg");
}

.logo {
  font-size: 30px;
  color: #fff;
  text-decoration: none;
  align-items: start;
  font-weight: 600;
}

.header-filters {
  width: 100%;
  display: flex;
  justify-content: center;
  border-radius: 6px;
  overflow: hidden;
  position: absolute;
  max-width: 1200px;
  top: 140px;
  background-color: white;
}

.search-input {
  flex: 2;
  padding: 32px 32px 32px 56px;
  background-image: url("data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik0xNi4wMjQgMTUuMDU5aDEuMDg4bDYuODMyIDYuODQ1LTIuMDQgMi4wNC02Ljg0NS02LjgzMnYtMS4wODFsLS4zNzctLjM3N2E4Ljg0NCA4Ljg0NCAwIDAgMS01Ljc4NCAyLjE0M0E4Ljg5OCA4Ljg5OCAwIDAgMSAwIDguODk4IDguODk4IDguODk4IDAgMCAxIDguODk4IDBhOC44OTggOC44OTggMCAwIDEgOC44OTkgOC44OThjMCAyLjIxMS0uODA4IDQuMjMtMi4xNSA1Ljc4NGwuMzc3LjM3N1pNMi43MzggOC44OTlhNi4xNiA2LjE2IDAgMSAwIDEyLjMyMi0uMDAyIDYuMTYgNi4xNiAwIDAgMC0xMi4zMjIuMDAxWiIgZmlsbD0iIzU5NjRFMCIvPjwvc3ZnPg==");
  background-position: left 24px center;
  background-size: 16px 24px;
  background-repeat: no-repeat;
  border: none;
  appearance: none;
  outline: none;
  border-right: 1px solid rgba($ darkGrey, .2);
  cursor: pointer;
  border-right: #f2f2f2 1px solid;
}

.location-input {
  flex: 1;
  padding: 32px 32px 32px 56px;
  background-image: url("data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAxNyAyNCI+PHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik04LjQ0OCAwYTguMyA4LjMgMCAwIDEgNS45MSAyLjQ1MWMyLjkyMiAyLjkyNSAzLjI4NSA4LjQyNy43NzcgMTEuNzc0bC02LjY4NyA5LjY2OS02LjY5Ny05LjY4MmMtMi40OTktMy4zMzQtMi4xMzYtOC44MzYuNzg2LTExLjc2QTguMyA4LjMgMCAwIDEgOC40NDcgMFpNNS40NzQgOC4yOWEzLjA1NyAzLjA1NyAwIDAgMCAzLjA1IDMuMDU2IDMuMDU3IDMuMDU3IDAgMCAwIDMuMDUyLTMuMDU1IDMuMDU3IDMuMDU3IDAgMCAwLTMuMDUxLTMuMDU1IDMuMDU3IDMuMDU3IDAgMCAwLTMuMDUxIDMuMDU1WiIgZmlsbD0iIzU5NjRFMCIvPjwvc3ZnPg==");
  background-position: left 24px center;
  background-size: 16px 24px;
  background-repeat: no-repeat;
  border: none;
  appearance: none;
  outline: none;
  cursor: pointer;
  border-right: #f2f2f2 1px solid;
}
.type-filter-container{
  margin-left: 32px;
  margin-right: 26px;
  display: flex;
  align-items: center;
  flex-shrink: 0;
  cursor: pointer;
}
.type-filter-container span{
  position: relative;
  display: flex;
  align-items: center;
  font-weight: bold;
  flex-shrink: 0;
}
.type-filter-container span:before{
  content: '';
  width: 24px;
  height: 24px;
  margin-right: 16px;
  background-color: #5964e0;
  border-radius: 3px;
}

.type-filter-container span:after{
  position: absolute;
  left: 0;
  top: 50%;
  transform: translateY(-50%);
  content: '';
  width: 24px;
  height: 24px;
  background-image: url("data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAxNSAxMiI+PHBhdGggZD0ibTEgNi41NyAzLjU3MiAzLjU3MkwxMy43MTQgMSIgc3Ryb2tlPSIjZmZmIiBzdHJva2Utd2lkdGg9IjIiLz48L3N2Zz4=");
  background-size: 12px 10px;
  background-position: center center;
  background-repeat: no-repeat;
  opacity: 0;
}
.type-filter-container input[type="checkbox"]{
  display: none;
}
.type-filter-container input[type="checkbox"]:checked + span:before{
  background-color: #5964e0;
}
.type-filter-container input[type="checkbox"]:checked + span:after{
  opacity: 1;
}
.filter-button{
  min-width: 120px;
  margin-left: 20px;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  text-align: center;
  color: white;
  background-color: #5964e0;
  border-radius: 5px;
  max-width: 141px;
  cursor: pointer;
  appearance: none;
  border: none;
  outline: none;
  transition: background-color ease-out .2s;
  text-decoration: none;
}
</style>