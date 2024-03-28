<template>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </div>
  <router-view/>
</template>

<script>
import Papa from 'papaparse';
import { extensionsMixin } from '../js/extensionsMixin.js'
import { resourcesMixin } from '../js/resourcesMixin.js'
import CountriesCodes from "./components/CountriesCodes";
import CountriesTextBox from "./components/CountriesTextBox";
import ForecastTypeTabs from "./components/ForecastTypeTabs";


import View from 'ol/View'
import Map from 'ol/Map'
import TileLayer from 'ol/layer/Tile'
import Feature from 'ol/Feature'
import OSM from 'ol/source/OSM'

import VectorSource from "ol/source/Vector";
import Point from "ol/geom/Point";
import VectorLayer from "ol/layer/Vector";

import { fromLonLat } from 'ol/proj'
// importing the OpenLayers stylesheet is required for having
// good looking buttons!
import 'ol/ol.css'



export default {

}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
