<template>
  <main>
    <h1>About Me</h1>
    <img src="../assets/portrait.jpg">

    <p>Hello, my name is Digby Harrison-Riley and this is my resume portfolio! I am currently studying a Bachelor and of Information Technology at Deakin University and have a passion for the digital realm. This portfolio will showcase my past projects, where I aspire to be and a little bit about myself.
    </p>

    <h2>Previous Projects</h2>

    <div>
      <table>
        <thead>
          <tr>
            <th>Title</th>
            <th>Image</th>
            <th>Description</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="item in items" :key="item.id">
            <td>{{ item.title }}</td>
            <td><img :src="item.imageUrl" alt="Item Image" /></td>
            <td>{{ item.description }}</td>
          </tr>
        </tbody>
      </table>
    </div>

    <h2>Future Aspirations</h2>
    <p>Looking further ahead, I see myself excel in my career as a cyber security analyst protecting online realms and keeping personal data safe from ever-changing risks. I have come to have this position with a broad set of skills outside of security. As a frontend specialist with years of experience building web applications, I know what makes an application intuitive, user-centric, and how to build robust, scalable apps. This is an ability that enables me to understand how digital systems work and better identify exploits from a development standpoint. It allows me to predict dangers ahead and counter them proactively. I have great enthusiasm to develop it and work as Cyber Security Analyst where i blend web dev skill to protect the Digital world. I’m dedicated to never stopping learning and eager to protect the digital world, one step at a time, making a difference with my career in cybersecurity.</p>
  </main>
</template>

<script setup>
const items = [
  {
    id: 1,
    title: 'Project I: HTML Basics',
    imageUrl: '../src/assets/P1image.png',
    description: 'This project was my initial learning of HTML/CSS, very basic stuff but from this project I was able to get fundamental knowledge for Web Development.'
  },
  {
    id: 2,
    title: 'Project II: Responsive Features',
    imageUrl: '../src/assets/P2image.png',
    description: 'This project was based around Responsive Web Design (RWD), It has features implemneted into the CSS and HTML that allow for the text/image to be resized in response the the users actions.'
  },
  {
    id: 3,
    title: 'Project III: Fitness Tracker',
    imageUrl: '../src/assets/P3image.png',
    description: 'This was by far my biggest project, a Fitness and Health Tracker with lots of functional features, inclduing caluclators, dark mode and more HTML, Vue 3 and CSS concepts.'
  },
];
</script>

<style lang="scss" scoped>
  @import url(../assets/PortfolioView.css);
</style>
