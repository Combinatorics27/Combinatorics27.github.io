---
title: "TIL: homomorphic encryption, federated learning"
date: 2026-09-14
categories: til
---

homomorphic encryption can be used to perform computations on an encrypted data without needing to decrypt it. the data stays encrypted. the server performs computations on the encrypted data. the client gets the computed encrypted data back which he can then decrypt.

federated learning is a technique to train ML models in cases of decentralized data. if there are multiple clients with the same structure of data but which they cannot share, federated learning allows training a model without centrally accessing anyone's data. everyone keeps their own data, trains the model on their data, and then only send the update in weights that needs to be done to the server which then aggregates the updates from each of the clients.
