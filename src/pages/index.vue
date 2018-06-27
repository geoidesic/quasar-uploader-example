<template>
  <q-page class="flex flex-center">
    <q-uploader
    ref="uploader"
    :url="url"
    multiple
    auto-expand
    >
	</q-uploader>
  </q-page>
</template>

<style>
</style>

<script>
export default {
  name: 'PageIndex',
  data() {
  	return {
  		url: 'http://localhost:8082/upload'
  	}
  }
}
</script>
