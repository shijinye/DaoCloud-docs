# Rancher cluster compatibility test

✅: Test passed; ❌: Test failed.

!!!note

     The test functions in the table are not comprehensive.

| case | | Test method | Rancher rke2c1(k8s 1.24.11) | Remarks |
| ------------ | ------------------------ | ----------- ----- |--------- |--------- |
| Collect and query web application metrics | | Manually | ✅| |
| Add custom metric collection | | Manual | ✅| |
| Query real-time metrics | | Manual | ✅| |
| Instantaneous index query | | Manual | ✅| |
| Instantaneous metric api field function verification | | Manual | ✅| |
| Query metrics over a period of time | | Manually | ✅| |
| Query api field function verification of metrics within a period of time | | Manual | ✅| |
| Batch query cluster CPU, memory usage, total cluster CPU, cluster memory usage, total number of cluster nodes | | Manual | ✅| |
| Batch query node CPU, memory usage, total node CPU, node memory usage | | Manual | ✅| |
| Batch query cluster CPU, memory usage, total cluster CPU, cluster memory usage, and total number of cluster nodes within a period of time | | Manual | ✅| |
| Batch query to query the function verification of the index api field within a period of time | | Manual | ✅ ||
| Query POD log | | Manual | ✅| |
| Query SVC Logs | | Manual | ✅| |
| Query statefulset logs | | Manually | ✅| |
| Query Deployment Logs | | Manual | ✅| |
| Query NPD log | | Manual | ✅| |
| Log Filtering | | Manual | ✅| |
| Log fuzzy query-workloadSearch | | Manual | ✅| |
| Log fuzzy query-podSearch | | Manual | ✅| |
| Log Fuzzy Query-containerSearch | | Manual | ✅| |
| Log precise query-cluster | | Manual | ✅| |
| Log precise query-namespace | | Manual | ✅| |
| Log query api field function verification | | Manual | ✅| |
| alert rules - addition, deletion, modification and query | | Manual | ✅ ||
| alert template - addition, deletion, modification and query | | Manual | ✅ ||
| Notification method - addition, deletion, modification and query | | Manual | ✅ ||
| trace query | | Manual | ✅ ||
| Topology query | | Manual | ✅ ||