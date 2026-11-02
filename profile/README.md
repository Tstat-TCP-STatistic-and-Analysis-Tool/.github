# Tstat — TCP STatistic and Analysis Tool

Tstat is a passive traffic monitor. It analyses packets captured on a link, or read from trace files, and reports statistics on the traffic at both the network and transport levels.

For every TCP and UDP flow, Tstat writes a log line with hundreds of metrics: volumes, round-trip times, losses, retransmissions and timings. It also identifies the application in use, such as HTTP, TLS (with the server name), QUIC, DNS and video streaming. Aggregate statistics are kept as RRD time series and histograms.

Tstat was born at Politecnico di Torino and has been used for years in research and on real ISP and campus networks.
