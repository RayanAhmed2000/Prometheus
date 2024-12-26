# Understanding Queries 
- Metrics eg http_requests_total
- Labels eg method="GET", status="200"
- Sample Query
```
http_requests_total{method="GET", status="200"}
```
- Apply range (send metrics over 5 minutes)
```
http_requests[5m]
```
- Mathematical Functions (min/max/count/average/sum/rate)
```
rate(sum(http_requests_total{method="GET", status="200"}))
```
- Group by Labels
```

```
