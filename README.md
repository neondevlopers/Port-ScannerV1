Run Tools
~~~sh 
python --veraion 
cd Tools
python cypherx_exploit.py 
~~~
• How To Scan ? 

: Basic Scan
~~~sh 
python cypherx_exploit.py example.com (Basic Scan)
~~~
: Fast Scan 
~~~sh
python cypherx_exploit.py example.com --quick (Fast Scan)
~~~
: Port Scan Specific
~~~sh
# Port 80, 443, 22
python cypherx_exploit.py example.com -p 80,443,22

# Port 1-1000
python cypherx_exploit.py example.com -p 1-1000

# Port 1-65535 
python cypherx_exploit.py example.com -p 1-65535
~~~
: Scan The Network 
~~~sh 
# Scan IP 192.168.1.1
python cypherx_exploit.py 192.168.1.1 -p 1-1000

# Scan IP 10.0.0.1
python cypherx_exploit.py 10.0.0.1 -p 80,443,22,3306

# Scan localhost
python cypherx_exploit.py 127.0.0.1 --quick
~~~
: Very Fast Scan 
~~~sh 
# Use Threads 200 For Fast Scan 
python cypherx_exploit.py example.com -p 1-1000 -t 200

#  Set timeout 3 MN
python cypherx_exploitpy example.com --timeout 3 -t 100
~~~
: By NeonDevlopers
