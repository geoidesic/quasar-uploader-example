<template>
  <q-page class="flex flex-center">
    <q-uploader
    ref="uploader"
    :url="url"
    multiple
    auto-expand
    :header="header"
    :additional-fields="additionalFields"
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
  		// url: 'http://localhost:8082/upload'
  		url: 'http://192.168.33.10:8080/api/upload_item_attachment/1',
  		header: {
  			'authorization': 'Bearer 410e18a7-5fd5-480d-9e0f-dba85928a94f'
  		},
  		additionalFields: [
  			{token: '410e18a7-5fd5-480d-9e0f-dba85928a94f'}
  		]
  		// url: 'http://0.0.0.0:8082/upload'
  	}
  }
}
</script>
