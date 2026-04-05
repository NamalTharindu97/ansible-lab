FROM ubuntu:22.04

RUN apt-get update && apt-get install -y \
    ansible openssh-client sshpass python3 \
    && rm -rf /var/lib/apt/lists/*

# Generate SSH key pair at build time
RUN ssh-keygen -t rsa -N "" -f /root/.ssh/id_rsa

WORKDIR /playbooks
CMD ["sleep", "infinity"]