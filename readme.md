Docker container with apache kudu.

Currently supports launching kudu in one node.

**note** Kudu needs `--use-hybrid-clock=false` flag to run on mac. This is because mac does not run netp service and containers time is always bound to the time of the host.

On ubuntu/centos host with ntp deamon installed and running container can query the time from host. Thus this issue does not occur.

Using `--use-hybrid-clock=false` to disables sync with ntptime. This is not needed if it is running in the same node. But using this is discouraged if running on cluster.

https://github.com/bigdatafoundation/docker-kudu/issues/1