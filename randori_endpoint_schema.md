```mermaid
flowchart TD
    %% Randori API Endpoint Relationships
    Target["Target<br>id<br>service_id"]
    Service["Service<br>id<br>service_id"]
    AllDetectionsForTarget["AllDetectionsForTarget<br>hostname_id<br>id<br>ip_id<br>service_id<br>target_id"]
    Hostname["Hostname<br>id"]
    IpsForService["IpsForService<br>id<br>ip_id<br>service_id"]
    IpsForHostname["IpsForHostname<br>id<br>hostname_id<br>ip_id"]
    IpsForNetwork["IpsForNetwork<br>id<br>ip_id<br>network_id"]
    Network["Network<br>id"]
    PortsForIp["PortsForIp<br>id<br>ip_id"]
    HostnamesForIP["HostnamesForIP<br>id<br>hostname_id<br>ip_id"]
    Ip["Ip<br>id"]

    %% Relationships
    Service -->|1-to-many| Target
    Target -->|1-to-many| AllDetectionsForTarget
    Service -->|1-to-many| AllDetectionsForTarget
    AllDetectionsForTarget -->|1-to-1| Hostname
    AllDetectionsForTarget -->|1-to-1| Ip
    IpsForService -->|1-to-1| Ip
    IpsForHostname -->|1-to-1| Ip
    IpsForNetwork -->|1-to-1| Ip
    PortsForIp -->|1-to-1| Ip
    HostnamesForIP -->|1-to-1| Ip
    Network -->|1-to-many| IpsForNetwork
