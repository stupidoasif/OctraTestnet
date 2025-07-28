# STEP BY STEP WALLET GENERATION GUIDE OF OCTRA { CODESPACE }

---

## 🔹 Step 1: Install Bun

```bash
curl -fsSL https://bun.sh/install | bash
source ~/.bashrc
bun --version
````

---

## 🔹 Step 2: Install Dependencies

```bash
bun install
```

---

## 🔹 Step 3: Build the Project

```bash
bun run build
```

---

## 🔹 Step 4: Start the Server

```bash
bun start
```

> ✅ After this, click the **“PORTS”** tab in Codespace and open `localhost:8888` in browser.

---

**Done! Wallet Generator is live. 🔐**


---
# 🪙 TASK 1 : TOKEN TRANSFER

### 🔹 STEP 1: Open in Codespace

1. Go to 👉 [https://github.com/octra-labs/octra_pre_client](https://github.com/octra-labs/octra_pre_client)
2. Click the green `Code` button  
3. Select → `Open with Codespaces` → `+ New codespace`
4. Wait for the environment to fully load

---

### 🔹 STEP 2: Install dependencies

In the Codespace terminal, run:

```bash
pip install -r requirements.txt
````

---

### 🔹 STEP 3: Create and edit wallet.json

Create the wallet file:

```bash
cp wallet.json.example wallet.json
```

Then open the file: wallet.json

Paste your test wallet details (⚠️ never use your real wallet):
![Wallet Generation](IMG_20250630_110429.png)


```
{
  "priv": "private key here",
  "addr": "octxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "rpc": "https://octra.network"
}
```

---

### 🔹 STEP 4: Send a test transaction

```bash
python cli.py send --to oct5ziFzQJkiJFPfcQeuAmp4vhfQgjwb8gyx2W2TZdGhzJm --amount 0.01
```

🟢 That’s it! You can now access the wallet UI and make transactions to addresses found on the explorer: https://octrascan.io/

---
---
# 🪙 TASK 2 : ENCRYPT / DECRYPT BALANCE

### 🔹 STEP 1: Follow Task 1 Steps & Open Wallet UI

---

### 🔹 STEP 2: 
![Step 1 Screenshot](IMG_20250710_160447.jpg)

• Use Command `4` For Encrypt  
• Use Command `5` For Decrypt  

Keep doing transactions, you can also use other commands like `6` & `7` for private Transfer & Claim , Use Address From Explorer: https://octrascan.io/

---
---
# 🪙 TASK 3 : Run Ocs01 Test Contract

### 🔹 STEP 1: Open in Codespace

1. Go to 👉 https://github.com/octra-labs/ocs01-test
2. Click the green `Code` button  
3. Select → `Open with Codespaces` → `+ New codespace`
4. Wait for the environment to fully load

### 🔹 STEP 2: In the Codespace terminal, run:

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
````

```bash
source $HOME/.cargo/env
```
```bash

git clone https://github.com/octra-labs/ocs01-test.git
cd ocs01-test
```
```bash
cargo build --release
```
```bash
cp EI/exec_interface.json 
```
### 🔹 STEP 3: Create  `wallet.json ` file in ocs01-test

Paste :
```bash
{
  "priv": "0xYOUR_PRIVATE_KEY_HERE",
  "addr": "0xYOUR_WALLET_ADDRESS_HERE",
  "rpc": "https://octra.network"
}
```

### 🔹 STEP 4: Run Octra Test
```bash
./target/release/ocs01-test
```
### 🔹 STEP 5: Run Octra Test

Now Start WIth Command  `3 ` & Till End

![Wallet Generation](Screenshot 2025-07-28 163757.png)

🟢 That’s it!

---
---

📢 **JOIN TG FOR UPDATES**: [t.me/EarnByAbhi23](https://t.me/EarnByAbhi23)

