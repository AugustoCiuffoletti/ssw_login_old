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

