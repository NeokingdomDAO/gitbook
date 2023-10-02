# dApp - High-level overview

The NEOKingdom DAO dApp is a Decentralized Application that can be accessed using a web browser or as a standalone application on a mobile device or desktop. It allows NEOKingdom DAO contributors to interact with the smart contracts for voting on governance topics via their cryptocurrency wallets and to keep track of the time and tasks they contribute to the DAO.

The dApp not only allows users to interact with the Smart Contracts in a seamless way, but it also offers the possibility to integrate with the ERP system via crypto wallets rather than passwords. We integrate with the smart contracts through the graph protocol API to read the data and through the wallet and client-side javascript code to write into the blockchain. We have a backend API layer to read and write to/from Odoo.

### Features&#x20;

* Track time through integration with Odoo, an Enterprise Resource Planning (ERP) software system that helps the DAO to automate and manage core processes. It integrates with Odoo via an API layer backend;
* View information stored in the blockchain through the integration with the Smart Contracts and perform transactions (i.e., to create/vote on resolutions or to exchange/offer tokens). An event-sourced system, the “graph protocol,” stores all the events triggered by the Smart Contracts and makes them available via a read-only GraphQL API that the dApp interfaces with;&#x20;
* A dashboard that offers a clear overview of what’s going on in the DAO at any given time;
* Seamless password-less integration with their crypto wallet.&#x20;

### Development and Deployment

Our development process is open and managed through GitHub. We use a continuous integration/continuous deployment (CI/CD) platform called “vercel” that allows us to immediately release fixes, do rollbacks, and to maintain the dApp, without needing to worry about the infrastructure.

### Security

The dApp is secure by design, as every operation performed in the Smart Contracts requires authorization by the user via their crypto wallet. Moreover, the information that we display is retrieved from the immutable and transparent data stored on the blockchain.&#x20;

For use of Odoo, users also need to login using their crypto wallet. Finally, the dApp is served through https.&#x20;

We use [https://mui.com](https://mui.com)  to develop the features in the dApp, for superior UX.
