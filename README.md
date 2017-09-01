# angular-link

authentication and authorization in angular--- 
  
1.  https://www.sitepoint.com/implementing-authentication-angular-applications/
2.  https://github.com/alarv/ng-login
3.  http://www.stefanoscerra.it/permission-based-auth-system-in-angularjs/
4. (best)   https://stackoverflow.com/questions/22537311/angular-ui-router-login-authentication
5.  https://medium.com/@him_jar/permission-based-views-in-angularjs-1edfd0fd8288
6.  https://medium.com/opinionated-angularjs/techniques-for-authentication-in-angularjs-applications-7bbf0346acec

pagination
 
1.https://ciphertrick.com/2015/06/01/search-sort-and-pagination-ngrepeat-angularjs/


To check no of watches  in angular

 1. (function () { 
        var root = $(document.getElementsByTagName('body'));
        var watchers = [];

        var f = function (element) {
            if (element.data().hasOwnProperty('$scope')) {
                angular.forEach(element.data().$scope.$$watchers, function (watcher) {
                    watchers.push(watcher);
                });
            }

            angular.forEach(element.children(), function (childElement) {
                f($(childElement));
            });
        };

        f(root);

        console.log(watchers.length);
    })();

Angular best practices( filters with ng-repeat)
  1  https://toddmotto.com/categories/angularjs
  
  
