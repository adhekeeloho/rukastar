<template>
  <div class="overflow-hidden">
    <section>
      <Intro />
    </section>

    <section class="mt-5">
      <Services />
    </section>

    <section class="mt-5">
      <Body />
    </section>

        <section class="mt-5" >
        <CardBody/>
      </section>

    <section class="mt-10">
      <Footer/>
    </section>
  </div>
</template>

<script>
import Intro from "@/components/Intro.vue";
import Services from "@/components/Services.vue";
import Body from "@/components/Body.vue";
import CardBody from "@/components/CardBody.vue";
import Footer from "@/components/Footer.vue";


export default {
  name: "Home",
  components: {
    Intro,
    Services,
    Body,
    CardBody,
    Footer
  },
  data() {
    return {};
  },
};
</script>

<style scoped></style>
