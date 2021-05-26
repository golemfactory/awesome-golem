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
> Note: this guide and its contents is specific to Golem and its current implementation, Yagna.

## Contents

- [Golem](#golem)
- [Apps](#apps)
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
- [Developer and requestor resources](#developer-and-requestor-resources)
- [Provider resources](#provider-resources)
  - [Monitoring](#monitoring)
  - [Provisioning](#provisioning)
- [Learning resources](#learning-resources)
  - [Presentations and workshop material](#presentations-and-workshop-material)
  - [Unraveling Golem's The Next Milestone blog series](#unraveling-golems-the-next-milestone-blog-series)
  - [GitHub Digest blog series](#github-digest-blog-series)
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
- [Golem Slate](https://github.com/deutschklub/golem-slate) - SLATE is a code pen SPA for writing a requester script to have work computed by the golem network. It utilizes dockerized yagna environments to communicate with the Golem Network in the background. Hosted [here](https://golem-slate.xyz/). **Compatibility: Beta 1**
- [Golem Network Video Transcoder](https://github.com/Doc-Saintly/golem-video) - A sample app that uses golem.network to transcode videos. Please select your transcoding profile and then upload your videos. **Compatibility: Alpha 2**
- [Golem Transcoding requestor](https://github.com/Edhendil/golem-transcoding) - A React + Spring based webapp accepting video files as input and transcoding these files into different formats using Golem. **Compatibility: Alpha 3**
- [Go le' Machin](https://github.com/DEUTSCHKLUB/go-le-m) - Go le' M. is a web based bulk image editor that uses the golem network for computation. It allows users to upload multiple images and apply bulk actions to them. **Compatibility: Alpha 3**

### Docker
- [Golem Requestor Node](https://github.com/DerekJarvis/general-golem) - A dockerized requestor environment. You can just pass in the py script  (example uses the blender demo) and it sets up the daemon and runs it. **Compatibility: Alpha 3**

### Testing
- [Golem Test Harness (Goth)](https://github.com/golemfactory/goth) - A tool with the purpose of speeding up your development process and making it more enjoyable for Golem app creators ([intro+demo video](https://youtu.be/HP6VVBUdkm8)). **Compatibility: Beta 1**
- [Golem-afl](https://github.com/sladecek/golem-afl) - Golem-afl is an experimental test-fuzzing framework for Golem. Assists in finding security holes. **Compatibility: Beta 1**
- [Golem Cargo Test](https://github.com/sladecek/golem_cargo_test) - Golem Cargo Test is an adaptive distributed test executor for rust projects running on the Golem network. **Compatibility: Alpha 3**
- [Golem CI](https://github.com/hhio618/golem-ci) - Decentralized Task pipeline on top of the Golem Network. **Compatibility: Alpha 3**

### Games
- [Chess on Golem](https://github.com/broadcastmonkey/ChessOnGolem) - A react frontend for the 2 AI's playing against each other through the Golem backend, that computes each others next move. **Compatibility: Beta 1**
- [Golem Sudoku](https://github.com/Dodecane/golem-sudoku) - Game of Sudoku with size variants, powered by Golem. **Compatibility: Alpha 3**
- [HSOG-requester](https://github.com/ChrisHelmsC/hsog-requestor) - HearthStone On Golem helps the HearthStone community in the design and building of decks by running a large number of simulated games on the Golem Network. **Compatibility: Beta 1**

### Data Analysis
- [Flan](https://github.com/nestorbonilla/flan) - A tool for entrepreneurs that provide customized analysis of millions of worldwide trade value records giving them a bold guideline about what sectors they would need to take more attention to. All computed on top of the Golem Network. **Compatibility: Alpha 3**
- [Golem Lorenz-attractor](https://github.com/hhio618/golem-lorenz-attractor) - The Lorenz Equations are a system of three coupled, first-order, nonlinear differential equations which describe the trajectory of a particle through time. **Compatibility: Alpha 2**
- [Golem Geomandel](https://github.com/Edhendil/golem-geomandel) - Geomandel requestor is a python script for generating sequences of Mandelbrot images centered on a single point and with zoom increasing in each image ([example](https://youtu.be/vKH7x2SrkEo)). **Compatibility: Alpha 2**
- [Golem COVID](https://github.com/iRhonin/golem-covid) - Grabs a parameter from data/owid-covid-data.csv file (like new_cases_per_million) and plot every day data on the world map. After all images generated (in outputs), it will gather them and create a gif ([example](https://i.imgur.com/0wtVDgx.mp4)). **Compatibility: Alpha 2**
- [Golem Parallel Matplotlib](https://github.com/CoeJoder/golem-parallel-matplotlib) - Various statistical analyses are performed on circadian rhythm measurements in human test subjects. **Compatibility: Alpha 2**

### Data Simulation
- [cadCAD Golem](https://github.com/rogervs/cadcadgolem) - A package wrapper for cadCAD to dispatch the simulation workload to multiple Golem nodes. Supports Jupyter Notebook. **Compatibility: Alpha 3**
- [Golem Array](https://github.com/johngrantuk/golem-array) - Antenna Array Design & Simulation - Powered By Golem. **Compatibility: Alpha 3**
- [Limit visualization](https://github.com/vporton/limit-visualization) - Plot graphs on Golem with various limits.
[Discontinous example](https://i.imgur.com/mxRDe5G.gif). **Compatibility: Alpha 2**
- [golemGraphWavePair](https://github.com/smiley1983/golemGraphWavePair) - Use the Golem Network to generate graph frames, then combine them into an animation. **Compatibility: Alpha 2**
- [Golemized strong-gravitational-lense](https://github.com/rezahsnz/golemized-strong-gravitational-lense) - A simple distributed computing hack that tries to simulate some physical phenomena called gravitional lensing and is based on the work of Prof. Adam Bolton. **Compatibility: Alpha 2**

### Data Optimization
- [Golem or-tools](https://github.com/Doc-Saintly/golem-ortools) - Uses the or-tools Constraint Programming library to solve problems on the Golem Network. **Compatibility: Alpha 1**
- [No more COFUD](https://github.com/DEUTSCHKLUB/no-more-COFUD) - A tool that calculates how to fit the most people into a space while keeping 2 meters distance between each other. **Compatibility: Alpha 3**

### Finance
- [ZKSync .csv export](https://github.com/blue-notes-robot/zksync-csv-export) - A tool that scrapes ZKSync to generate financial data in a .csv file.

### Machine Learning
- [DeML-Golem](https://github.com/anshuman73/DeML-Golem) - A Proof Of Concept of Decentralised Machine Learning. It uses Federated Learning to combine the sub-step models it trains on different provider nodes into a full fleged model. **Compatibility: Alpha 3**

### Deep Learning
- [mlg](https://github.com/rezahsnz/mlg) - CNN predict services on top of Golem. A deep learning application that distributes popular CNNs pre-trained with ImageNet datasets across Golem provider nodes. **Compatibility: Beta 1**
- [Deepart Golem](https://github.com/echinocacti/deepart_golem) - Make art using distributed computing, running a tensorflow app and uploading your content and style picture and make the golem network process your image, doing beautiful art with style transfer and deeplearning. **Compatibility: Alpha 3 (PoC)**

### RNG
- [Gandom](https://github.com/rezahsnz/gandom) - A tool that tries to extract random streams from providers on the Golem Network. It supports two PRNGs, one based on [Chaos machines](https://github.com/maciejczyzewski/libchaos) and the other that makes use of [Sodium](https://libsodium.org/). **Compatibility: Alpha 3**

### Password Cracking
- [Golem-JTR](https://github.com/hhio618/golem-jtr) - Run John The Ripper on Golem Nodes to recover a password. **Compatibility: Alpha 2**
- [Yacat](https://handbook.golem.network/requestor-tutorials/create-your-own-application-on-golem/the-steps-to-do) - Hashcat password-recovery example, this tutorial is designed to inspire you to create your own Golem applications, we will explain all the needed details of Golem application implementation. **Compatibility: Alpha 3**

### DeFi

- [Golem Staking Pool incentivize system for GLM holders](https://github.com/masaun/GLM-stake-pool) - Is a smart contract in order to provide the opportunity of yield farming for Golem's GLM token holders. (By staking uniswap-LP tokens that is a pair between GLM and ETH into the stake pool). **Compatibility: Alpha 3**
- [Magic-doll](https://github.com/bakaoh/magic-doll) - Sumer is a DeFi application that people may delegate their Splinterland card to earn passive income. Its core is [Kyle](https://github.com/bakaoh/magic-doll/tree/master/kyle), a Golem application that do all the computation to pick the best team to play for each match. **Compatibility: Alpha 3**

### User Interfaces

- [Golem UI](https://github.com/shri4net/golem-hackathon-2020) - A electron user interface for the Golem Network. **Compatibility: Alpha 3**

### Miscellaneous

- [gvm-vim](https://github.com/canokaue/gvm-vim) - A golemized docker image for compiling the most loved vim editor. **Compatibility: Alpha 2**
- [YaJSapi fork with greeting example](https://github.com/rezahsnz/yajsapi) - A simple Node.js requestor app that greets you. It writes some important message to a file and then downloads it for you, the basic eskeleton of a requestor app. Look in `examples/greetings`. **Compatibility: Alpha 3**
- [Golem Image Sharpening](https://github.com/visualNext/golem) - Using golem to sharpen your images. **Compatibility: Alpha 3**

## Developer and requestor resources

- [Yagna handbook](https://handbook.golem.network/) - Handbook for the Golem, implementation name, Yagna.
- [Releases List](https://github.com/golemfactory/yagna/releases) - GitHub releases of Yagna.
- [Requestor flash tutorial](https://handbook.golem.network/requestor-tutorials/flash-tutorial-of-requestor-development) - Get started quick and create your first tasks/request on Golem.
- [Yagna tag on Stack Overflow](https://stackoverflow.com/questions/tagged/yagna) - If you have an interesting question you'd like answered.
- [Breakdown of blender.js](https://docs.google.com/document/d/e/2PACX-1vRONc0RRaqImJumYQ3SmILtLo4jiCYgtE0AO3JfpMy0b0-BjAU8TvlIHdtbrs5cDrMbuPFv7khE47MO/pub) - JS guide to see how to run a task on Golem.

## Provider resources

- [Provider Tutorial](https://handbook.golem.network/provider-tutorials/provider-tutorial) - Get started as a Provider on Golem Network using the handbook.
- [Provider FAQ](https://github.com/figurestudios/community-golem-docs/blob/main/providing/provider-faq.md) - Community curated list of commonly asked questions and answers.

### Monitoring

- [Golem Provider dashboard](https://github.com/vciancio/golem-dashboard) - A ReactJS dashboard made to quickly gather status from your provider nodes without havingn to SSH into them. **Compatibility: Beta 1**
- [Golem Provider dashboard backend / GolemBar](https://github.com/vciancio/golem-node-server) - The flask backend that collects the data from the provider that's then used with the dashboard project above. **Compatibility: Beta 1**

### Provisioning

- [WSL](https://github.com/r34x/WSL) - Allows Windows users to run Golem within Windows Subsystem for Linux. Removing the requirement of Windows users needing to use a Virtual Machine. **Compatibility: Beta 1**
- [Golem Provider Terraform](https://github.com/nemani/golem-provider-terraform) - A terraform script to automatically deploy a Golem Provider on a cloud provider and setup monitoring using prometheus. **Compatibility: Beta 1**
- [Automatic Golem](https://github.com/r34x/Automatic-Golem) - A way to setup a Golem Provider with simple instructions and logs guiding you through the process. **Compatibility: Beta 1**
- [Golem Provider Node](https://github.com/alexandre-abrioux/golem-node) - A Docker version of a node to help you get started running as a provider in a Docker container quick. Before you start please check that `ARG YA_CORE_VERSION`, `ARG YA_WASI_VERSION` and `ARG YA_VM_VERSION` in the [Dockerfile](https://github.com/alexandre-abrioux/golem-node/blob/master/docker/Dockerfile) are the correct versions. **Compatibility: Beta 1**
- [Golem Provider node](https://github.com/blue-notes-robot/golem-node) - A fork of Alxexandre-abrioux project above that allows to dynamically generate config files from ENV variables and specify how many replicas you'd like to spawn. **Compatibility: Beta 1**

## Learning resources

### Presentations and workshop material

- [Golem: Architecture, SDKs and tips with Jakub Mazurek at 0xHack](https://youtu.be/1UoZWC9XI2g) - A live workshop diving into how any developer with Python or JS coding experience can start build applications running on Golem.
- [Golem: Growing an ecosystem the Golem way with María Paula Fernández at 0xHack](https://youtu.be/FmrdyU90NVE) - High-level overview and introduction to Golem as a project.
- [Golem Workshop at H3LLO Decentralization](https://gist.github.com/zakaprov/5366bffa49b3c116748bf9b5b73c602c) - A list of resources containing a live-coding hackathon workshop and relevant resources to help developers understand and requesting on Golem.
- [Mainnet Requestor quickstart Walk-through](https://youtu.be/GcdTq3i_wdY) - A video walk-through of the requestor quick-start handbook guide to get a request on Golem Network testnet and then mainnet using the Yagna Python API.
- [Mainnet Provider quickstart Walk-through](https://youtu.be/RITdKtEOV_E) - A video walk-through of the provider handbook guide to start sharing computational resources the Golem Network.

### Unraveling Golem's The Next Milestone blog series

- [Unraveling Golem's The Next Milestone](https://blog.golemproject.net/next-milestone) - An introduction to the Yagna implementation.
- [Unraveling Golem's The Next Milestone, Part II](https://blog.golemproject.net/next-milestone-part-ii/) - Fundamental architectural concepts which constitute the foundations of the new implemenation of Golem, Yagna.
- [Unraveling Golem's The Next Milestone, Part III](https://blog.golemproject.net/next-milestone-part-iii/) - The elements of Golem's reference architecture, and illustrates how they interact to form a working ecosystem, being the Golem Network.

### GitHub Digest blog series

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
- [Golem Network Discussion Group](https://t.me/GolemProject) - Community driven Telegram channel.
