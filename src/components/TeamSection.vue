<template>
  <v-container fluid id="team">
    <v-container grid-list-md class="my-14">
      <h1 class="title-h1 text-center mb-5">Our Team</h1>
      <v-row justify="center" align="center" class="mt-16">
        <TeamCard
          v-for="(member, index) in members"
          :key="index"
          :member="member"
        />
      </v-row>
    </v-container>
  </v-container>
</template>
<script>
import TeamCard from "./ui/TeamCard.vue";

export default {
  components: {
    TeamCard,
  },
  data: () => ({
    members: [
      {
        id: 0,
        photo: "team1.jpg",
        name: "Constantin Cearanovski",
        role: "Board member – NGO Positive Initiative",
      },
      {
        id: 1,
        photo: "team2.jpg",
        name: "Ruslan Poverga",
        role: "Co-Founder and CEO – NGO Positive Initiative",
      },
      {
        id: 2,
        photo: "team3.png",
        name: "Andrei Tintari",
        role: "Web3 Moldova Community Founder, CTO",
      },
    ],
  }),
};
</script>
<style lang=""></style>
