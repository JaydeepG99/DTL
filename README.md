# DTL

Makes a local server.
Connect by using http://localhost:8080/ on your system.

Server is tested using -  ab -n 10000 -c 16 http://localhost:8080/  on terminal giving following results:

This is ApacheBench, Version 2.3 <$Revision: 1807734 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking localhost (be patient)
Completed 1000 requests
Completed 2000 requests
Completed 3000 requests
Completed 4000 requests
Completed 5000 requests
Completed 6000 requests
Completed 7000 requests
Completed 8000 requests
Completed 9000 requests
Completed 10000 requests
Finished 10000 requests


Server Software:        
Server Hostname:        localhost
Server Port:            8080

Document Path:          /
Document Length:        12 bytes

Concurrency Level:      16
Time taken for tests:   0.470 seconds
Complete requests:      10000
Failed requests:        0
Total transferred:      730000 bytes
HTML transferred:       120000 bytes
Requests per second:    21261.67 [#/sec] (mean)
Time per request:       0.753 [ms] (mean)
Time per request:       0.047 [ms] (mean, across all concurrent requests)
Transfer rate:          1515.72 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        0    0   0.1      0       0
Processing:     0    0   1.2      0      13
Waiting:        0    0   1.2      0      13
Total:          0    1   1.2      0      13

Percentage of the requests served within a certain time (ms)
  50%      0
  66%      0
  75%      0
  80%      0
  90%      0
  95%      1
  98%      1
  99%      9
 100%     13 (longest request)
 
 Hence it can handle 10000 concurrent requests easily.
