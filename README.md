# mlxcontainer
Mellanox Config Tools Container

Run container with high priviliges to get hardware access.

Bash:
docker run --privileged --entrypoint /bin/bash -it xeroxxx/mlxcontainer

Set MLX Card to Ethernet:

lspci


mlxconfig -d <pcie_id> set LINK_TYPE_P1=2 LINK_TYPE_P2=2

Allows you to configure Mellanox Connect-X Cards within a container, for example on a synology NAS where you're not able to install mlxconfig.
