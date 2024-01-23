# LasticUI

Welcome to the **LasticUI** repository! This repository is dedicated to enabling seamless interaction with the Coretime Parachain.

## 🌿 Branch Structure
There are 3 main branches that are relevant: 
 - `development` - this branch contains most recent development
 - `main` - this branch is features deployments that have yet to be tested and released to the public. The deployment of [main branch inside folder `./static-frontend`](https://github.com/LasticXYZ/LasticUI/tree/main/static_frontend) can be also accessed on [test.lastic.xyz](https://test.lastic.xyz/)
 - `stable` - features the stable branch that is tested, this is the branch that is deployed on [lastic.xyz](https://lastic.xyz/)

## 📁 Directory Overview
`./substrate-interact`: 
   - Developed on top of the [`substrate-front-end-template`](https://github.com/substrate-developer-hub/substrate-front-end-template.git).
   - By following the guidelines in `./substrate_interact/README.md`, you can interact with the Coretime chain seamlessly.

### 🚚 Repository Migration
 - `./core_chain_sdk` has moved! Check out [LasticSDK](https://github.com/LasticXYZ/lastic-sdk) for the SDK development tailored for Coretime chain interactions.

## 🚀 Quick Start

### Prerequisites
Before you begin, ensure you have the Substrate node running. To spin up a local Substrate node run the following command:

```sh
./start.sh
```

If that doesn't work try command:
```sh
./start2.sh
```

For additional instructions on how to interact with the substrate node navigate to `./substrate-interact/README.md`.

### Run
You can run the repositories inside differnt folders either inidividually (by following instruction in the individual README.md folders) or by running the command

For installing dependencies on both repositories:
```sh
pnpm i
```

And then run:
```sh
pnpm run dev
```

Now to open up `lastic_frontend` navigate to
```
http://localhost:3000
```

and to open the `substrate_interact` navigate to
```
http://localhost:8000/substrate-front-end-template
```



## Visual Resources

### Flow Chart:

Click on the image below to access the full-sized flow chart:

[Click to visit Flow Chart](https://www.figma.com/file/aFn15lyvti5hqLJBNUDZlU/Lastic-Flow-Chart-%231?type=whiteboard&node-id=0%3A1&t=ZiWNv9gRsH68D5Km-1)

![FLOW CHART](https://github.com/LasticXYZ/LasticUI/assets/30662672/a08dd7b3-bc14-4d51-9689-75bac7895b26)
### Figma UI:

After launching, navigate to Options > Fit Width for the best view.
[Click to visit Figma UI](https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Fproto%2FYzHexLzhb9Q4FPkM19cl1y%2FLastic%3Fpage-id%3D0%253A1%26type%3Ddesign%26node-id%3D203-897%26viewport%3D1012%252C165%252C0.06%26t%3DFBfVL9tIBH4OQJ1A-1%26scaling%3Dmin-zoom%26starting-point-node-id%3D203%253A897%26mode%3Ddesign)

![FIGMA UI](https://github.com/LasticXYZ/LasticUI/assets/30662672/442e1f73-8bd9-48a2-8139-1057ec2dddd1)

## Articles

Articles to check out: 
 - [Unlocking the Future of Blockspace](https://medium.com/lastic-marketplace/unlocking-the-future-of-blockspace-introducing-lastic-9036b9d6637)
 - [The Genesis of Lastic](https://medium.com/lastic-marketplace/the-genesis-of-lastic-a-coretime-marketplace-for-polkadot-75130e40306c)
 - [Simplifying RFC-1: Understanding Agile Coretime for the Polkadot Network](https://medium.com/lastic-marketplace/the-genesis-of-lastic-a-coretime-marketplace-for-polkadot-75130e40306c)
 - [Polkadot 2.0: A New Era of Decentralization](https://medium.com/lastic-marketplace/polkadot-2-0-a-new-era-of-decentralization-d5626a6e63e5)
 - [Unraveling Agile Coretime: Polkadot’s Innovative Resource Allocation](https://medium.com/lastic-marketplace/unraveling-agile-coretime-polkadots-innovative-resource-allocation-2c025d0daa59)




# Lastic Substrate Interact
Lastic Substrate Interact is a user interface designed to work with the Substrate framework. This directory will eventually be merged together with `../static_frontend`. This guide will help you set up and run the project.

## Prerequisites

Before you begin, ensure you have the Substrate node running. To spin up a local Substrate node run the following command:

```sh
../start.sh
```

## Running the Frontend

To set up and run the frontend, execute the following commands:

```sh
# Install the required dependencies
pnpm i

# Start the frontend server
pnpm run dev
```

Once the server is running, you can access the frontend at:  
[http://localhost:8000/substrate-front-end-template](http://localhost:8000/substrate-front-end-template)

## Coretime Chain Setup

Check the guide in the docs.lastic to help you interact with the Coretime chain
 - [installation guide](https://docs.lastic.xyz/substrate-interact/)
 - [interaction instructions](https://docs.lastic.xyz/substrate-interact/interact.html)

### Alternative way (more difficult)
1. Launch the Polkadot.js application.
2. Navigate to **Development > Local node**.
3. Go to **Developer > Extrinsics**.
4. Decode and submit the following hex-encoded calls:

   - Sudo configure: `0x1600460005000000140000001e000000640000000046c323013200002d31010a000000`
   - Start sale: `0x16004604e80300000000000000000000000000001400`
   - Purchase: `0x4605a0860100000000000000000000000000`

 - Reserve: `0x1600460005000000140000001e000000640000000046c323013200002d31010a000000`

## Template Reference

This project is based on the following template:  
[substrate-developer-hub/substrate-front-end-template](https://github.com/substrate-developer-hub/substrate-front-end-template.git)

