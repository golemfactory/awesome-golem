</p>
<p align="center">
    <a href="https://twitter.com/golemproject" alt="Twitter">
        <img src="https://img.shields.io/twitter/follow/golemproject?style=social" />
    </a>
    <a href="https://discord.gg/y29dtcM" alt="Discord">
        <img src="https://img.shields.io/discord/684703559954333727?logo=discord" />
    </a>  
    <a href="https://reddit.com/GolemProject" alt="Reddit">
        <img src="https://img.shields.io/reddit/subreddit-subscribers/GolemProject?style=social" />
    </a>
</p>

# Awesome Golem [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Welcome to **Awesome Golem**, a community-curated list of resources, links, projects, tools and apps on Golem!
> Note: this guide and its contents is specific to Golem and it's current implementation, Yagna.

## Contents

- [Golem](#golem)
- [Apps](#apps)
  - [Monitoring](#monitoring)
  - [Provisioning](#provisioning)
  - [Docker](#docker)
  - [Testing](#testing)
  - [Games](#games)
  - [Data Analysis](#data-analysis)
  - [Data Simulation](#data-simulation)
  - [Data Optimization](#data-optimization)
  - [Finance](#finance)
  - [Machine Learning](#machine-learning)
  - [Deep Learning](#deep-learning)
  - [RNG](#rng)
  - [Password Cracking](#password-cracking)
  - [DeFi](#defi)
  - [User Interfaces](#user-interfaces)
  - [Miscellaneous](#miscellaneous)
- [Developer Resources](#developer-resources)
  - [Docs and Releases](#docs-and-releases)
  - [Running a node on Golem](#running-a-node-on-golem)
  - [Testnet GLM and Ether](#testnet-glm-and-ether)
- [Learning Resources](#-learning-resources)
  - [Unraveling Golem's The Next Milestone series](#unraveling-golems-the-next-milestone-series)
  - [Videos and presentations](#videos-and-presentations)
  - [GitHub Digest](#github-digest)
- [Community](#community)

## Golem

- [Golem.Network Website](https://golem.network/) - The official Golem Network website.
- [Golem Factory GitHub](https://github.com/golemfactory) - Where you can find the open source code of all things Golem!
- [Yagna GitHub](https://github.com/golemfactory/yagna) - The implementation of Golem [![Watch on GitHub](https://img.shields.io/github/watchers/golemfactory/yagna.svg?style=social)](https://github.com/golemfactory/yagna/watchers)
[![Star on GitHub](https://img.shields.io/github/stars/golemfactory/yagna.svg?style=social)](https://github.com/golemfactory/yagna/stargazers)
- [Golem Community Chat](https://chat.golem.network/) - Join the community and team open discussion on Discord.
- [Reddit](https://reddit.com/r/GolemProject) - Golem Network discussion on the Reddit platform.
- [Twitter](https://twitter.com/golemproject) - The Golem Project Twitter.
- [Blog](http://blog.golemproject.net/) - The official blog where you can find the most reliable information on announcements, summaries and updates.

## Apps
- [Golem Slate](https://github.com/deutschklub/golem-slate) - SLATE is a code pen SPA for writing a requester script to have work computed by the golem network. It utilizes dockerized yagna environments to communicate with the Golem Network in the background. Hosted [here](https://golem-slate.xyz/).
    * **Compatibility: Beta 1**
- [Golem Network Video Transcoder](https://github.com/Doc-Saintly/golem-video) - This is sample app that uses golem.network to transcode videos. Please select your transcoding profile and then upload your videos.
    * **Compatibility: Alpha 2**
- [Golem Transcoding requestor](https://github.com/Edhendil/golem-transcoding) - A React + Spring based webapp accepting video files as input and transcoding these files into different formats using Golem.
    * **Compatibility: Alpha 3**
- [Go le' Machin](https://github.com/DEUTSCHKLUB/go-le-m) - Go le' M. is a web based bulk image editor that uses the golem network for computation. It allows users to upload multiple images and apply bulk actions to them.
    * **Compatibility: Alpha 3**

## Monitoring
- [Golem Provider Terraform](https://github.com/nemani/golem-provider-terraform) - A terraform script to automatically deploy a Golem Provider on a cloud provider and setup monitoring using prometheus.
    * **Compatibility: Beta 1**
- [Golem Provider dashboard](https://github.com/vciancio/golem-dashboard) - A ReactJS dashboard made to quickly gather status from your provider nodes without havingn to SSH into them.
    * **Compatibility: Beta 1**
- [Golem Provider dashboard backend / GolemBar](https://github.com/vciancio/golem-node-server) - The flask backend that collects the data from the provider that's then used with the dashboard project above.
    * **Compatibility: Beta 1**

## Provisioning
- [WSL](https://github.com/r34x/WSL) - Allows Windows users to run Golem within Windows Subsystem for Linux. Removing the requirement of Windows users needing to use a Virtual Machine.
    * **Compatibility: Beta 1**
- [Golem Provider Terraform](https://github.com/nemani/golem-provider-terraform) - A terraform script to automatically deploy a Golem Provider on a cloud provider and setup monitoring using prometheus.
    * **Compatibility: Beta 1**
- [Automatic Golem](https://github.com/r34x/Automatic-Golem) - A way to setup a Golem Provider with simple instructions and logs guiding you through the process.
    * **Compatibility: Beta 1**

## Docker
- [Golem Provider Node](https://github.com/alexandre-abrioux/golem-node) - A Docker version of a node to help you get started running as a provider in a Docker container quick. Before you start please check that `ARG YA_CORE_VERSION`, `ARG YA_WASI_VERSION` and `ARG YA_VM_VERSION` in the [Dockerfile](https://github.com/alexandre-abrioux/golem-node/blob/master/docker/Dockerfile) are the correct versions.
    * **Compatibility: Beta 1**
- [Golem Provider node](https://github.com/blue-notes-robot/golem-node) - A fork of Alxexandre-abrioux project that allows to dynamically generate config files from ENV variables and specify how many replicas you'd like to spawn.
    * **Compatibility: Beta 1**
- [Golem Requestor Node](https://github.com/DerekJarvis/general-golem) - A dockerized requestor environment. You can just pass in the py script  (example uses the blender demo) and it sets up the daemon and runs it.
    * **Compatibility: Alpha 3**

## Testing
- [Golem Test Harness (Goth)](https://github.com/golemfactory/goth) - A tool with the purpose of speeding up your development process and making it more enjoyable for Golem app creators ([intro+demo video](https://youtu.be/HP6VVBUdkm8)).
    * **Compatibility: Beta 1**
- [Golem-afl](https://github.com/sladecek/golem-afl) - Golem-afl is an experimental test-fuzzing framework for Golem. This can help you find security holes in your software, such as a Stack Overflow.
    * **Compatibility: Beta 1**
- [Golem Cargo Test](https://github.com/sladecek/golem_cargo_test) - Golem Cargo Test is an adaptive distributed test executor for rust projects running on the Golem network.
    * **Compatibility: Alpha 3**
- [Golem CI](https://github.com/hhio618/golem-ci) - Decentralized Task pipeline on top of the Golem Network.
    * **Compatibility: Alpha 3**

## Games
- [Chess on Golem](https://github.com/broadcastmonkey/ChessOnGolem) - A react frontend for the 2 AI's playing against each other through the Golem backend, that computes each others next move.
    * **Compatibility: Beta 1**
- [Golem Sudoku](https://github.com/Dodecane/golem-sudoku) - Game of Sudoku with size variants, powered by Golem.
    * **Compatibility: Alpha 3**
- [HSOG-requester](https://github.com/ChrisHelmsC/hsog-requestor) - HearthStone On Golem helps the HearthStone community in the design and building of decks by running a large number of simulated games on the Golem Network.
    * **Compatibility: Beta 1**

## Data Analysis
- [Flan](https://github.com/nestorbonilla/flan) - A tool for entrepreneurs that provide customized analysis of millions of worldwide trade value records giving them a bold guideline about what sectors they would need to take more attention to. All computed on top of the Golem Network.
    * **Compatibility: Alpha 3**
- [Golem Lorenz-attractor](https://github.com/hhio618/golem-lorenz-attractor) - The Lorenz Equations are a system of three coupled, first-order, nonlinear differential equations which describe the trajectory of a particle through time.
    * **Compatibility: Alpha 2**
- [Golem Geomandel](https://github.com/Edhendil/golem-geomandel) - Geomandel requestor is a python script for generating sequences of Mandelbrot images centered on a single point and with zoom increasing in each image ([example](https://youtu.be/vKH7x2SrkEo)).
    * **Compatibility: Alpha 2**
- [Golem COVID](https://github.com/iRhonin/golem-covid) - This program get a parameter from data/owid-covid-data.csv file (like new_cases_per_million) and plot every day data on the world map. After all images generated (in outputs), it will gather them and create a gif ([example](https://i.imgur.com/0wtVDgx.mp4)).
    * **Compatibility: Alpha 2**
- [Golem Parallel Matplotlib](https://github.com/CoeJoder/golem-parallel-matplotlib) - Various statistical analyses are performed on circadian rhythm measurements in human test subjects.
    * **Compatibility: Alpha 2**

## Data Simulation
- [cadCAD Golem](https://github.com/rogervs/cadcadgolem) - This package is a wrapper for cadCAD to dispatch the simulation workload to multiple Golem nodes. Supports Jupyter Notebook.
    * **Compatibility: Alpha 3**
- [Golem Array](https://github.com/johngrantuk/golem-array) - Antenna Array Design & Simulation - Powered By Golem.
    * **Compatibility: Alpha 3**
- [Limit visualization](https://github.com/vporton/limit-visualization) - Plot graphs on Golem with various limits.
[Discontinous example](https://i.imgur.com/mxRDe5G.gif).
    * **Compatibility: Alpha 2**
- [golemGraphWavePair](https://github.com/smiley1983/golemGraphWavePair) - Use the Golem Network to generate graph frames, then combine them into an animation.
    * **Compatibility: Alpha 2**
- [Golemized strong-gravitational-lense](https://github.com/rezahsnz/golemized-strong-gravitational-lense) - A simple distributed computing hack that tries to simulate some physical phenomena called gravitional lensing and is based on the work of Prof. Adam Bolton.
    * **Compatibility: Alpha 2**

## Data Optimization
- [Golem or-tools](https://github.com/Doc-Saintly/golem-ortools) - Uses the or-tools Constraint Programming library to solve problems on the golem network.
    * **Compatibility: Alpha 1**
- [No more COFUD](https://github.com/DEUTSCHKLUB/no-more-COFUD) - A tool that calculates how to fit the most people into a space while keeping 2 meters distance between each other.
    * **Compatibility: Alpha 3**

## Finance
- [ZKSync .csv export](https://github.com/blue-notes-robot/zksync-csv-export) - A tool that scrapes ZKSync to generate financial data in a .csv file.

## Machine Learning
- [DeML-Golem](https://github.com/anshuman73/DeML-Golem) - A Proof Of Concept of Decentralised Machine Learning. It uses Federated Learning to combine the sub-step models it trains on different provider nodes into a full fleged model.
    * **Compatibility: Alpha 3**

## Deep Learning
- [mlg](https://github.com/rezahsnz/mlg) - CNN predict services on top of Golem. This deep learning application distributes popular CNNs pre-trained with ImageNet datasets across Golem provider nodes.
    * **Compatibility: Beta 1**
- [Deepart Golem](https://github.com/echinocacti/deepart_golem) - Make art using distributed computing, running a tensorflow app and uploading your content and style picture and make the golem network process your image, doing beautiful art with style transfer and deeplearning. (POC)
    * **Compatibility: Alpha 3 (PoC)**

## RNG
- [Gandom](https://github.com/rezahsnz/gandom) - A tool that tries to extract random streams from providers on the Golem Network. It supports two PRNGs, one based on [Chaos machines](https://github.com/maciejczyzewski/libchaos) and the other that makes use of [Sodium](https://libsodium.org/).
    * **Compatibility: Alpha 3**

## Password Cracking
- [Golem-JTR](https://github.com/hhio618/golem-jtr) - Run John The Ripper on Golem Nodes to recover a password.
    * **Compatibility: Alpha 2**
- [Yacat](https://handbook.golem.network/requestor-tutorials/create-your-own-application-on-golem/the-steps-to-do) - Hashcat password-recovery example, this tutorial is designed to inspire you to create your own Golem applications, we will explain all the needed details of Golem application implementation.
    * **Compatibility: Alpha 3**

## DeFi

- [Golem Staking Pool incentivize system for GLM holders](https://github.com/masaun/GLM-stake-pool) - Is a smart contract in order to provide the opportunity of yield farming for Golem's GLM token holders. (By staking uniswap-LP tokens that is a pair between GLM and ETH into the stake pool).
    * **Compatibility: Alpha 3**
- [Magic-doll](https://github.com/bakaoh/magic-doll) - Sumer is a DeFi application that people may delegate their Splinterland card to earn passive income. It's core is [Kyle](https://github.com/bakaoh/magic-doll/tree/master/kyle), a Golem application that do all the computation to pick the best team to play for each match.
    * **Compatibility: Alpha 3**

## User Interfaces

- [Golem UI](https://github.com/shri4net/golem-hackathon-2020) - A electron user interface for the Golem Network.
    * **Compatibility: Alpha 3**

## Miscellaneous

- [gvm-vim](https://github.com/canokaue/gvm-vim) - A golemized docker image for compiling the most loved vim editor.
    * **Compatibility: Alpha 2**
- [YaJSapi fork with greeting example](https://github.com/rezahsnz/yajsapi) - A simple Node.js requestor app that greets you. It writes some important message to a file and then downloads it for you, the basic eskeleton of a requestor app. Look in `examples/greetings`.
    * **Compatibility: Alpha 3**
- [Golem Image Sharpening](https://github.com/visualNext/golem) - Using golem to sharpen your images.
    * **Compatibility: Alpha 3**

## Developer Resources

### Docs and releases

- [Yagna handbook](https://handbook.golem.network/) - Handbook for the Golem, implementation name, Yagna.
- [Releases List](https://github.com/golemfactory/yagna/releases) - GitHub releases of Yagna.

## Running a node on Golem
> Golem went on mainnet March 11th 2021.

### Requestor
Get started quick and make your first request with the [Requestor flash tutorial](https://handbook.golem.network/requestor-tutorials/flash-tutorial-of-requestor-development).

- If you have an interesting question you'd like answered, the Golem development team monitors the [Yagna tag on Stack Overflow](https://stackoverflow.com/questions/tagged/yagna).
- If you're a JS developer, you can take a look at the community-made [breakdown of blender.js](https://docs.google.com/document/d/e/2PACX-1vRONc0RRaqImJumYQ3SmILtLo4jiCYgtE0AO3JfpMy0b0-BjAU8TvlIHdtbrs5cDrMbuPFv7khE47MO/pub) to see how to run a task on Golem.

### Provider
Follow the [Provider section](https://handbook.golem.network/provider-tutorials/provider-tutorial) of the handbook.

Go through the [FaQ](https://github.com/figurestudios/community-golem-docs/blob/main/providing/provider-faq.md) for commonly asked questions.

## Testnet GLM and Ether

To receive some tGLM on [rinkeby zksync](https://rinkeby.zkscan.io/) you can run `yagna payment fund` followed by `yagna payment init --sender`. You no longer need test ETH to run your task golem, tx fees on zksync are paid in tGLM too.

In case there is an issue with zksync, you can use the old erc20 payment driver:
- Get some funds with `yagna payment fund --driver erc20`.
- Enable sending for this account with `yagna payment init --sender --driver erc20`.
- Run your task ( f.e. python blender examplpe ) with `--driver erc20` argument.

If for any reason the faucet was unsuccessful, grab some testnet Ether via the [Rinkeby faucet](https://faucet.rinkeby.io/), send it to your node address (can be found with `yagna app-key list`, starts with "0x") and run the payment steps again `yagna payment fund --driver erc20` followed by `yagna payment init --sender --driver erc20`.

If you have the MetaMask browser extension installed you can also try the [MetaMask faucets](https://faucet.metamask.io). Change to Rinkeby test network by clicking at the top on 'Main Ethereum Network' and select Rinkeby.

## 📝 Learning Resources

### Unraveling Golem's The Next Milestone series

- [Unraveling Golem's The Next Milestone](https://blog.golemproject.net/next-milestone)
- [Unraveling Golem's The Next Milestone, Part II](https://blog.golemproject.net/next-milestone-part-ii/)
- [Unraveling Golem's The Next Milestone, Part III](https://blog.golemproject.net/next-milestone-part-iii/)


### Videos and presentations

- [Mainnet Requestor quickstart Walk-through](https://youtu.be/GcdTq3i_wdY) - Mattias.
- [Golem Workshop at H3LLO Decentralization](https://youtu.be/gWRqu7IvYfk) - Kuba M.
- [Mainnet Provider quickstart Walk-through](https://youtu.be/RITdKtEOV_E) - Mattias.
- [Golem x Gitcoin - Hackathon 101 (December 2020) + Alpha 3 limitations](https://www.youtube.com/watch?v=P6D5ziYcDy0&t=481s)
- [Golem Loves Layer 2 presentations and panel](https://youtu.be/B8Qu-Nofbaw) - Kuba & Mikolaj (Golem) + Panel: Jay Zhou (Loopring Protocol), Kasima Tharnpipitchai (OMG Network), Alex Gluchowski (MatterLabs), Kelvin Fichter (Optimism), Kuba Kucharski (Golem).
- [New Golem - Alpha 2 Release - Quick intro](https://youtu.be/TenOjOql5vA) - Kuba.
- [EDCON - Building New Golem: Where We're at and Where We're Heading](https://www.youtube.com/watch?v=FVzn1G9wtUg&feature=youtu.be&t=901) - Kuba.
- [ReadyLayerOne - A Golem (R)evolution](https://youtu.be/s9WdFqLyLFo) - Piotr Janiuk.


### GitHub Digest

- [Golem GitHub Digest #1](https://blog.golemproject.net/golem-github-digest-1/) - Understanding the Golem Repositories.
- [Golem GitHub Digest #2](https://blog.golemproject.net/golem-github-digest-2/) - Diving into the Golem Repositories.
- [Golem GitHub Digest #3](https://blog.golemproject.net/golem-github-digest-3/) - Diving into Pull Requests of the Golem repositories.
- [Golem GitHub Digest #4](https://blog.golemproject.net/golem-github-digest-4/) - Diving into latest releases in the Golem repositories.
- [Golem GitHub Digest #5](https://blog.golemproject.net/golem-github-digest-5/) - Diving into the Golem alpha testnet.
- [Golem GitHub Digest #6](https://blog.golemproject.net/golem-github-digest-6/) - SGX proof-of-concept for Golem.
- [Golem GitHub Digest #7](https://blog.golemproject.net/golem-github-digest-7/) - Decentralization of the Golem marketplace.
- [Golem GitHub Digest #8](https://blog.golemproject.net/golem-github-digest-8/) - Awesome Golem and next steps to Alpha 3.
- [Golem GitHub Digest #9](https://blog.golemproject.net/golem-github-digest-9/) - AMD provider support, network metrics and improved proposal handling.
- [Golem GitHub Digest #10](https://blog.golemproject.net/golem-github-digest-10/) - Improvements from community feedback.
- [Golem GitHub Digest #11](https://blog.golemproject.net/golem-github-digest-11/) - Easy log collection.
- [Golem GitHub Digest #12](https://blog.golemproject.net/golem-github-digest-12/) - We are on MAINNET and gathering feedback.
- [Golem GitHub Digest #13](https://blog.golemproject.net/golem-github-digest-13/) - Progressing faster with the help of the Golem community.


## Community

- [Golem Community GLM Rewards Program](https://blog.golemproject.net/community-incentives-program/) - Participate in the community and get rewarded for it in GLM!
- Community driven [Golem Network Discussion Group](https://t.me/GolemProject) Telegram channel.
