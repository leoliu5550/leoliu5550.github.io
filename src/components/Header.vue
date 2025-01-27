<template>
  <header>
    <div class="header-container">
      <img src="../assets/image/meandcf.jpg" alt="Leo Liu pic" class="picture" />

      <div class="header-text">
        <div class="name">
        <h1 class="title">Leo Liu Resume</h1>
        </div>
        <div class="description_list">
        <nav>
          <router-link to="/">Home</router-link> <!-- router-link 生成一個 <a> 標籤 -->
          <router-link to="/about">About</router-link>
          <router-link to="/skills">Skills</router-link>
          <router-link to="/projects">Projects</router-link>
          <router-link to="/contact">Contact</router-link>
        </nav>
        </div>
      </div>

    </div>
  </header>
</template>

<script>
export default {
  name: "Header"
};
</script>

<style src="../assets/styles/header.css"></style>