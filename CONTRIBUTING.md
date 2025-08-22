🤝 Contributing to ProofPDF

Welcome to **ProofPDF** — a modular, verifiable document toolkit built on the **ProofPWA** framework.  
This project enables developers to create installable, trust-first applications with advanced PDF tools and zero-knowledge data verification.

We’re excited to have you here! Whether you're fixing bugs, adding features, improving documentation, or extending smart contract logic — your contributions matter.



🛠️ How to Contribute

1. **Fork** the repository  
2. **Create a new branch**  
   ```bash
   git checkout -b feature/your-feature-name

3. Make your changes


4. Test thoroughly


5. Submit a pull request with a clear description of your changes



🧪 Development Guidelines

Follow consistent naming conventions & formatting

Use semantic commits (e.g., feat: add zkTLS badge, fix: resolve PDF merge bug)

Document new components & APIs

Write unit tests for critical logic

Keep UI components modular & reusable




📦 Project Structure

proofpdf/
├── public/                 # Static assets
├── src/
│   ├── components/         # Reusable UI modules
│   ├── pages/              # Route-based views
│   ├── services/           # API + blockchain integrations
│   ├── utils/              # Helper functions
│   └── styles/             # Global & scoped styles
├── manifest.json           # PWA metadata
├── service-worker.js       # Offline caching logic
└── README.md



🔐 Verifiability Modules

Reclaim Integration — verify Web2 API data with zkTLS:

import { fetchProof } from '@xion/reclaim-sdk';

const proof = await fetchProof('https://api.github.com/users/username');

DocuStore Smart Contract — store structured metadata:

const doc = {
  userId: '0x123',
  documentHash: 'abc123',
  verifiedSources: ['GitHub', 'Strava']
};
await docuStore.save(doc);

Crossmint Checkout — mint digital certificates:

import { mintNFT } from '@crossmint/sdk';

mintNFT({
  recipient: userWallet,
  metadata: { title: 'Verified Resume', proof: proofHash }
});



🌍 Use Case Templates

App Type	Implementation

Verified Resume	Pull GitHub data → verify via zkTLS → embed in PDF
Workout Log	Sync Strava → verify progress → attach to fitness report
Event Attendance	Scan QR → store zkTLS proof → generate certificate
Medical Records	Upload health data → verify via API → share securely



📣 Acknowledgments

This project is built with support from:

XION — zkTLS, DocuStore, walletless contracts

Reclaim Protocol — Web2 data verification

Crossmint — NFT minting & digital assets

Storyblok — Composable content management

Devpost — Hackathon inspiration & community



📜 License

Licensed under the terms of the MIT License.


💬 Contact

For questions, feedback, or collaboration:

GitHub Issues

Devpost → oracle69digitalmarketing

Twitter → @sophiemabel69
