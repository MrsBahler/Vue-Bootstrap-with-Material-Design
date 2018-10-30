<template>
  <container class="pt-4">
    <h1 class="pb-2 pt-4 h1-responsive">
      <Fa icon="cloud-upload" class="grey-text mr-2"/>
      File Upload
    </h1>
    <hr class="mb-4"/>
    <vue-clip :options="options">
      <template slot="clip-uploader-action" scope="params">
        <div v-bind:class="{'is-dragging': params.dragging}" class="upload-action p-5 border border-blue--light">
          <row>
            <column md="4"></column>
            <column md="4" class="mx-auto" className="align-items-start" align="center">
              <a class="dz-message">
                <Fa icon="cloud-upload" class="grey-text mr-2"/>
                Click <u>here</u> to upload</a>
              <p class="dz-message">...or Drag and Drop files here to upload</p>
            </column>
            <column md="4"></column>
          </row>
        </div>
      </template>

      <template slot="clip-uploader-body" scope="props">
        <div v-for="file in props.files" class="pt-4">
          <img v-bind:src="file.dataUrl"/>
          {{ file.name }} {{ file.status }}
        </div>
      </template>
    </vue-clip>
  </container>
</template>
<style scoped>
  .upload-action.is-dragging {
    background: rgba(173, 216, 230, 0.31);
  }

  .border-blue--light {
    border-color: rgba(44, 143, 184, 0.4) !important;
  }
</style>
<script>
  import {Btn, Container, Row, Column, Fa} from 'mdbvue';

  export default {
    name: 'ComponentsPage',
    components: {
      Btn,
      Container,
      Row,
      Column,
      Fa
    },
    data() {
      return {
        options: {
          url: '/upload',
          paramName: 'file',
          acceptedFiles: ['image/*', 'application/pdf'],
          message: 'You are uploading an invalid file',
          maxFiles: {
            limit: 5,
            message: 'You can only upload a max of 5 files'
          }
        }
      };
    },

  };
</script>