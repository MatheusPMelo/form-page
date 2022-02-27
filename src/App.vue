<template>
  <main class="bg">
    <header>
      <TopPage btn="Login" />
    </header>
    <section>
      <div class="titleContent">
        <Title 
          mainTitle="Lorem ipsum dolor sit amet, consectetur adipiscing elit" 
          subTitle="Lorem ipsum dolor sit amet, consectetur"
        />
      </div>
      <div class="formContent">
        <Form />
      </div>
    </section>
  </main>
    <section>
      <div class="contentText">
        <ContentText />
      </div>
      <div class="carroussel">
        <Carroussel />
      </div>
    </section>
    <footer>
      <div class="contentFooter">
        <Footer />
      </div>
    </footer>
</template>

<script>
import TopPage from './components/TopPage.vue'
import Title from './components/Title.vue'
import Form from './components/Form.vue'
import ContentText from './components/ContentText.vue'
import Carroussel from './components/Carroussel.vue'
import Footer from './components/Footer.vue'


export default {
  name: "App",
  components: {
    TopPage,
    Title,
    Form,
    ContentText,
    Carroussel,
    Footer
  }
}
</script>

<style scoped>
  .bg{
    background-image: url(./assets/bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    padding-bottom: 4rem;
    box-shadow: 0 0 10px grey;
  }
</style>
