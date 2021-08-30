k3os:
  sysctl:
    kernel.printk: "4 4 1 7"
    kernel.kptr_restrict: "1"
  ntp_servers:
  - 0.us.pool.ntp.org
  - 1.us.pool.ntp.org
  password: rancher
  k3s_args:
  - server
  - "--disable-agent"
  - --disable=traefik
