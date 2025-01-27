<template>
    <section class="skills">
      <h2>Skills</h2>
      <div class="skills-list">
        <div v-for="skill in skills" :key="skill.name" class="skill-item">
          <img :src="skill.icon" alt="Skill icon" class="skill-icon" />
          <div class="skill-info">
            <h3>{{ skill.name }}</h3>
            <p>{{ skill.description }}</p>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    data() {
      return {
        skills: [
          { name: "Python", icon: "/icons/python.svg", description: "Data analysis, ML, AI." },
          { name: "R", icon: "/icons/r.svg", description: "Statistical analysis, visualization." },
          { name: "TensorFlow", icon: "/icons/tensorflow.svg", description: "Deep learning models." },
          { name: "SQL", icon: "/icons/sql.svg", description: "Data extraction, queries." }
        ]
      };
    }
  };
  </script>
  
  <style src="../assets/styles/skills.css"></style>
  