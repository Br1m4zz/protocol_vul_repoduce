# steps:
1. build dockerfile
2. copy nyx_net_payload_executor.py and crash_reproduce into docker
3. run ``proftpd: ./proftpd -n -c ${WORKDIR}/basic.conf -X``
4. run ``python nyx_net_payload_executor.py crash_reproduce/cnt_xxx.py tcp 21``