# riemann-world
riemann custom

~]# riemann-health --help
Options:
  -h, --host=<s>              Riemann host (default: 127.0.0.1)
  -p, --port=<i>              Riemann port (default: 5555)
  -e, --event-host=<s>        Event hostname
  -i, --interval=<i>          Seconds between updates (default: 5)
  -t, --tag=<s>               Tag to add to events
  -l, --ttl=<i>               TTL for events
  -a, --attribute=<s>         Attribute to add to the event
  -m, --timeout=<i>           Timeout (in seconds) when waiting for acknowledgements (default: 30)
  -c, --tcp, --no-tcp         Use TCP transport instead of UDP (improves reliability, slight overhead. (Default: true)
  -u, --cpu-warning=<f>       CPU warning threshold (fraction of total jiffies) (default: 0.9)
  -r, --cpu-critical=<f>      CPU critical threshold (fraction of total jiffies) (default: 0.95)
  -d, --disk-warning=<f>      Disk warning threshold (fraction of space used) (default: 0.9)
  -s, --disk-critical=<f>     Disk critical threshold (fraction of space used) (default: 0.95)
  -o, --load-warning=<i>      Load warning threshold (load average / core) (default: 3)
  --load-critical=<i>         Load critical threshold (load average / core) (default: 8)
  -w, --steal-warning=<i>     Steal warning threshold (default: 10)
  --steal-critical=<i>        Steal critical threshold (default: 30)
  -y, --memory-warning=<f>    Memory warning threshold (fraction of RAM) (default: 0.85)
  --memory-critical=<f>       Memory critical threshold (fraction of RAM) (default: 0.95)
  -k, --checks=<s+>           A list of checks to run. (Default: cpu, load, memory, disk, steal)
  --help                      Show this message

~]# riemann-portcheck --help
Options:
  -h, --host=<s>          Riemann host (default: 127.0.0.1)
  -p, --port=<i>          Riemann port (default: 5555)
  -e, --event-host=<s>    Event hostname
  -i, --interval=<i>      Seconds between updates (default: 5)
  -t, --tag=<s>           Tag to add to events
  -l, --ttl=<i>           TTL for events
  -a, --attribute=<s>     Attribute to add to the event
  -m, --timeout=<i>       Timeout (in seconds) when waiting for acknowledgements (default: 30)
  -c, --tcp, --no-tcp     Use TCP transport instead of UDP (improves reliability, slight overhead. (Default: true)
  -o, --hostname=<s>      Host, defaults to localhost (default: riemann-server.localdomain)
  -r, --ports=<i>         Port to check, e.g. '-r 80'
  -s, --opsi=<i>          1: ping, 2: port, 3: ping & port
  --help                  Show this message


~]# check_ping_port_riemann --help
Usage :
        ./check_ping_port -H [STRING] -p [VALUE]

        OPTION          DESCRIPTION
        ----------------------------------
        -h              Help
        -H [STRING]     Riemann Server
        -p [VALUE]      Riemann Port
        -i [VALUE]      Interval
        -l [VALUE]      TTL
        -t [VALUE]      Tag
        ----------------------------------
Note : [VALUE and PORT] must be an integer.

