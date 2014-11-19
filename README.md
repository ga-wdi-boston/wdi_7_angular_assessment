wdi_7_angular_assessment
========================

### Question 1

Complete the following code so that the sum of num1 and num2 is displayed

`<p ng-init="numbers = {num1: 5, num2: 10}">The sum goes here</p>`

`<p ng-init="numbers = {num1: 5, num2: 10}">{{num1 + num2}}</p>`

### Question 2

What are the four methods of the $http service that we have used?

POST GET DELETE PUT

### Question 3

Create an unordered list out of the users in the following code

`<ul ng-init="users = [{name: 'Dan'}, {name: 'Ella'}]"></ul>`

<ul ng-init="users = [{name: 'Dan'}, {name: 'Ella'}]" ng-repeat="user in users">
  <li>{{user}}</li>
</ul>

### Question 4

Based on questions #1 and #3, where are numbers and users getting created and stored?

I do not know for sure, but they are stored "behind the scene" when line 8 and 22 get executed.

### Question 5

Write the correct version of the code below

`angular.module($scope).controller($http, 'MainCtrl', [])`

`angular.module('whatever is in <body ng-app="xxxx">').controller('MainCtrl', function($scope, $http))`

### Question 6

True of False - the following is an example of a filter?

`<ng-view></ng-view>`
false, i think it is a template

### Question 7

Modify the following code so that if the route is not /home or /about, it will load a 404.html template

```
$routeProvider
  .when('/home', {
    templateUrl: 'templates/home.html'
  })
  .when('/about', {
    templateUrl: 'templates/about.html'
  });
```

$routeProvider
  .when('/home', {
    templateUrl: 'templates/home.html'
  })
  .when('/about', {
    templateUrl: 'templates/about.html'
  });
  .otherwise({
    templateUrl: 'templates/404.html'
  });
### Question 8

Change the following code so that it uses one time binding

`<p>{{ user.first_name }}</p>`

`<p>{{ ::user.first_name }}</p>`

### Question 9

Give two examples of angular directives used for handling events

$scope.$watch('favColor', function(newValue, oldValue) {});
$scope.$watchgroup(['favColor' 'favNumber], function(newValue, oldValue, scope) {});

### Question 10

Which of the following is the correct way to send data to Rails to update a user model?

```
{
  first_name: 'Dan',
  last_name: 'Dohnson'
}
```

```
{
  user: {
    first_name: 'Dan',
    last_name: 'Dohnson'
  }
}
```

second method is correct, rails expect a property of the model, in this case property "user:"
