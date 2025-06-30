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

📢 **JOIN TG FOR UPDATES**: [t.me/EarnByAbhi23](https://t.me/EarnByAbhi23)


Perfect bhai! Ye raha full **`README.md`** file ka content jo tu directly `octra_pre_client` repo me daal sakta hai for Codespaces setup:

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

✅ This will install all required libraries:
`aiohttp`, `eth_account`, `web3`, etc.

---

### 🔹 STEP 3: Create and edit wallet.json

Create the wallet file:

```bash
cp wallet.json.example wallet.json
```

Then open the file:

```bash
code wallet.json
```

Paste your test wallet details (⚠️ never use your real wallet):

```json
{
  "address": "0xYourAddressHere",
  "privateKey": "0xYourPrivateKeyHere"
}
```

---

### 🔹 STEP 4: Send a test transaction

```bash
python cli.py send --to 0xReceiverAddress --amount 0.01
```

🟢 That’s it! The CLI will send the transaction using your test wallet.

---

## ⚠️ Notes

* Only use **test wallets**. Never share your mainnet private key.
* This CLI is for dev/testing purposes only.



