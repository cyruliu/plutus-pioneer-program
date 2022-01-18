# Homework Notes
The main purpose of this homework is to get familiar with development evironment, get to know aboutl haskell project (compile, package management), nix-shell, and plutus playground (a simulator). I like functional world, feel enjoyable to set them up, excited to understand more about ledger code, data structure in haskell!

## Haskell 
When I was setting up haskell environment, for each haskell project, it's good to know and understand the `cabal.project` and `your-app.cabal` files. 
They help you to manage project dependencise and compiling options for your application respectively.

## Nix-shell
I had a nix-shell [question](https://cardano.stackexchange.com/questions/6479/nix-build-not-found-inside-nix-shell-linux), the rest went smoothly for me.

## Plutus Playground
I was able to run the plutus playground on my linux machine, then recently it fails to run normally, I didn't want to spend too much time debugging, using [playground online](https://playground.plutus.iohkdev.io/) is quite handy, it helps me shift my focus on the haskell code itself.

## Q&A
- PBA is not necessary, it's convinent to use it to build the transaction, we can use plutus api/cardano-cli talk to cardano node too.
- Transaction needs to be validated by the node, on-chain code encodes some criteria that needed by a validator. The off-chain code can be anywhere like a cloud server, a browser application, or PBA etc., the main functionality of off-chain code is query/create/submit transactions on the blockchain.
- Wrtiting on-chain and off-chain code with the same language Haskell.
- Playground is not just a learning toy, we can use it to fast testing our contracts, but with some restrictions (e.g. no staking ability.).
