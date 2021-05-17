# Provider FaQ

### Contents

- [Setup](#setting-up-a-provider-node)
  - [Linux](#on-linux)
  - [Windows](#on-windows)
  - [macOS](#on-macos)
- [Settings](#change-settings-on-your-node)
  - [Pricing](#pricing)
  - [Allocated Resources](#allocated-resources)
- [Experimental Contributions](#experimental-contributions)
  - [Providing Logs](#providing-logs)
  - [Rewards](#rewards)
- [Payment FaQ](#payment-faq)
  - [Where can I see my earnings](#where-can-i-see-my-earnings)
  - [Can I just put my normal ethereum address into my node](#can-i-just-put-my-normal-ethereum-address-into-my-node)
  - [How much can I earn](#how-much-can-i-earn)
  - [How are payments calculated](#how-are-payments-calculated)
- [General FaQ](#general-faq)
  - [What hardware is needed to get started](#what-hardware-is-needed-to-get-started)
  - [How can I set up multiple nodes](#how-can-i-set-up-multiple-nodes)

## Setting up a provider node

### On Linux
Install the latest stable release by invoking this command:

``curl -sSf https://join.golem.network/dev/as-provider | bash -``
##### Troubles? Refer to [this](https://handbook.golem.network/troubleshooting/provider-troubleshooting) page or join the [discord](https://chat.golem.network).

### On Windows
1. Install VMWare [here](https://www.vmware.com/products/workstation-player.html).
2. Download Ubuntu [18.04 LTS](https://releases.ubuntu.com/18.04/) or [20.04 LTS](https://releases.ubuntu.com/20.04/).
3. Set it up in VMWare - [video guide](https://youtube.com/watch?v=9rUhGWijf9U).
4. Make sure KVM is enabled by following these instructions in VMWare:
> Power off the (virtual) machine > Right click > Settings > Hardware > Processors > Virtualize Intel VT-x/EPT or AMD-V/RVI
5. Power on the machine/create an account/setup it how you want.
6. Open the terminal and enter this command:

``curl -sSf https://join.golem.network/dev/as-provider | bash -``

##### Troubles? Refer to [this](https://handbook.golem.network/troubleshooting/provider-troubleshooting) page or join the [discord](https://chat.golem.network).

### On macOS
Currently not supported

## Change settings on your node

### Pricing
Open a new terminal window and set prices for the seperate commands by invoking these commands:

```css
golemsp settings set --starting-fee <price>
golemsp settings set --env-per-hour <price>
golemsp settings set --cpu-per-hour <price>
```
Then, restart the node with `golemsp stop`, and confirm with `golemsp status` or by locating your node [here](https://golemstats.com/).

### Allocated Resources
Open a new terminal window and set prices for the seperate commands by invoking these commands:

```css
golemsp settings set --node-name <node-name>             
golemsp settings set --cores <num>                       Number of shared CPU cores
golemsp settings set --memory <bytes (like "1.5GiB")>    Size of shared RAM
golemsp settings set --disk <bytes (like "1.5GiB")>      Size of shared disk space
golemsp settings set --account <account>                 Account for payments [env: YA_ACCOUNT=]
golemsp settings set --payment-network <network>         Payment network [env: YA_PAYMENT_NETWORK=]  [default: mainnet]
                                                         [possible values: mainnet, rinkeby]
```
Then, restart the node with `golemsp stop`, and confirm with `golemsp status` or by locating your node [here](https://golemstats.com/).

## Experimental Contributions
Right now, there is a payment bug stopping some transactions to go through. There will always be issues to resolve, and feedback to be given. With that being said, you can help issues get resolved by contributing time, logs, and other node-specific information.

### Providing Logs
##### Use of Experimental Versions
Sometimes, logs are only looked for in releases that are not yet officially released. These are so called Release Candidates, and can be found [here](https://github.com/golemfactory/yagna/releases). 

Installing the one you want is as simple as running this command:

`curl -sSf https://join.golem.network/as-provider | YA_INSTALLER_CORE=pre-rel-vX.X.X-rcX bash -`

where `vX.X.X-rcX` is swapped for something in the lines of `v0.6.6-rc1`.

##### Collecting logs
To start collecting logs, simply start golemsp with this command:

`RUST_LOG=debug,ya_runtime_api=info,ya_runtime_vm=info,ya_payment=trace golemsp run --payment-network mainnet --subnet public-beta`

##### Errors currently sought-after
Current issues being looked for are listed [here](https://github.com/golemfactory/yagna-triage/issues).

If you're unsure on which errors you've found, any logs are greatly appreciated and sorting can be done by somebody else.

##### Sending log files
Once you've found a sought-after error, join the [discord](https://chat.golem.network) and send them privately to `@Phillip#9780` or publicly in `#providers`.

### Rewards
Every month, two users are picked for being helpful for how much feedback they have given on the technology. This, per the [CIP](https://blog.golemproject.net/community-incentives-program/), rewards these users with 1,000 GLM each!

## Payment FaQ

### Where can I see my earnings?
You can see your earnings by entering `golemsp status` when your node is online, or logging in on [zkWallet](https://wallet.zksync.io/).

### Can I just put my normal ethereum address into my node?
Yes and no. You need to make sure you can login to [zkWallet](https://wallet.zksync.io/) with your wallet, but if you can make sure that works then your normal address is fine.

### How much can I earn?
Earnings are generated on a supply & demand basis; there's no sure way to know how much you're going to earn. You can lower price-settings to receive more tasks, you can higher price-settings to get more per task. You can also lower the allocated resources per node to get more nodes out, and also higher the allocated resources to get more heavy tasks.

You can ask around in the [discord](https://chat.golem.network) to see what settings, hardware, and earnings other providers are currently having.

### How are payments calculated?
There are three price variables currently available, and you can see in this chart how they work:
```css
--env-per-hour      Hourly cost for downloading, uploading, and finalizing a result. For a task it is multiplied by time(h).
--cpu-per-hour      Cost of renting 1 core for 1 hour. For a task it is multiplied by time(h) and the amount of allocated cores. It starts when the task is starting to get calculated.
--starting-fee      Base cost of starting a calculation.
```

##### Example
With the settings { --env-per-hour 0.1, --cpu-per-hour 0.1, starting-fee 0.1 } and the task details { 3 minutes total time, 2 minutes computation time } and node details { 4 cores } we can see how the total cost adds up like this:

`(3-2) / 60 * 0.1 + 2 / 60 * 4  * 0.1 + 0.1 = 0.0394433 GLM`

##### Formula
`(totalMinutes - computeMinutes) / 60 * env-per-hour + computeMinutes / 60 * cpu-per-hour * cores + starting-fee = cost`

## General FaQ
### What hardware is needed to get started?
There are no hardware limitations set by Golem, so aslong as you have a processor, a disk of any kind, and also an internet connection you should be good to go!

The only thing is that some requestors might want better hardware than you're providing, but to start your own node you don't need anything fancy at all.

### How can I set up multiple nodes?
On Linux you can setup more nodes by using something like the [scaleable golem provider](https://github.com/cryptobench/scaleable-golem-provider).

On Windows, you can do the same in your VM or simply create more VM instances.

##### Can they be named the same?
Yes. Just make sure that the yagna id's differentiate by running this command:

`yagna id create`
