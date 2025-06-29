#Multi-Chain-Wallet-Crawler
This project is a **Python-based blockchain transaction crawler and graph builder** for tracing wallet activity across Ethereum, Arbitrum, and Optimism.  
It classifies wallets (e.g., CEX, smart contract, hot wallet, or EOA) and builds a transaction network you can visualize in **Gephi** or any graph analysis tool.
these project is not the final version as it would be upgraded in coming years. the final version would be able to tell you which wallets have been blacklisted and which wallets are deposits to CEXs and what are those CEXs.

---

## 🚀 Features

- 🌐 Crawls **Ethereum**, **Arbitrum**, and **Optimism** blockchains.
- 📦 Uses **Etherscan**, **Arbiscan**, **Optimistic Etherscan**, **Bitquery**, and **Covalent** APIs for fallback.
- 🕵️ Classifies wallets:
  - Static CEX
  - Smart Contract
  - Likely Hot Wallet
  - EOA
- 🗂️ Exports:
  - `trace_combined.csv` — all transactions found.
  - `classified_nodes.csv` — each address with its class.
  - `trace_graph.gexf` — graph format for **Gephi** visualization.

---

## 🛠️ Technologies Used

- Python
- `requests`, `pandas`, `web3`, `networkx`
- Etherscan, Bitquery, Covalent APIs

---

## ⚙️ How to Run

1. **Clone the repo**
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
2. Install dependencies

pip install requests pandas web3 networkx


3. Set your API keys

Edit the Python file to insert your own:

INFURA key

Etherscan / Arbiscan / Optimism key(s)

Bitquery key (optional)

Covalent key 



4. Run the script

python tracer.py

It will:

Crawl transactions up to MAX_HOPS

Save trace_combined.csv, classified_nodes.csv, and trace_graph.gexf





---

📊 Visualize the Graph

Open trace_graph.gexf in Gephi or Gephi Lite to explore the wallet network.


---

📜 License

This project’s source code is made publicly visible for educational and demonstration purposes only.
All rights reserved by the author.
Do not copy, modify, or redistribute without explicit permission.

© Mohammed Mubarak Danjuma, 2025. All rights reserved.


---

🙋 Author

Mohammed Mubarak Danjuma

https://www.linkedin.com/in/mohammed-mubarak-danjuma-0a760227b?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app


---

✅ Notes

Adjust MAX_HOPS in the code to limit the crawl depth.

Be mindful of API rate limits.

Use at your own discretion for learning and demonstration only.
