# Install Dependencies

**1. Update System Packages**
```bash
sudo apt-get update && sudo apt-get upgrade -y
```
**2. Install General Utilities and Tools**
```bash
sudo apt install screen curl iptables build-essential git wget lz4 jq make gcc nano automake autoconf tmux htop nvme-cli libgbm1 pkg-config libssl-dev libleveldb-dev tar clang bsdmainutils ncdu unzip libleveldb-dev  -y
```

**3. Install Docker**
```bash
# Remove old Docker installations
for pkg in docker.io docker-doc docker-compose podman-docker containerd runc; do sudo apt-get remove $pkg; done

# Install dependencies
sudo apt install apt-transport-https ca-certificates curl software-properties-common -y

# Add Docker’s official GPG key
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg

# Set up the stable Docker repository
echo "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

# Install Docker
sudo apt install docker-ce docker-ce-cli containerd.io -y

# Verify Docker installation
sudo docker --version

# Start and enable Docker
sudo systemctl enable docker
sudo systemctl start docker

# Run Docker without sudo (optional)
sudo usermod -aG docker $USER

# Test Docker installation
docker run hello-world

```
**4. Install Python**
```bash
sudo apt-get install python3 python3-pip python3-venv python3-dev -y
```

**5. Install Node**
```
sudo apt-get update
```
```
curl -fsSL https://deb.nodesource.com/setup_22.x | sudo -E bash -
```
```
sudo apt-get install -y nodejs
```
```
node -v
```
```bash
sudo npm install -g yarn
```
```bash
yarn -v
```

**6. Install Yarn**
```bash
curl -o- -L https://yarnpkg.com/install.sh | bash
```
```bash
export PATH="$HOME/.yarn/bin:$HOME/.config/yarn/global/node_modules/.bin:$PATH"
```
```bash
source ~/.bashrc
```

---

## 2) Get HuggingFace API Key 
**1- Create account in [HuggingFace](https://huggingface.co/)**

**2- Create an Access Token with `Write` permissions [here](https://huggingface.co/settings/tokens) and save it**

---

## 3) Clone the Repository
```bash
git clone https://github.com/gensyn-ai/rl-swarm/
```
```
cd rl-swarm
```
---

## 4) Run the Node (For VPS)
Open a screen to run it in background
```bash
screen -S swarm
```
### To run the Node
```bash
python3 -m venv .venv
```
```
source .venv/bin/activate
```
```
./run_rl_swarm.sh
```
Press `Y`

---







* Official dashboard: https://dashboard.gensyn.ai/

**You can search your Node name in the dashboard after a while when you have done your first training completed**
