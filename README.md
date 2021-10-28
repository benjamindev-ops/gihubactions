# gihubactions


1.- To start working with the github actions create a repository and include a directory called 

``` bash

.github/workflows

```
2.- Include the folowwind code on a file called cicd.yml 

``` bash
name: A workflow for my Hello World file
on: push
jobs:
  build:
    name: Hello world action
    runs-on: ubuntu-latest
    steps:
      - run: echo "Hi from the pipeline"
 
 ```
 3.- Summit the commit

 Later on te menu of actions we will se our pipeline in deplaoy and the message "Hi from the pipeline"
__________________________________________________

# important considerations 

1 .- there is a limit of the deployments when we are usign github actions it is important to consierar include some runners for the deployments
2.- For the yml code is imporant to inlcude always 
on - there is the instruction of when the pipeline will be executed
jobs - ther is the stage where the pipeline will be declared
build - englobes all the instrucctions and definitions of our deploy 
steps - include the phases 
run - that is the instruction of what the code will do

