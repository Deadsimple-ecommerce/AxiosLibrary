[![Latest Stable Version](https://poser.pugx.org/deadsimple/axioslibrary/version)](https://packagist.org/packages/deadsimple/axioslibrary) [![Total Downloads](https://poser.pugx.org/deadsimple/axioslibrary/downloads)](https://packagist.org/packages/deadsimple/axioslibrary) [![License](https://poser.pugx.org/deadsimple/axioslibrary/license)](https://packagist.org/packages/deadsimple/axioslibrary)

# Deadsimple Axios Magento2 Composer Library

This package allows you to include the latest version of axios and use on a global level together with requirejs in your Magento2 setup straight out of the box

## Installation

Use composer to install the module: `composer require deadsimple/axioslibrary`

## Usage
Using this library is easy peasy, just include the axios script through requirejs, define Axios and use it wherever you like.


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

This library loads: `Axios v0.19.2`
