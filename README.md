# Uniswap V3 Development Book

<p align="center">
  <strong><a href="https://uniswapv3book.com/">Read online</a></strong> ·
  <a href="https://uniswapv3book.com/print.html">Print / PDF</a>
</p>

Overview
--------
The Uniswap V3 Development Book is a practical, developer-focused guide that walks through building a functional clone of Uniswap V3. The book emphasizes the protocols, smart-contract design, and engineering trade-offs behind concentrated-liquidity automated market makers (AMMs). It is intended for developers who want a hands-on walkthrough of advanced Solidity and on-chain design patterns.

Key goals
- Explain the core economics and math behind constant-product AMMs and Uniswap V3.
- Implement an educational, end-to-end Uniswap V3 clone (smart contracts + simple UI).
- Demonstrate practical Solidity patterns, fixed-point math, and testing techniques.
- Preserve safety by clearly marking differences from production Uniswap; do not deploy this code to mainnet.

What this repository contains
- The book content (Markdown source for the guide).
- Diagrams and reference images used in the book.
- Development notes and local build scripts for mdBook.

What you will learn
- AMM fundamentals and price mechanics.
- Liquidity math and fixed-point arithmetic in Solidity.
- Contract architecture for pools, factories, and position managers.
- Building a minimal front-end to interact with the contracts.
- Testing, deployment, and common pitfalls when implementing AMMs.

Repository structure (high level)
- src/           — mdBook source files and chapters
- src/images     — images used in the book
- examples/      — (optional) reference code snippets or mocks
- README.md      — this overview and local development instructions

Important disclaimer
This project is an educational clone and intentionally diverges from production Uniswap V3 in places for clarity and pedagogical reasons. It contains intentionally simplified code and known limitations. Do not use it as-is for mainnet deployments.

Quick start — run the book locally
1. Install Rust (https://www.rust-lang.org/).
2. Install mdBook and the KaTeX plugin:
   ```powershell
   cargo install mdbook
   cargo install mdbook-katex
   ```
3. Clone the repository and change directory:
   ```powershell
   git clone https://github.com/0xAllan123/uniswapv3-book
   cd uniswapv3-book
   ```
4. Serve the book locally:
   ```powershell
   mdbook serve --open
   ```
   The command will start a local server and open the book in your browser (default http://localhost:3000).

Contributing
- Issues and discussions are welcome: https://github.com/0xAllan123/uniswapv3-book/discussions
- Keep changes focused, add tests or examples where appropriate, and follow the existing Markdown style.
- When contributing code that modifies examples, clearly document any behavioral differences from the text.

Support and discussion
- For questions about book content or milestones, use the repository Discussions page:
  https://github.com/0xAllan123/uniswapv3-book/discussions

License
- The book and repository are available under the repository's license. See the LICENSE file for details.

Acknowledgements
- The book builds on concepts popularized by Uniswap and other AMM research. See references inside the chapters for original sources and further reading.