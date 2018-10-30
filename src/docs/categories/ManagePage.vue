<template>
  <container class="pt-4">
    <h1 class="pb-2 pt-4 h1-responsive"><Fa icon="folder-open" class="grey-text mr-2" />File Management</h1>
    <hr class="mb-4" />
    <row>
      <column md="8" class="mx-auto">
        <accordion :panes="panes"/>
      </column>
    </row>
    <hr />
    <div class="mt-5 pt-5 mx-3">
      <h2>Datatable data from API</h2>
      <br />
      <mdb-datatable
          :data="'https://my-json-server.typicode.com/Rotarepmi/exjson/db'"
          striped
          bordered
          materialInputs
      />
    </div>
  </container>
</template>

<script>
  import {Accordion, Container, Row, Column, Fa, Jumbotron, ListGroup, NavbarItem, Btn, mdbDatatable} from 'mdbvue';

  export default {
    name: 'ManagePage',
    components: {
      Container,
      Row,
      Btn,
      Column,
      Accordion,
      Fa,
      Jumbotron,
      ListGroup,
      NavbarItem,
      mdbDatatable
    },
    methods: {
      handlePages (value) {
        this.pages = value;
      },
      handleFields (value) {
        this.fields = value;
      }
    },
    data() {
      return {
        panes: [
          {
            title: 'Collapsible Group Item #1',
            content: "test",
          },
          {
            title: 'Collapsible Group Item #2',
            content: "test",
          },
          {
            title: 'Collapsible Group Item #3',
            content: "test",
          }
        ],
      };
    },
  };

</script>
