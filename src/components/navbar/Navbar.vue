<script setup>
</script>

<template>
  <nav>
    <div class="nav-section">
      <div class="first-nav-section">
        <div class="user-section">
          <svg
            class="svg"
            width="35"
            height="35"
            viewBox="0 0 32 32"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M10.5 11c0-1.657 1.343-3 3-3h5c1.657 0 3 1.343 3 3 0 1.043-.533 1.963-1.341 2.5.808.537 1.341 1.457 1.341 2.5 0 1.657-1.343 3-3 3-.768 0-1.47-.289-2-.764V21c0 1.657-1.343 3-3 3-1.657 0-3-1.343-3-3 0-1.044.533-1.962 1.341-2.5-.808-.538-1.341-1.456-1.341-2.5 0-1.043.533-1.963 1.341-2.5-.808-.537-1.341-1.457-1.341-2.5zm3 2c-1.105 0-2-.895-2-2 0-1.105.895-2 2-2h2v4h-2zm2 1h-2c-1.105 0-2 .895-2 2 0 1.105.895 2 2 2h2v-4zm0 5h-2c-1.105 0-2 .895-2 2 0 1.105.895 2 2 2 1.105 0 2-.895 2-2v-2zm3-5c-1.105 0-2 .895-2 2 0 1.105.895 2 2 2 1.105 0 2-.895 2-2 0-1.105-.895-2-2-2zm0-1c1.105 0 2-.895 2-2 0-1.105-.895-2-2-2h-2v4h2z"
              fill-rule="evenodd"
              fill-opacity="1"
              fill="#fff"
              stroke="none"
            ></path>
          </svg>
          <div>
            <p>Afzalbek Orifjonov</p>
            <h6>uzafo.dev@gmail.com</h6>
          </div>
        </div>
        <div class="search-panel">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="16"
            height="16"
            fill="currentColor"
            class="bi bi-search"
            viewBox="0 0 16 16"
          >
            <path
              d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z"
            />
          </svg>
          <input type="text" placeholder="Search files, teams or people" />
        </div>
      </div>

      <div class="second-nav-section">
        <div class="ball-svg">
          <svg
            class="svg"
            width="35"
            height="35"
            viewBox="0 0 32 32"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M20 14v3c0 .768.289 1.47.764 2h-9.528c.475-.53.764-1.232.764-2v-3c0-2.21 1.79-4 4-4 2.21 0 4 1.79 4 4zm1 0v3c0 1.105.895 2 2 2v1H9v-1c1.105 0 2-.895 2-2v-3c0-2.761 2.239-5 5-5 2.761 0 5 2.239 5 5zm-5 9c-1.105 0-2-.895-2-2h-1c0 1.657 1.343 3 3 3 1.657 0 3-1.343 3-3h-1c0 1.105-.895 2-2 2z"
              fill-rule="evenodd"
              fill-opacity="1"
              fill="#dadada"
              stroke="none"
            ></path>
          </svg>
        </div>
        <div class="item-section">
          <a href="https://afzalbek.netlify.app/" target="__blank">A</a>
          <span>></span>
        </div>
      </div>
    </div>
  </nav>
</template>

<style scoped>
nav {
  background: #2c2c2c;
  color: white;
  font-size: 16px;
  padding: 0 5px;
  position: fixed;
  width: 100%;
}
.nav-section {
  display: flex;
  align-items: center;
  margin: 3px 0;
}
.nav-section .first-nav-section {
  display: flex;
  align-items: center;
  justify-content: start;
  width: 50%;
}
.nav-section .second-nav-section {
  display: flex;
  width: 50%;
  justify-content: end;
  align-items: center;
}
.user-section {
  display: flex;
  align-items: center;
  width: 225px;
  color: white;
  font-size: 12px;
  font-family: sans-serif;
  font-weight: bold;
  margin-right: 25px;
  border-right: 1px solid #797777;
}
.user-section:hover {
  background: #000;
  padding: 1px;
  border-radius: 5px;
  transition-delay: 200ms;
}
.user-section h6 {
  color: #7e7e7e;
  font-size: 10px;
}

.search-panel {
  display: flex;
  align-items: center;
  height: 38px;
  border-radius: 5px;
  padding: 5px;
}
.search-panel input {
  background: none;
  outline: none;
  border: none;
  width: 300px;
  color: white;
  margin-left: 15px;
}
.search-panel:hover {
  background: #585858;
}
.search-panel:active {
  background: #585858;
}
/* Second section */
.second-nav-section span {
  transform: rotate(90deg);
  font-size: 14px;
}
.second-nav-section a {
  background: red;
  text-decoration: none;
  color: white;
  height: 30px;
  width: 30px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 50%;
  font-size: 14px;
  margin: 0 8px;
}
.item-section {
  display: inline-flex;
  align-items: center;
  margin: 0 15px;
  padding: 5px;
}
.ball-svg {
  margin-right: 40px;
}
.ball-svg:hover {
  background: black;
}
.item-section:hover {
  background: black;
}
</style>