<template>
  <div>
    <div class="mb-2">
     <b-button @click="showMsgBoxOne">{{TextBouton}}</b-button>
    </div>
  </div>
</template>

<script>
  export default {
    name:'ModalBlock',
    props:['TextBouton','ModalContent'],
    data() {
      return {
        boxOne: 'te',
        
      }
    },
    methods: {
      showMsgBoxOne() {
        this.$bvModal.msgBoxOk(this.ModalContent)
          .then(value => {
            this.boxOne = value
          })
          .catch(err => {
            // An error occurred
          })
      },
    }
  }
</script>