<template>
  <div class="card">
    <div class="card-image">
      <slot name="image"></slot>
    </div>
    <div class="card-header">
      <div class="card-title h5">
        <div name="title"> h</div>
      </div>
      <div class="card-subtitle text-gray">
        <div name="subtitle"></div>
      </div>
    </div>
    <div class="card-body">
      <div name="body"></div>
    </div>
    <div class="card-footer">
      <div name="button"></div>
    </div>
  </div>
</template>
<script>


export default {

}
</script>

