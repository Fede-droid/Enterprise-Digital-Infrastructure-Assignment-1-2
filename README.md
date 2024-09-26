# Enterprise-Digital-Infrastructure-Assignment-1-2
Publication of my personal assignments 1-2

# Performance Benchmarking and DNS Analysis Projects

## Author:
- Federico Cignoli

## Date:
- July 9, 2024

## Abstract
This report covers two key projects:
1. **Performance Benchmarking**: Utilizing the SPECviewperf tool and Windows Performance Monitor to assess GPU performance across three different systems.
2. **DNS Analysis**: Investigating DNS performance, including active queries and performance testing, using various tools and techniques.

## Project 1: Performance Benchmarking with SPECviewperf and Windows Performance Monitor

### Tools Used:
- **SPECviewperf**: A benchmarking tool to assess the performance of GPUs by simulating various professional workloads (viewsets).
- **Windows Performance Monitor**: Used to monitor CPU, memory, and GPU utilization during benchmarking.

### Methodology:
The benchmarking process was conducted on three computers:
1. **PC1 (Workstation)**: No dedicated GPU, integrated graphics only.
2. **PC2 (Personal Laptop)**: Equipped with a dedicated GPU.
3. **PC3 (Older Laptop)**: A combination of integrated and dedicated GPUs.

### Key Findings:
- **PC1**: Poor performance due to lack of a dedicated GPU. Frequent freezes and low frame rates during rendering tasks.
- **PC2**: Significantly better performance with minimal lag. The dedicated GPU handled 3D rendering efficiently.
- **PC3**: Performed decently, though some lag was observed due to the older hardware.

### Results:
The FPS (Frames Per Second) for various viewsets showed wide variation depending on the complexity of the task and the hardware. PC2 had the best overall performance, while PC1 struggled with demanding tasks.

## Project 2: DNS Analysis and Performance Testing

### Tools Used:
- **dig**: For querying DNS servers.
- **dnsping**: To measure the response times of DNS queries.
- **dnseval**: To evaluate DNS server performance across different query types.

### Active Experiments:
1. Querying DNS for the name servers of **apple.com**.
2. Retrieving IP addresses of various name servers.
3. Performing WHOIS queries to gather domain registration details.

### Performance Experiments:
- Tested DNS response times using UDP, TCP, DoH (DNS-over-HTTPS), and DoT (DNS-over-TLS) protocols.
- Results showed that UDP had the fastest response times, while DoH and DoT, though more secure, were slower.

### Key Findings:
- **DNS Query Times**: UDP provided the fastest response times, but secure protocols like DoH and DoT introduced latency.
- **Multiple Queries**: Performance varied based on the type of query (A, MX, AAAA) and the DNS server queried.

## Conclusion:
Both projects provided valuable insights into performance benchmarking and DNS analysis. The first project highlighted the importance of dedicated GPUs for handling 3D workloads, while the second project explored DNS performance, emphasizing the trade-off between speed and security in DNS query protocols.

## License
This project is for educational purposes only.

