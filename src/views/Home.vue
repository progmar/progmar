<template>
  <TheHeader />
  <main class="content">
    <Welcome />
    <Performance />
    <Tech />
    <Team />
    <Contact />
  </main>
  <TheFooter />
</template>

<script>
// @ is an alias to /src
import TheHeader from "@/components/TheHeader";
import Welcome from "@/components/Welcome";
import Performance from "@/components/Performance";
import Tech from "@/components/Tech";
import Team from "@/components/Team";
import Contact from "@/components/Contact";
import TheFooter from "@/components/TheFooter";

export default {
  name: "Home",
  components: {
    TheHeader,
    Welcome,
    Performance,
    Tech,
    Team,
    Contact,
    TheFooter,
  },
};
</script>
