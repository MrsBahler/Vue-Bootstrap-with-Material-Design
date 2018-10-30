<template>
  <container class="pt-4">
    <h1 class="pb-2 pt-4 h1-responsive">
      <Fa icon="graduation-cap" class="grey-text mr-2"/>
      Dashboard Lernübersicht
    </h1>
    <hr class="mb-4"/>
    <carousel :interval="8000" full>
      <carousel-item video src="https://mdbootstrap.com/img/video/forest.mp4" alt="Second slide" auto loop>
        <carousel-caption title="Video Teaserimage" text="Second text"></carousel-caption>
      </carousel-item>
    </carousel>
    <hr class="mb-0"/>
    <h3 class="h3 h3-responsive pt-4 pl-5">Fächerübersicht:</h3>
      <jumbotron class="pt-3">
        <list-group>
          <navbar-item class="pb-2 list-group-item list-group-item-action" router href="/learn/program">
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
  </container>
</template>

<script>
  import {
    Container,
    Row,
    Column,
    Fa,
    Jumbotron,
    NavbarItem,
    ListGroup,
    PolarChart,
    Carousel,
    CarouselItem,
    CarouselCaption
  } from 'mdbvue';

  export default {
    name: 'LearnPage',
    components: {
      Container,
      Row,
      Column,
      Fa,
      Jumbotron,
      NavbarItem,
      ListGroup,
      PolarChart,
      Carousel,
      CarouselItem,
      CarouselCaption
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
  .view {
    background: url("https://mdbootstrap.com/img/Photos/Others/img(42).jpg") no-repeat center center;
    background-size: cover;
    height: 100%;
  }

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

