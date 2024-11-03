<template>
  <div>
    <h1>Resume</h1>

    <div class="paragraph">
      
      <br>
      Hi, I'm <strong>Mark</strong>,I make games!
      I'm currently studying Software and Game Developer in the Netherlands.<br>
      <br>
      After my first internship at Extra Nice as a junior developer and level designer I have started releasing my own games, usually written in C# using Unity.<br>
      <br>
      Together with a friend I'm currently developing a Visual Novel in Python.<br>
      <br>
      I'm also in the process of releasing a sci-fi game on Steam.<br>
      <br>        
      I am also knowledgable in Construct and Gamemaker.<br>
      <br>
      I'm always open to using the right engine for the job!<br>
      <br>
      <router-link to="/contact">contact me</router-link>.

      <div style="margin-top:20px; margin-bottom:20px;">
        <a class="download-link" href="d/resume-en.pdf" target="_blank"><i class="fa fa-download fa-lg fa-fw"></i> Download as PDF 🇬🇧</a>
        <div style="clear:both"></div>
      </div>
    </div>
    <div class="photo">
      <img src="img/resume-photo.png" alt="Photo of Mark" class="center" />
    </div>

    <div style="clear:both"></div>

    <div class="full-content">
      <h2>Work experience</h2>

      <h3>Extra Nice</h3>
      <h4>2020-2021</h4>

      <div>Developer and level designer on Skirmish.</div>

      <div class="tech-stack">Unity & C#. </div>

      <h2>Skills</h2>

      <div class="skill-set">
        <h3>Software</h3>
        <SkillRate name="Unity 2022" :rate="4" />
        <SkillRate name="Visual Studio 2024" :rate="5" />
        <SkillRate name="Construct 2" :rate="4" />
        <SkillRate name="Game Maker" :rate="4" />
        <SkillRate name="Git/Github Desktop" :rate="5" />
        <SkillRate name="Plastic SCM" :rate="5" />
        <SkillRate name="Microsoft 356" :rate="5" />

      </div>

      <div class="skill-set">
        <h3>Languages</h3>
        <SkillRate name="C#" :rate="5" />
        <SkillRate name="html/CSS" :rate="4" />
        <SkillRate name="PHP" :rate="3" />
      </div>
      <div style="clear:both" />

      <h2>Education</h2>

      <h3>Piter Jelles !mpulse</h3>
      <h4>Highschool diploma</h4>
      <div>Certificaat van verworven competenties</div>

      <h2>Languages</h2>

      <h3>English</h3>
      <div>Highly proficient.</div>

      <h3>Dutch</h3>
      <div>My native tongue.</div>

      <h3>Frysian</h3>
      <div>Born and raised.</div>

      <h3>German</h3>
      <div>I have a fair bit German neurons but it takes me a few days immersed in Germany to activate them.</div>

      <h3>Finnish</h3>
      <div>Learning via Duolingo and with friends!</div>


      <h2>Besides...</h2>
      <div>
        <h3>I ❤️ Videogames</h3>
        <div>Fallout New Vegas, Red Dead Redemption 2, GTA 5 and even the eternal Town of Salem.</div>

        <h3>I 🧡 Tabletop Games</h3>
        <div>Nemesis, Eclipse, Warhammer 40K, Bloodbowl, you name it!</div>

        <h3>I 💛 Card games</h3>
        <div>MTG, UNO and classics like Durak & Mao</div>

        <h3>I 💚 Bouldering</h3>
        <div>The only sport that I enjoy as much as gaming.</div>

      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import SkillRate from "@/components/SkillRate.vue";

export default Vue.extend({
  name: "Resume",
  components: {
    SkillRate,
  },
});
</script>

<style scoped>
h2 {
  font-weight: 100;
  font-size: 2em;
  margin: 0px;
  padding: 0px;
  padding-top: 50px;
}
h3 {
  font-weight: 100;
  font-size: 1.6em;
  margin: 0px;
  padding: 0px;
  padding-top: 30px;
}
h4 {
  font-weight: 100;
  font-size: 1.3em;
  margin: 0px;
  padding: 0px;
  padding-top: 15px;
  font-style: italic;
}

.paragraph {
  max-width: 700px;
}

.download-link {
  float:left;
  margin-right: 50px;
}

.full-content div {
  max-width: 800px;
}

.skill-set h3 {
  padding-bottom: 10px;
}

.photo img {
  height: 300px;
  width: 300px;
}

.tech-stack {
  font-style: italic;
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
    padding: 30px;
    padding-left: 80px;
  }

  .skill-set {
    float: left;
    padding-right: 60px; 
  }
}
</style>