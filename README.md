wdi_7_angular_assessment
========================

### Question 1

Complete the following code so that the sum of num1 and num2 is displayed

`<p ng-init="numbers = {num1: 5, num2: 10}">{{ numbers.num1 + numbers.num2 }}</p>`

CORRECT

### Question 2

What are the four methods of the $http service that we have used?

get, post, put, delete

CORRECT

### Question 3

Create an unordered list out of the users in the following code

`<ul ng-init="users = [{name: 'Dan'}, {name: 'Ella'}]">`
`<li ng-repeat="user in users"> {{ user.name }}</li> `
`</ul>`

CORRECT

### Question 4

Based on questions #1 and #3, where are numbers and users getting created and stored?

in the browser (they are not being stored in the server)

TECHNICALLY CORRECT - but answer he's looking for is that they are being stored in $scope

### Question 5

Write the correct version of the code below

`angular.module($scope).controller($http, 'MainCtrl', [])`

corrected version:
//initialize:
`angular.module('App', []);`

//create controller:
`angular.module('App').controller('MainCtrl', function($scope, $http));`

[referred to notes for syntax]

CORRECT

### Question 6

True of False - the following is an example of a filter?

`<ng-view></ng-view>`

False

CORRECT, it is an element directive

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
    redirectTo: 'templates/404.html'
  });
```
[referred to notes for syntax]

CORRECT

### Question 8

Change the following code so that it uses one time binding

`<p ng-init="user = {first_name: 'Dan'}">{{ user.first_name }}</p>`

INCORRECT: one-time binding is for when you just want to display the static value; it would be:

{{ ::user.first_name }}


### Question 9

Give two examples of angular directives used for handling events

ng-click
ng-repeat

CORRECT

### Question 10

Which of the following is the correct way to send data to Rails to update a user model?

the first one:

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

INCORRECT; but this answer actually depends on how the API is structured
