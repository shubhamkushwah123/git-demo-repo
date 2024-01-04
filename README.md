Red Hat Enterprise Linux (RHEL) and its derivatives like CentOS use the yum package manager for installations. Below are the detailed installation steps for each tool on Red Hat-based systems:

1. Java:
Installation:
bash
Copy code
sudo yum install java-1.8.0-openjdk
Verification:
bash
Copy code
java -version
javac -version
2. Python:
Installation:
bash
Copy code
sudo yum install python3
Verification:
bash
Copy code
python3 --version
pip3 --version
3. Git:
Installation:
bash
Copy code
sudo yum install git
Verification:
bash
Copy code
git --version
4. Maven:
Installation:
bash
Copy code
sudo yum install maven
Verification:
bash
Copy code
mvn -v
5. Jenkins:
Installation:
bash
Copy code
sudo yum install java-1.8.0-openjdk
sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat-stable/jenkins.repo
sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key
sudo yum install jenkins
Verification:
Visit http://localhost:8080/ in a web browser. Follow the on-screen instructions, and retrieve the Jenkins unlock key from the Jenkins server.

6. Docker and DockerHub:
Installation:
bash
Copy code
sudo yum install docker
sudo systemctl start docker
sudo systemctl enable docker
Verification:
bash
Copy code
docker --version
docker run hello-world
7. Kubernetes (Minikube):
Installation:
bash
Copy code
sudo yum install conntrack
sudo curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-latest.x86_64.rpm
sudo rpm -ivh minikube-latest.x86_64.rpm
Verification:
bash
Copy code
minikube version
minikube start
8. Ansible:
Installation:
bash
Copy code
sudo yum install ansible
Verification:
bash
Copy code
ansible --version
9. Terraform:
Installation:
bash
Copy code
sudo yum install unzip
sudo curl -LO https://releases.hashicorp.com/terraform/1.0.7/terraform_1.0.7_linux_amd64.zip
sudo unzip terraform_1.0.7_linux_amd64.zip
sudo mv terraform /usr/local/bin/
Verification:
bash
Copy code
terraform --version
10. Prometheus and Grafana:
Prometheus:
Installation:
bash
Copy code
sudo yum install prometheus
Verification:
Visit http://localhost:9090/ in a web browser.

Grafana:
Installation:
bash
Copy code
sudo yum install grafana
sudo systemctl start grafana-server
sudo systemctl enable grafana-server
Verification:
Visit http://localhost:3000/ in a web browser. Default credentials are admin/admin.

These commands should guide you through the installation of the mentioned tools on Red Hat-based systems. If you have any further questions or need additional assistance, feel free to ask!
