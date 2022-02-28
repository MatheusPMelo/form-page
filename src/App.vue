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
        <Form 
          thanksTextMain="Obrigado!" 
          thanksSubTextMain="Em breve estaremos entrando em contato :)"
        />
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

  body{
    scrollbar-width: thin;          /* "auto" or "thin" */
    scrollbar-color: blue orange;   /* scroll thumb and track */
  }

  body::-webkit-scrollbar {
    width: 12px;               /* width of the entire scrollbar */
  }
  
  body::-webkit-scrollbar-track {
    background: #fff;        /* color of the tracking area */
  }
  
  body::-webkit-scrollbar-thumb {
    background-color: rgb(144, 93, 192);    /* color of the scroll thumb */
    border-radius: 20px;       /* roundness of the scroll thumb */
    border: 3px solid #fff;  /* creates padding around scroll thumb */
  }
</style>
