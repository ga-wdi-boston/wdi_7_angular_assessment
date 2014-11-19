wdi_7_angular_assessment
========================

### Question 1

Complete the following code so that the sum of num1 and num2 is displayed

`<p ng-init="numbers = {num1: 5, num2: 10}">{{numbers.num1 + numbers.num2}}</p>`


### Question 2

What are the four methods of the $http service that we have used?
Get, Post, Delete, Put(update)

### Question 3

Create an unordered list out of the users in the following code

<ul ng-init="users = [{name: 'Dan'}, {name: 'Ella'}]">
  <li ng-repeat="user in users">{{user.name}}</li>
</ul>`

### Question 4

Based on questions #1 and #3, where are numbers and users getting created and stored?
####################### got this one wrong ################################
on the $scope

### Question 5

Write the correct version of the code below

`angular.module($scope).controller($http, 'MainCtrl', [])`


  ############# The right answer is : ###############################
angular.module('Demo').controller('MainCtrl', function($scope, $http){

  });

### Question 6

True of False - the following is an example of a filter?
False
`<ng-view></ng-view>`

### Question 7

Modify the following code so that if the route is not /home or /about, it will load a 404.html template

```
$routeProvider
  .when('/home', {
    templateUrl: 'templates/home.html'
  })
  .when('/about', {
    templateUrl: 'templates/about.html'
  })
  .otherwise('/404.html',{
    templateUrl: 'templates/404.html'
  });
```

### Question 8

Change the following code so that it uses one time binding

`<p>{{ ::user.first_name }}</p>`

### Question 9

Give two examples of angular directives used for handling events
ng-repeat
ng-click
ng-submit

### Question 10

Which of the following is the correct way to send data to Rails to update a user model?

```
{
  first_name: 'Dan',
  last_name: 'Dohnson'
}
```

```

#this is the correct way
{
  user: {
    first_name: 'Dan',
    last_name: 'Dohnson'
  }
}
```
