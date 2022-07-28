<template>
  <div class="backdrop" @click.self="closeModal" >
      <div class="modal" >
          <slot></slot>
          <div class="neon">
              <slot name="links"></slot>
          </div>
      </div>
  </div>
</template>
<script>
 export default {
     props: ['header'],
     methods:{
         closeModal(){
             this.$emit('close')    

         }
     }
 }

</script>




<style>
.modal{
    width: 400px;
    padding: 20px;
    margin: 100px auto;
    border-radius: 20px;
    background-color: white;
}
.backdrop{

    top: 0;
    position: fixed;
    background-color: rgba(0,0,0,0.5);
    width: 100%;
    height: 600px;
}

</style>