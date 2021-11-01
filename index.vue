<template>
  <div class="modal">

  </div>
</template>
<script>
export default {

}
</script>
<script src="https://unpkg.com/vue"></script>
<link rel="stylesheet" type="text/css" href="/style.css" />
<!-- template for the modal component -->
<script type="text/x-template" id="modal-template">
<transition name="modal">
<div class="modal-mask">
  <div class="modal-wrapper">
    <div class="modal-container">

      <div class="modal-header">
        <slot name="header">
          default header
        </slot>
      </div>

      <div class="modal-body">
        <slot name="body">
          1900200115金宇峰
        </slot>
      </div>

      <div class="modal-footer">
        <slot name="footer">
          折叠
          <button class="modal-default-button" @click="$emit('close')">
            OK
          </button>
        </slot>
      </div>
    </div>
  </div>
</div>
</transition>
</script>
<style type="css" scoped>
.firstdemo{
  width: 100px;
  height: 100px;
  background: #2c3e50;
}
.firstdemo a{
  color: aliceblue;
  text-decoration: none;
}
</style>
<style scoped>

</style>
