# Tstat — TCP STatistic and Analysis Tool

Tstat is a passive traffic monitor. It analyses packets captured on a link, or read from trace files, and reports statistics on the traffic at both the network and transport levels.

For every TCP and UDP flow, Tstat writes a log line with hundreds of metrics: volumes, round-trip times, losses, retransmissions and timings. It also identifies the application in use, such as HTTP, TLS (with the server name), QUIC, DNS and video streaming. Aggregate statistics are kept as RRD time series and histograms.

Tstat was born at Politecnico di Torino and has been used for years in research and on real ISP and campus networks.

## Repositories

| Repository | Description |
|---|---|
| [tstat](https://github.com/Tstat-TCP-STatistic-and-Analysis-Tool/tstat) | The Tstat traffic analyser and the `libtstat` library. Reads live traffic via libpcap or pcap/pcapng trace files. |
| [tstat-dpdk](https://github.com/Tstat-TCP-STatistic-and-Analysis-Tool/tstat-dpdk) | A DPDK wrapper that runs several Tstat instances in parallel on DPDK-compatible NICs, splitting traffic with symmetric RSS, to monitor links at 40+ Gbit/s. |
| [rrd-viewer](https://github.com/Tstat-TCP-STatistic-and-Analysis-Tool/rrd-viewer) | A web viewer (CGI and Docker image) for the RRD files produced by Tstat. |
| [cpan-tools](https://github.com/Tstat-TCP-STatistic-and-Analysis-Tool/cpan-tools) | Tools to anonymize IPv4/IPv6 addresses with Crypto-PAn, compatible with the anonymization done by Tstat. |
