<template>
  <div style="margin-bottom: 80px;">
    <h1>Hello!</h1>

    <div class="paragraph">
      <div>
        <br>
        I'm <strong>Mark Hoitsma</strong>, a passionate Game Developer with 6 years of experience.<br>
        <br>
        I am proficient in Unity and C#, level and gameplay design.<br>
        <br>
        Since I'm from a musician's family I am also passionate about music and sound design in my games.<br>
        <br>
        I've studied in the Netherlands, worked for an indie studio and worked on personal projects.<br>
        <br>
      </div>

      <div style="margin-top: 20px;">I've worked on  <router-link to="/game-projects">stuff</router-link> and took part in <router-link to="/resume">a few things</router-link> as well.</div>

      <div style="margin-top: 40px;">I'm <strong>currently looking for a place to do my final project.</strong> You can reach me at <a href="mailto:markhoitsma@gmail.com">markhoitsma@gmail.com</a> or <router-link to="/contact">through here</router-link>.</div>
    </div>



    <div class="photo">
  <img src="img/avatar.png" alt="Picture of Mark"/>

  <style> 
    div 
    {
      position:relative;
      height: 500px;
    }
    img
    {
      position: absolute;
      top: 50%;
      transform:
      translateY(-50%);
      width: 25;
    }
    </style>
</div>

    <div style="clear:both"></div>

  </div>
</template>

<style scoped>
.paragraph {
  max-width: 700px;
  margin-bottom: 20px;
}

.photo {
  margin-top: 50px;
  text-align: center;
}

@media only screen and (min-width: 620px){
  .paragraph {
    float: left;
  }

  .photo {
    float: left;
    padding: 10px;
    padding-left: 80px;
  }
}

</style>