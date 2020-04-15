[![Latest Stable Version](https://poser.pugx.org/deadsimple/axioslibrary/version)](https://packagist.org/packages/deadsimple/axioslibrary) [![Total Downloads](https://poser.pugx.org/deadsimple/axioslibrary/downloads)](https://packagist.org/packages/deadsimple/axioslibrary) [![License](https://poser.pugx.org/deadsimple/axioslibrary/license)](https://packagist.org/packages/deadsimple/axioslibrary)

# Deadsimple Axios Magento2 Composer Library

This package allows you to include the latest version of axios and use on a global level together with requirejs in your Magento2 setup straight out of the box

## Installation

Use composer to install the module: `composer require deadsimple/axioslibrary

## Usage
Create a main js file to load through requirejs in this main.js file define `Vue` (with a capital V) and use `vue` (see the non capital v) to load your created vue components in this example `Searchinput.vue`. From this point on you can initialize vue the way your used to with the `new Vue()` initializer, please make sure you have a container available to run your VueJS code in `#essearch` in this example;


```
define([
  'Axios'
], function (axios) {
  'use strict';
  
  // Make a request for a user with a given ID
  axios.get('/user?ID=12345')
    .then(function (response) {
      // handle success
      console.log(response);
    })
    .catch(function (error) {
      // handle error
      console.log(error);
    })
    .then(function () {
      // always executed
    });
})
``` 

### Version

This library loads: `Axios v0.19.2
