# Decentralized Star Notary Service

### Deploying to Rinkeby

````
Adrians-MacBook-Pro:smart_contracts adrianmohnacs$ truffle deploy --network rinkeby
Using network 'rinkeby'.

Running migration: 1_initial_migration.js
  Deploying Migrations...
  ... 0x88f97ab9599d53207b18dc68293394b4fec5aec51c8bade95569ed21c5017cf9
  Migrations: 0xfc967480dc1761b184aa0d6a392cbae299beab34
Saving successful migration to network...
  ... 0x437069429f62f46d152ebbbf0716468e519f83cf71f5fb4dd8aaa576847b33e8
Saving artifacts...
Running migration: 2_star_notary_migration.js
  Deploying StarNotary...
  ... 0xb74a93a567081ec00aebe0c7b8a36273f75408459a58e753fa5b799b692c2456
  StarNotary: 0x3dbf14c52de3bec278864410f3a085e1e0ae1a8d
Saving successful migration to network...
  ... 0xa002dae863114216bf9f4e9dec07f9e62b121a6083eff4a3ecb4ff3f722f08f5
Saving artifacts...

Migrations: 0xfc967480dc1761b184aa0d6a392cbae299beab34
  StarNotary: 0x3dbf14c52de3bec278864410f3a085e1e0ae1a8d
````

### Front End Configuration

Front-end is configured to:

1) Claim a new star. Each new star support these pieces of metadata:
Star coordinators
Dec
Mag
Cent
Star story
2) Lookup a star by ID using tokenIdToStarInfo()

### Screenshots

<img width="1280" alt="screen shot 2019-02-26 at 6 24 50 pm" src="https://user-images.githubusercontent.com/7444521/53406320-b2700500-39f4-11e9-868a-2ad81029fc48.png">


### Instruction

````
truffle test StarNotaryTest.js
http-server ./web
````
