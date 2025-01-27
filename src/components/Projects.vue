<template>
    <section class="projects">
      <h2>My Projects</h2>
      <div class="project-list">
        <div v-for="project in projects" :key="project.title" class="project-item">
          <h3>{{ project.title }}</h3>
          <p>{{ project.description }}</p>
          <a :href="project.link" target="_blank">View Project</a>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: "Projects",
    data() {
      return {
        projects: [
          {
            title: "Machine Learning Dashboard",
            description: "A web-based dashboard for ML model visualization.",
            link: "https://example.com/ml-dashboard"
          },
          {
            title: "Stock Market Prediction",
            description: "Using deep learning to predict stock market trends.",
            link: "https://example.com/stock-prediction"
          },
          {
            title: "Data Science Portfolio",
            description: "A collection of my data science projects.",
            link: "https://example.com/ds-portfolio"
          }
        ]
      };
    }
  };
  </script>
  
  <style src="../assets/styles/projects.css"></style>
  