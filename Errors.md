# Error 1
![photo_2025-05-01_11-22-34](https://github.com/user-attachments/assets/7c88f415-9bd7-4762-be8f-7c32964bf700)

## -Error Localhost refused to Connect
### FOLLOW THESE STEPS
# Install Ngork
```
wget https://bin.equinox.io/c/bNyj1mQVY4c/ngrok-v3-stable-linux-amd64.tgz && tar -xvzf ngrok-v3-stable-linux-amd64.tgz && sudo mv ngrok /usr/local/bin/
```
visit: https://ngrok.com

- Sign up using email
- Go to Your Authtoken Section
- Click on "show authtoken" 
- Copy that command
- Go back paste and run the command
## Now Connect with Ngrok
```
ngrok http 3000
```
![Screenshot 2025-05-11 164248](https://github.com/user-attachments/assets/c61b5fd3-2db7-448a-b232-1abcf0adce68)
 - Copy the underlined link
 - Paste it on any browser and visit the site
 - Login on the gensyn website
# Error 2

![photo_2025-05-11_15-42-54](https://github.com/user-attachments/assets/34f66666-d7d8-4bf8-97f4-486dade53d7b)

### Check On Image - Failed To Complie
```
cd /root/rl-swarm/modal-login/ && yarn upgrade &&  yarn add next@latest &&  yarn add viem@latest
```
### Yarn Cache Clear
```
yarn cache clean
```
### Probuf Error
```
pip install protobuf==6.30.0
```

-Next do manual CMD 
```
nano requirements-CPU.txt
```
transformers - 6.30.0
save with cmd ctrl+O, Enter & Ctrl+X

If this cmd is not working then use protobuf version 4.46.0

### Hivemind Error
```
nano $(python3 -c "import hivemind.p2p.p2p_daemon as m; print(m.__file__)")
```
-Find
 startup_timeout: float = 15

Change  120

then save with cmd ctrl+O, Enter & Ctrl+X

# Minor Node Updates
- No Change in installation process
- Minor UI changes
- Introduction of low optimisation models

  # No Further Updates, if you face any other errors, make sure to visit their Discord for help
- Here's the discord link (https://discord.com/channels/852932483691577395/922626442934767687)
