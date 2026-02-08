```mermaid
flowchart TD
    Service["Service\nid\nservice_id"]
    Target["Target\nid\nservice_id"]
    AllDetectionsForTarget["AllDetectionsForTarget\nhostname_id\nid\nip_id\nservice_id\ntarget_id"]
    IpsForService["IpsForService\nid\nip_id\nservice_id"]
    IpsForHostname["IpsForHostname\nid\nhostname_id\nip_id"]
    Ip["Ip\nid"]
    Hostname["Hostname\nid"]
    HostnamesForIP["HostnamesForIP\nid\nhostname_id\nip_id"]
    IpsForNetwork["IpsForNetwork\nid\nip_id\nnetwork_id"]
    Network["Network\nid"]
    PortsForIp["PortsForIp\nid\nip_id"]

    %% Relationships (as plain arrows matching screenshot)
    Service --> Target
    Target --> AllDetectionsForTarget
    Service --> AllDetectionsForTarget
    AllDetectionsForTarget --> Hostname
    AllDetectionsForTarget --> Ip
    IpsForService --> Ip
    IpsForHostname --> Ip
    Ip --> HostnamesForIP
    IpsForNetwork --> Ip
    Network --> IpsForNetwork
    Ip --> PortsForIp

