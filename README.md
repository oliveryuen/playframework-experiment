# playframework-experiment
Experimenting with Play Framework

## Notes
- ```conf/routes``` file defines a route that tells Play to invoke which controller on which route
- template is defined in ```app/views/index.scala.html``` file and compiled as a standard Java class

### Async Controller
- rather than returning ```Result```, the action returns ```CompletionStage<Result>```. When execution completes, Play can use a thread to render the result without blocking the thread in the mean time.
