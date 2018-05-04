# Resiliency in Distributed system

[slides](https://slides.com/rajeevbharshetty/resiliency-in-distributed-systems)

[Blog](https://blog.gojekengineering.com/resiliency-in-distributed-systems-efd30f74baf4)


-----
Need proper discipline

Capacity to Recover from difficulties

## Pattern

Heimdall

### 1s Pattern
Timesouts

Stop waiting for an answer

Required at Integration Points

based on SLA

### 2nd Retries

### 3rd Circuit Breakers

Hystrix

### 4th Fallbacks

Fallback from Route Distance to Route Approximation

Fallback to a Different Maps Provider

### 5th Resiliency Testing

