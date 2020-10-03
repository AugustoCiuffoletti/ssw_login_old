# A login form with route control

The aim of this exercise is to implement a login form that controls the routing mechanism: only the user that successfully completes the login process has access to the inner pages.

The web service offers two routes:

- the "login" route, that is the landing point of our web service,ù
- the "main" route, that is the protected route, accessible only after a successful login

The operation is based on two components:

- The "login" component, visible when authorization is pending
- The "main" component, visible after successful login

The directory of the login components hosts also:

- an "auth" service implementing an observable
- the "login" guard that implement a blocking "onActivate" method

## Step 0

At this stage, we have simply created a new project using the Angular CLI, by specifying that we want the routing configured in our template project.

You can load to stackblitz this project, and proceed updating it.

## Step 1

Here we create all the features of our project:

  * two components: one for the login form, another for the (empty) main service
  * a guard that will open/close the route to the main component
  * a service that will operate asynchronously user I/O

You can do this using the Stackblitz IDE

### Observe

Browse the new template files

## Step 2

The app-routing.module.ts is populated with suitable routes. The guard is added to the main route.

The html of the root app component contains only a title and the router-outlet.

The guard is always false.

### Observe

Visiting the URL with empty route points to the login page ("login works"), the same with a login route. The URL with the "main" route returns only the title (easy to configure an "Access Denied" component).

##  Step 3

The login form is added with a view and no function.

### Observe

See the form and type login and password, with no effect

