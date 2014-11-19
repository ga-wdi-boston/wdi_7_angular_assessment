wdi_7_angular_assessment
========================

### Question 1

Complete the following code so that the sum of num1 and num2 is displayed

`<p ng-init="numbers = {num1: 5, num2: 10}"> {{numbers.num1 + numbers.num2}}</p>`

### Question 2

What are the four methods of the $http service that we have used?

get
post
put
delete

### Question 3

Create an unordered list out of the users in the following code

`<ul ng-init="users = [{name: 'Dan'}, {name: 'Ella'}]"></ul>`

`<li ng-repeat="user in users">{{user.name}}</li>`

### Question 4

Based on questions #1 and #3, where are numbers and users getting created and stored?

In Angular's current scope

### Question 5

Write the correct version of the code below

`angular.module($scope).controller($http, 'MainCtrl', [])`

`angular.module('MyModule').controller('MainCtrl, function($scope, $http)`

### Question 6

True of False - the following is an example of a filter?

`<ng-view></ng-view>`

False, filters are denoted using a pipe

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
  .otherwise({
    redirectTo: '404.html'
  });
```

### Question 8

Change the following code so that it uses one time binding

`<p>{{ user.first_name }}</p>`

`<p>{{ ::user.first_name }}</p>`

### Question 9

Give two examples of angular directives used for handling events

ng-click
ng-keypress
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
{
  user: {
    first_name: 'Dan',
    last_name: 'Dohnson'
  }
}
```

Depending on the way the strong params on our Rails server are set up. If we are using yesterday's setup the answer is #2.
