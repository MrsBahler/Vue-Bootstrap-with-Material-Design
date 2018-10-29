<template>
    <div>
      <container fluid>
        <div>
          <div class="card card-image" style="background-image: url(https://images.unsplash.com/photo-1518081461904-9d8f136351c2?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=8a815e999d0f593c8c8bbcb6473b0d39&auto=format&fit=crop&w=1977&q=80);">
            <md-mask overlay="black-strong" flexCenter></md-mask>
            <div class="text-white text-center py-5 px-4 my-5">
              <div>
                <h2 class="card-title h1-responsive pt-3 mb-5 font-bold"><strong>SAE - Project Action Homepage</strong></h2>
                <p class="mx-5 mb-5">Vue Bootstrap with Material Design</p>
                <p class="pb-4">This application shows the actual use of MDB Vue components in the application.</p>
                <a class="btn btn-outline-white btn-md"><i class="fa fa-clone left"></i> View project</a>
              </div>
            </div>
          </div>
        </div>
        <hr class="my-5">
        <row>
          <column md="4" class="mb-5">
            <card>
              <view-wrapper zoom hover src="https://mdbootstrap.com/img/Mockups/Lightbox/Thumbnail/img%20(67).jpg" alt="Card image cap" waves>
                <md-mask overlay="blue-slight" flexCenter text="Upload Files">
                </md-mask>
              </view-wrapper>
              <card-body>
                <card-title>Card with waves effect</card-title>
                <card-text>Some quick example text to build on the card title and make up the bulk of the card's content.</card-text>
                <navbar-item router href="/components" waves-fixed><btn color="info">Learn more</btn></navbar-item>
              </card-body>
            </card>
          </column>
          <column md="4" class="mb-5">
            <card>
              <view-wrapper zoom hover src="https://mdbootstrap.com/img/Photos/Others/laptop-sm.jpg" alt="Card image cap" waves>
                <md-mask overlay="blue-slight" flexCenter text="Upload Files">
                </md-mask>
              </view-wrapper>
              <card-body>
                <card-title>Card with waves effect</card-title>
                <card-text>Some quick example text to build on the card title and make up the bulk of the card's content.</card-text>
                <navbar-item router href="/components" waves-fixed><btn color="info">Learn more</btn></navbar-item>
              </card-body>
            </card>
          </column>
          <column md="4" class="mb-5">
            <card>
              <view-wrapper zoom hover src="https://mdbootstrap.com/img/Mockups/Lightbox/Thumbnail/img%20(67).jpg" alt="Card image cap" waves>
                <md-mask overlay="blue-slight" flexCenter text="Upload Files">
                </md-mask>
              </view-wrapper>
              <card-body>
                <card-title>Card with waves effect</card-title>
                <card-text>Some quick example text to build on the card title and make up the bulk of the card's content.</card-text>
                <navbar-item router href="/components" waves-fixed><btn color="info">Learn more</btn></navbar-item>
              </card-body>
            </card>
          </column>
        </row>
        <hr class="my-5">
        <row>
          <column md="4" class="mb-5">
            <column col="2" md="2" class="float-left">
              <fa icon="bars" size="2x" class="pink-text" />
            </column>
            <column col="10" md="8" lg="10" class="float-right">
              <h4 class="font-weight-bold">NAVIGATION</h4>
              <p class="grey-text">Ready-to-use navigation layouts, navbars, breadcrumbs and much more! Learn more about our navigation components.</p>
              <navbar-item router href="/navigation" waves-fixed><btn size="sm" color="teal darken-1">Learn more</btn></navbar-item>
            </column>
          </column>
          <column md="4" class="mb-5">
            <column col="2" md="2" class="float-left">
              <fa icon="edit" size="2x" class="blue-text" />
            </column>
            <column col="10" md="8" lg="10" class="float-right">
              <h4 class="font-weight-bold">FORMS</h4>
              <p class="grey-text">Inputs, autocomplete, selecst, date and time pickers. Everything in one place is ready to use!</p>
              <navbar-item router href="/forms" waves-fixed><btn size="sm" color="default">Learn more</btn></navbar-item>
            </column>
          </column>
          <column md="4" class="mb-5">
            <column col="2" md="2" class="float-left">
              <fa icon="table" size="2x" class="green-text" />
            </column>
            <column col="10" md="8" lg="10" class="float-right">
              <h4 class="font-weight-bold">TABLES</h4>
              <p class="grey-text">Basic and advanced tables. Responsive, datatables, with sorting, searching and export to csv.</p>
              <navbar-item router href="/tables" waves-fixed><btn size="sm" color="teal darken-1">Learn more</btn></navbar-item>
            </column>
          </column>
        </row>
        <hr class="my-5">
        <row class="mb-4">
          <column md="4" class="mb-5">
            <column col="2" md="2" class="float-left">
              <fa icon="window-restore" size="2x" class="pink-text" />
            </column>
            <column col="10" md="8" lg="10" class="float-right">
              <h4 class="font-weight-bold">MODALS</h4>
              <p class="grey-text">Models used to display advanced messages to the user. Cookies, logging in, registration and much more.</p>
              <navbar-item router href="/modals" waves-fixed><btn size="sm" color="teal darken-1">Learn more</btn></navbar-item>
            </column>
          </column>
          <column md="4" class="mb-5">
            <column col="2" md="2" class="float-left">
              <fa icon="arrows" size="2x" class="blue-text" />
            </column>
            <column col="10" md="8" lg="10" class="float-right">
              <h4 class="font-weight-bold">ADDONS</h4>
              <p class="grey-text">Google Maps, Social Buttons, Pre-built Contact Forms and Steppers. Find out more about our extended components.</p>
              <navbar-item router href="/addons" waves-fixed><btn size="sm" color="default">Learn more</btn></navbar-item>
            </column>
          </column>
          <column md="4" class="mb-5">
            <column col="2" md="2" class="float-left">
              <fa icon="th" size="2x" class="green-text" />
            </column>
            <column col="10" md="8" lg="10" class="float-right">
              <h4 class="font-weight-bold">SECTIONS</h4>
              <p class="grey-text">E-commerce, contact, blog and much more sections. All ready to use in seconds.</p>
              <navbar-item router href="/sections" waves-fixed><btn size="sm" color="teal darken-1">Learn more</btn></navbar-item>
            </column>
          </column>
        </row>
      </container>
    </div>
</template>

<script>
import { Container, Column, Row, Fa, MdMask, ViewWrapper, Navbar, NavbarItem, NavbarNav,
  NavbarCollapse, Btn, EdgeHeader, CardBody, Card, CardImg, CardTitle, CardText } from 'mdbvue';

export default {
  name: 'HomePage',
  components: {
    Container,
    Column,
    Row,
    Fa,
    MdMask,
    ViewWrapper,
    Navbar,
    NavbarItem,
    NavbarNav,
    NavbarCollapse,
    Btn,
    EdgeHeader,
    CardBody,
    Card,
    CardImg,
    CardTitle,
    CardText
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

.home-feature-box {
  padding: 40px 0;
}

.home-feature-box i {
  font-size: 6rem;
}

.home-feature-box span {
  display: block;
  color: black;
  font-size: 20px;
  font-weight: bold;
  padding-top: 20px;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
}

a {
  color: #42b983;
}

</style>
