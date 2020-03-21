<template>
  <q-page padding>
    <div class="column justify-center items-center">
    <q-card class="my-card" @click="alert=true">
      <q-img :src="character.img">
        <div class="absolute-bottom text-center">
            <div class="text-h3">{{ character.name }}</div>
            <div class="text-h5">{{ character.nickname }}</div>
        </div>
      </q-img>
    </q-card>
    </div>
    <q-dialog v-model="alert">
        <q-card>
            <q-card-section>
                <div class="text-center">
                    <div class="text-h6">Info</div>
                    <div>
                        <p>{{character.birthday}}</p>
                        <p>{{character.status}}</p>
                        <p>{{character.occupation}}</p>
                    </div>
                </div>
            </q-card-section>
            <q-card-actions align="right">
                <q-btn flat label="OK" color="primary" v-close-popup></q-btn>
            </q-card-actions>
        </q-card>
    </q-dialog>
  </q-page>
</template>

<script>
export default {
  async created() {
      let url = `https://www.breakingbadapi.com/api/characters/${this.$route.params.id}`;
      if (this.$route.params.id === 'random') {
          url = `https://www.breakingbadapi.com/api/character/${this.$route.params.id}`;
      }
      const character = await this.$axios.get(url);
      console.log(character.data);
      this.character = character.data[0];
  },
  data() {
      return {
          character: '',
          alert: false
      }
  }
}
</script>
<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 400px
</style>