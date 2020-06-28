# Fproxy-Internal-Load-Balancer
This is forward proxy with internal load balancer.It is working on Layer 7(for now) and it is balancing load between internal network interface and every request made on another network card on host.<br><br>
<br>&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;->interface1------>x.com
<br>&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;->interface2------>y.com
<br>Request---->PROXY->interface3------>z.com  
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;->interface4------>x.com
<br>&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;->interface5------>y.com
# TODOs
- Https support
- Healthcheck(network card based and addres based)
- Failover(If cannot reach from an interface than try another one)
- Load Balancing Algorithms
- Enabling Reverse Proxy on demand(on another port)
- Add Layer 3 support
- Dashboard(Monitoring Requests)
- Auth(From headers)
- More Header options from args
- Tls Termination
