<template>
  <container>
    <row>
      <column class="flex-center">
        <jumbotron class="mt-5">
          <h1 class="pb-2">
            <Fa icon="code" class="grey-text mr-2"/>
            Programmieren
          </h1>
          <hr class="mt-5">
          <h3>Themenübersicht:</h3>
          <polar-chart :data="polarChartData" :options="polarChartOptions" :width="600" :height="300"></polar-chart>
          <hr class="mt-5">
          <list-group>
            <navbar-item class="list-group-item list-group-item-action" router href="/advanced/accordion">
              <h5 class="justify-content-between d-flex align-items-center">
                Accordion
                <fa icon="angle-right"/>
              </h5>
            </navbar-item>
            <navbar-item class="list-group-item list-group-item-action" router href="/advanced/carousel">
              <h5 class="justify-content-between d-flex align-items-center">
                Carousel
                <fa icon="angle-right"/>
              </h5>
            </navbar-item>
            <navbar-item class="list-group-item list-group-item-action" router href="/advanced/chart">
              <h5 class="justify-content-between d-flex align-items-center">
                Charts
                <fa icon="angle-right"/>
              </h5>
            </navbar-item>
            <navbar-item class="list-group-item list-group-item-action" router href="/advanced/collapse">
              <h5 class="justify-content-between d-flex align-items-center">
                Collapse
                <fa icon="angle-right"/>
              </h5>
            </navbar-item>
            <navbar-item class="list-group-item list-group-item-action" router href="/advanced/maps">
              <h5 class="justify-content-between d-flex align-items-center">
                Google Maps
                <fa icon="angle-right"/>
              </h5>
            </navbar-item>
            <navbar-item class="list-group-item list-group-item-action" router href="/advanced/popover">
              <h5 class="justify-content-between d-flex align-items-center">
                Popover
                <fa icon="angle-right"/>
              </h5>
            </navbar-item>
            <navbar-item class="list-group-item list-group-item-action" router href="/advanced/tooltip">
              <h5 class="justify-content-between d-flex align-items-center">
                Tooltip
                <fa icon="angle-right"/>
              </h5>
            </navbar-item>
            <navbar-item class="list-group-item list-group-item-action" router href="/advanced/videocarousel">
              <h5 class="justify-content-between d-flex align-items-center">
                Video Carousel
                <fa icon="angle-right"/>
              </h5>
            </navbar-item>
          </list-group>
        </jumbotron>
      </column>
    </row>
  </container>
</template>

<script>
  import {Container, Row, Column, Fa, Jumbotron, NavbarItem, ListGroup, PolarChart} from 'mdbvue';

  export default {
    name: 'ProgramPage',
    components: {
      Container,
      Row,
      Column,
      Fa,
      Jumbotron,
      NavbarItem,
      ListGroup,
      PolarChart
    },
    data() {
      return {
        polarChartData: {
          labels: ["PHP", "SQL", "C#", "HTML & CSS", "ERM"],
          datasets: [
            {
              data: [40, 85, 50, 95, 30],
              backgroundColor: ["rgba(247, 70, 74, 0.3)", "rgba(70, 191, 189, 0.3)", "rgba(253, 180, 92, 0.3)", "rgba(233, 30, 99, 0.2)", "rgba(77, 83, 96, 0.3)"],
              hoverBackgroundColor: ["rgba(247, 70, 74, 0.4)", "rgba(70, 191, 189, 0.4)", "rgba(253, 180, 92, 0.4)", "rgba(233, 30, 99, 0.3)", "rgba(77, 83, 96, 0.4)"],
            }
          ]
        },
        polarChartOptions: {
          responsive: false,
          maintainAspectRatio: true,
        },
      };
    }
  }
  ;
</script>

<style scoped>
  .example-components-list {
    padding-top: 20px;
  }

  .example-components-list li {
    padding: 10px;
    background-color: white;
    border-bottom: 1px solid #f7f7f7;
    transition: .3s;
  }

  .example-components-list h6 {
    padding: 20px 10px 5px 10px;
    color: grey;
  }

  .example-components-list li:hover {
    background-color: #fafafa;
  }

  .example-components-list i {
    float: right;
    padding-top: 3px;
  }

  .nav-link.navbar-link h5 {
    color: #212529;
  }
</style>
