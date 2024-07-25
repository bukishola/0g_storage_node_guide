# 0g_storage_node_guide
A simple guide to launching Storage node


## Hardware Requirement
- Memory: 16 GB RAM
- CPU: 4 cores
- Disk: 500GB / 1T NVME SSD
- Bandwidth: 500 MBps for Download / Upload

## Download the source code
```bash
git clone https://github.com/0glabs/0g-storage-client.git
cd 0g-storage-client
go build
```

## Run the file upload/download commands
```bash
# file upload
./0g-storage-client upload --url <blockchain_rpc_endpoint> --contract <log_contract_address> --key <private_key> --node <storage_node_rpc_endpoint> --file <file_path>
# file download
./0g-storage-client download --node <storage_node_rpc_endpoint> --root <file_root_hash> --file <output_file_path>
# file download with verfication
./0g-storage-client download --node <storage_node_rpc_endpoint> --root <file_root_hash> --file <output_file_path> --proof
```
