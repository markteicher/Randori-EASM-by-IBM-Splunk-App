```mermaid
flowchart TD
    Service["Service
id
service_id"]
    Target["Target
id
service_id"]
    AllDetectionsForTarget["AllDetectionsForTarget
hostname_id
id
ip_id
service_id
target_id"]
    IpsForService["IpsForService
id
ip_id
service_id"]
    IpsForHostname["IpsForHostname
id
hostname_id
ip_id"]
    Ip["Ip
id"]
    Hostname["Hostname
id"]
    HostnamesForIP["HostnamesForIP
id
hostname_id
ip_id"]
    IpsForNetwork["IpsForNetwork
id
ip_id
network_id"]
    PortsForIp["PortsForIp
id
ip_id"]
    Network["Network
id"]

    Service --> IpsForService
    Service --> Target
    Target --> AllDetectionsForTarget
    AllDetectionsForTarget --> Hostname
    AllDetectionsForTarget --> IpsForHostname
    AllDetectionsForTarget --> Ip
    IpsForService --> Ip
    IpsForHostname --> Ip
    IpsForNetwork --> Ip
    Network --> IpsForNetwork
    Ip --> PortsForIp
    Ip --> HostnamesForIP

