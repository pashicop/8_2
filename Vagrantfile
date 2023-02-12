Vagrant.configure("2") do |config|

    config.vm.define "clickhouse" do |clickhouse|
    clickhouse.vm.box = "centos/7"
    clickhouse.vm.hostname = "clickhouse-01"
    clickhouse.vm.network "public_network", bridge: "wlp10s0", ip: "192.168.0.15"
#         use_dhcp_assigned_default_route: true
    end

    config.vm.define "vector" do |vector|
    vector.vm.box = "centos/7"
    vector.vm.hostname = "vector-01"
    vector.vm.network "public_network", bridge: "wlp10s0", ip: "192.168.0.16"
    end
end