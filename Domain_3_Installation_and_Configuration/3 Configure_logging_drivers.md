# Configure logging drivers

## Official Docker Documentation
[Configure logging drivers](https://docs.docker.com/engine/admin/logging/overview/)  

## Linux /etc/docker/daemon.json
## Windows C:\ProgramData\docker\config\

## Default JSON format
{
  "log-driver": "syslog"
}

## Optional syslog format
{
  "log-driver": "json-file",
  "log-opts": {
    "labels": "production_status",
    "env": "os,customer"
  }
}
