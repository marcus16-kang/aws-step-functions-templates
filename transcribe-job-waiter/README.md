# Transcribe Job Waiter

<p align="center"><img src="images/stepfunctions_graph.svg"></p>

## State Execution Input Format

``` json
{
    "jobName": "<JOB NAME>"
}
```

## How to Deploy

``` shell
aws cloudformation create-stack \
    --stack-name transcribe-waiter-state-machine-stack \
    --template-body file://template.yaml \
    --capabilities CAPABILITY_NAMED_IAM
```