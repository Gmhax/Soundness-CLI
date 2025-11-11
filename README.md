# Soundness-CLI

# Installation process

# Knight tour pattern
<img width="568" height="425" alt="image" src="https://github.com/user-attachments/assets/fca4760a-d966-47fd-b1fa-a55e7db0a38f" />


- Use Codespace https://github.com/codespaces
<img width="1575" height="845" alt="image" src="https://github.com/user-attachments/assets/0bd0003c-d8e2-4721-ab77-b2b94395ee6f" />

## Soundness Layer Setup Guide (Step-by-Step)
1. Update your system packages
```
sudo apt update && sudo apt upgrade -y
```

2. Install soundnessup
```
curl -sSL https://raw.githubusercontent.com/soundnesslabs/soundness-layer/main/soundnessup/install | bash
```

 3. Refresh your shell (to load the new command)
```
source ~/.bashrc
```

 4. Install Rust (required for running CLI tools)
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

5. Source Rust environment
```
source $HOME/.cargo/env
```

6. Install Soundness CLI
```
soundnessup install
```

NOTE: You have 2 options at this point:
🔹 If this is your first time, proceed with Step 7 to generate a new key.
🔹 If you already have a 24-word seed phrase from a previous setup, skip to Step 8 to import it.

 7. Generate a new key
```
soundness-cli generate-key --name my-key
```
- Choose and enter a password
- Save the seed phrase and public key shown on screen
✅ IMPORTANT: Do not share your seed phrase with anyone.
## Save your key
-After generating your key, a file named key_store.json will be created.
- To find where it is saved, run:
```
ls ~/.soundness/keys/
key_store.json
```

8. Import an existing key (optional)
- If you already have your 24-word seed phrase, you can restore your key with:
```
soundness-cli import-key --name my-key --mnemonic "your 24-word seed phrase"
```


 9. Register your public key to join the testnet
Go to the Soundness Discord server https://discord.gg/tAh8e9Wd
- Enter the #testnet-access channel
- Type the following command:
```
!access your_pub_key_here
```


8-Queens (92 Solutions): https://docs.google.com/spreadsheets/d/1J_fkd-6NA43zy5W61-cvSPRMGLB_S8Y4tuiBpi84HsE/edit?usp=sharing&pli=1&authuser=0

# Done






