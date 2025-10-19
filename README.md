🔐 DevSecOps — TryHackMe “On-Prem IaC” Challenge

Analysed and exploited an on-prem Infrastructure-as-Code pipeline (Vagrant + Ansible) that provisioned a Dockerized Flask + MySQL application. Investigated Vagrantfile and Ansible roles, tunneled into the private Docker network, exploited a command-injection vector to spawn a reverse shell, recovered synced SSH keys and authorized_keys changes, pivoted across the internal network, and escalated privileges to capture challenge flags.

Key Areas Covered:

🧭 Vagrant topology analysis (private networks, synced folders, IP mapping)

⚙️ Ansible playbook/template inspection (variable injection into DB/app scripts)

🔌 SSH tunnelling & network pivoting into internal 172.20.128.0/24 Docker network

💥 Command-injection discovery & exploitation in the Flask app (netcat reverse shell)

🔐 Extraction and reuse of synced SSH private keys (chmod 400, ssh -i ...)

🔁 authorized_keys sync trick to gain host user access and lateral movement

🛠️ Privilege escalation to root and flag capture (documented step-by-step evidence)

Skills: Vagrant · Ansible · Docker · Flask · Linux exploitation · SSH tunneling · Network pivoting · Netcat · IaC security · TryHackMe lab experience
