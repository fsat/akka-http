# options

Matches requests with HTTP method `OPTIONS`.

## Description

This directive filters the incoming request by its HTTP method. Only requests with
method `OPTIONS` are passed on to the inner route. All others are rejected with a
@unidoc[MethodRejection], which is translated into a `405 Method Not Allowed` response
by the default `RejectionHandler`.

## Example

Scala
:  @@snip [MethodDirectivesExamplesSpec.scala]($test$/scala/docs/http/scaladsl/server/directives/MethodDirectivesExamplesSpec.scala) { #options-method }

Java
:  @@snip [MethodDirectivesExamplesTest.java]($test$/java/docs/http/javadsl/server/directives/MethodDirectivesExamplesTest.java) { #options }
