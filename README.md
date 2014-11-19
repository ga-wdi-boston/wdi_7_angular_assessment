wdi_7_angular_assessment
========================

### Question 1

Complete the following code so that the sum of num1 and num2 is displayed.

`<p ng-init="numbers = {num1: 5, num2: 10}">The sum goes here</p>`

### Question 2

What are the four methods of the $http service that we have used?

### Question 3

Create an unordered list out of the users in the following code

`<ul ng-init="users = [{name: 'Dan'}, {name: 'Ella'}]"></ul>`

### Question 4

Based on questions #1 and #3, where are numbers and users getting created and stored?

### Question 5

Write the correct version of the code below

`angular.module($scope).controller($http, 'MainCtrl', [])`

### Question 6

True of False - the following is an example of a filter

`<ng-view></ng-view>`

### Question 7

Add a route that will catch any routes not matched in the following code

```
$routeProvider
  .when('/', {
    templateUrl: 'templates/home.html'
  })
  .when('/about', {
    templateUrl: 'templates/about.html'
  });
```
