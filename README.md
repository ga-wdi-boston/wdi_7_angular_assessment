wdi_7_angular_assessment
========================

### Question 1

Complete the following code so that the sum of num1 and num2 is displayed

> `<p ng-init="numbers = {num1: 5, num2: 10}">{{ numbers.num1 + numbers.num2 }}</p>`

### Question 2

What are the four methods of the $http service that we have used?

> `$http.get();`,
> `$http.post();`,
> `$http.put();`,
> `$http.delete();`.

### Question 3

Create an unordered list out of the users in the following code

    <ul ng-init="users = [{name: 'Dan'}, {name: 'Ella'}]">

      <li ng-repeat="user in users">{{ user.name }}</li>

    </ul>

### Question 4

Based on questions #1 and #3, where are numbers and users getting created and stored?

> `numbers` and `users` are being stored in the controller $scope.

### Question 5

Write the correct version of the code below

> `angular.module('ModuleName').controller('ControllerName', function ($http, $scope) { ... });`

### Question 6

True of False - the following is an example of a filter?

`<ng-view></ng-view>`

> No, a filter is more like this:
> `<ng-repeat="item in items | filter:searchFilter">`
> where there is usually an input that allows you to
> set the filter for the items:
> `<input ng-model="searchFilter">`

### Question 7

Modify the following code so that if the route is not /home or /about, it will load a 404.html template

    $routeProvider
      .when('/home', {
        templateUrl: 'templates/home.html'
      })
      .when('/about', {
        templateUrl: 'templates/about.html'
      })
      .otherwise({
        templateUrl: 'templates/404.html'
      });

### Question 8

Change the following code so that it uses one time binding

> `<p>{{ ::user.first_name }}</p>`

> Meaning, it will render the value of `user.first_name`
> rather than the `user.first_name` object itself.

### Question 9

Give two examples of angular directives used for handling events

> `ng-click` handles what happens when an element is clicked, and
> `ng-submit` handles what happens when a form is submitted.

### Question 10

Which of the following is the correct way to send data to Rails to update a user model?


    {
      first_name: 'Dan',
      last_name: 'Dohnson'
    }


    {
      user: {
        first_name: 'Dan',
        last_name: 'Dohnson'
      }
    }


> The second one is correct. A Rails API
> usually expects a singular named parameter
> for a RESTful POST action.
> For example, a UsersController
> would expect a `user` parameter,
> so only the second example would be valid.

### Final Score
> 10/10