# FAQ

## Let's get started

### 1. What is Immu3?

Immu3 is the complete developer platform for pioneering the future of global on-chain communication with low-code tooling and configurability you need to accelerate from idea to launch.

### 2. Why is on-chain communication important?

In apps built on the Immu3 infra stack, each mail, message or data file sharing is an L1/L2 transaction, while larger files are stored on decentralized storage. This model enables true decentralized communication that is non-custodial, permissionless, immutable, and resistant to Web2 data mining, contrasting sharply with traditional off-chain centralized communication.

### 3. What is the difference between legacy Web2 communication platforms and apps built on Immu3? <a href="#id-3.-what-is-the-difference-between-legacy-web2-communication-platforms-and-4p-super-app" id="id-3.-what-is-the-difference-between-legacy-web2-communication-platforms-and-4p-super-app"></a>

Legacy email applications use centralized databases and often lack E2E encryption. Users pay with their data, which is mined by the app. This Web2 model leads to data ownership loss, potential de-platforming, identity theft, spam, spoofing, and privacy loss.

The Immu3-based apps can be characterised as decentralized Web3 applications with no centralized database, giving users full control over their data. This approach prevents Web2 issues like data mining, data ownership loss, and de-platforming. It ensures secure, permissionless, immutable, self-custodial P2P on-chain communication.

### 4. What is the difference between dMail/dChat and BlockMail/BlockChat?

We refer to blockchain-based Mail/Chat as BlockMail/BlockChat. The Immu3 platform supports on-chain communication, with the level of decentralization matching that of the underlying network. Hence, terms like decentralized Mail/Chat, or dMail/dChat, are also applicable. However, given potential questions about some blockchain networks' decentralization, we prefer BlockMail/BlockChat. Sometimes the term on-chain email/message is also used within the Immu3 documentation. Ultimately, the choice of naming comes down to user preference.

### 5. Who can use Immu3?

Immu3 is an infrastructure and protocol stack platform for integrators to develop on-chain communication-based mail, messaging, and data-sharing apps. Simultaneously, the Immu3  AppSuite was created to provide permissionless access for anyone to use. Users can connect their MetaMask, Coinbase, or WalletConnect-supported wallets to experience on-chain communication within polished Web3 UIs:

* **BlockCommunicator**: A blockchain-based alternative to traditional email and messaging. This app allows users to communicate on-chain in a self-custodial manner, ensuring security and preserving data ownership.
* **W3XShare**: A decentralized alternative to "WeTransfer," enabling secure, self-custodial data file sharing that protects against data ownership loss and data mining.
* **PX Drive:** A decentralized storage application that allows users to store and access files online in a true self-custodial and permissionless way.

### 6. What is the integration cost?

There is no cost for integrators to utilise the OCC (i.e. on-chain communication) SDK and White labels. Immu3 charges the protocol base fee to earn money. To understand monetization read the [Fees & Integrator Economics](https://wiki.immu3.io/integrators/fees-and-integrator-economics) chapter.

### 7. What is the cost of using Immu3 AppSuite?

Parallel to the underlying L1/L2 transaction gas cost, the service fees (i.e. protocol fees) are also settled on the smart contract level and are applicable for every mail, message or data-sharing transaction. Total user cost equals the sum of the L1/L2 transaction gas and the service fees. The gas and service fees converge and manifest as one end-user communication transaction fee. [Read more](https://wiki.immu3.io/integrators/fees-and-integrator-economics).

### 8. How can I become an integrator and do I need to be a developer?

Permissionless integrator licences will be available via the Immu3 Integrator Dashboard and are perfect for teams wanting to build their on-chain communication apps. The Integrator Dashboard will unlock the skill and know-how required to abstract the complexities and simplify the deployment of on-chain communication apps. Anyone, not only developers will be able to deploy the mail or messaging apps in an hour.

## Technical

### 9. How does it work? <a href="#id-6.-how-does-it-work" id="id-6.-how-does-it-work"></a>

The message exchange happens on-chain as one short message represents one L1/L2 blockchain transaction. As the mailing or data file sharing process is data heavier, lite encrypted JSON objects are created to hold mail metadata. The link to this metadata and checksum is recorded on the chain as a blockchain transaction. So again, the core primitive described by the formula below applies;

* 💡1 blockchain mail/message/data-sharing= 1 L1/L2-TX

### 10. Which blockchain does Immu3 support? <a href="#id-7.-which-blockchain-can-i-use-to-connect-to-4p" id="id-7.-which-blockchain-can-i-use-to-connect-to-4p"></a>

Immu3 is supporting all EVM (e.g., Ethereum, Binance Smart Chain, Polygon, etc.), but is adding deployments in a planned timeframe. The first batch of deployments includes Fantom Opera, Oasis, Zeta, Edgeware, Arthera and Immu3 blockchains.

### 11. Where is my data stored? <a href="#id-9.-where-is-my-data-stored" id="id-9.-where-is-my-data-stored"></a>

Integrators can select the storage used within their apps, determining the data storage location. The OCC SDK and White labels integrate PollinationX's decentralized storage service by default. When chosen, it utilizes BTFS (i.e. Bittorrent file system) for self-custodial storage of encrypted user data. In the end-user AppSuite, mails and attachments are encrypted and stored on both decentralized storage and local devices, while encrypted messaging data is stored on-chain.

## User Experience & Features <a href="#user-experience-and-features" id="user-experience-and-features"></a>

### 12. Can I send images, videos and attachments through Immu3 AppSuite? <a href="#id-10.-can-i-send-images-videos-and-attachments-through-4p" id="id-10.-can-i-send-images-videos-and-attachments-through-4p"></a>

Yes, you can send any type of data file as a mail attachment through BlockCommunicator or use the W3XShare data file transfer app for larger data files. The user's PX sNFT determines storage availability (e.g., 100MB, 1GB, 10GB, 20GB) and by that, it defines the data file transfer size.&#x20;

### 13. What is the PX sNFT and do I need it? <a href="#id-11.-what-is-the-px-snft-and-do-i-need-it" id="id-11.-what-is-the-px-snft-and-do-i-need-it"></a>

PX sNFTs (i.e. PollinationX Decentralized Storage NFTs) let users mint self-custodial storage units with specific capacities (e.g., 100MB, 5GB, 10GB, 20GB, 100GB) for upload bandwidth. PollinationX offers the first 100MB sNFT of storage for free. Users can upgrade their storage with larger PX sNFTs. Unlike centralized storage, which often mines and sells user data for "free" plans, PX sNFTs ensure your data remains private. If you're only using text messaging within the BlockCommunicator without data or media file exchanges, PX sNFTs are not needed.

### 14. Why do I need to install the Encryptor extension into my browser? <a href="#id-12.-why-do-i-need-to-install-the-encryptor-extension-into-my-browser" id="id-12.-why-do-i-need-to-install-the-encryptor-extension-into-my-browser"></a>

Encryptor extension adds the communication end-to-end encryption layer within the BlockCommunicator app that is currently not supported in major wallets. It enables user encryption self-custody not available before in any digital communication.

### 15. How do I enable the Premium BlockCommunicator version? <a href="#id-13.-how-do-i-enable-pro-version" id="id-13.-how-do-i-enable-pro-version"></a>

BlockCommunicator Premium unlocks advanced mail and chat features like the send mail tab, mail whitelisting, chat group creation and lower transaction fees. It requires a Premium subscription which you can enable within the app.&#x20;

### 16. Can I create a group chat in BlockCommunicator? <a href="#id-14.-can-i-create-a-group-chat-in-4p" id="id-14.-can-i-create-a-group-chat-in-4p"></a>

Yes, Premium users can create encrypted on-chain group chats. They can create unlimited group chats with any number of participants and manage groups by adding or removing member wallet addresses.

### 17. How does mail address whitelisting work? <a href="#id-15.-how-does-email-address-whitelisting-work" id="id-15.-how-does-email-address-whitelisting-work"></a>

Mail address whitelisting is a smart contract feature that allows you to whitelist specific wallet addresses, permitting them to contact you. This provides an ultimate filter and true security tool. It is available in the BlockCommunicator Premium version.

## Other

### 18. The Team behind Immu3?

Immu3 represents an open-source collection of protocols created by a community of researchers and developers. The repositories are maintained by the Immu3 core team with contributions made by approximately 8 developers.

### 19. How can I contribute? <a href="#id-17.-how-can-i-contribute" id="id-17.-how-can-i-contribute"></a>

Contributions from the development community are highly encouraged and appreciated. Feel free to submit GitHub issues, pull requests, or offer general feedback.

