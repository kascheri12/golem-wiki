### Jump to a Section:

* [How Golem Works](https://github.com/golemfactory/golem/wiki/FAQ#golem-technology)
* [Business Model](https://github.com/golemfactory/golem/wiki/FAQ#golem-business-model)
* [Safety and Security](https://github.com/golemfactory/golem/wiki/FAQ#safety-and-security)
* [Using Golem (Troubleshooting)](https://github.com/golemfactory/golem/wiki/FAQ#using-golem)
   - [What to do if Something Goes Wrong](https://github.com/golemfactory/golem/wiki/FAQ#what-do-i-do-if-something-goes-wrong)
   - [Docker Errors](https://github.com/golemfactory/golem/wiki/FAQ#docker-errors)
* [Golem vs. Others](https://github.com/golemfactory/golem/wiki/FAQ#comparing-golem-to-other-services)
* [Golem Token](https://github.com/golemfactory/golem/wiki/FAQ#golem-token)
* [Read our Whitepaper (ctrl + click to open in new tab)](https://golem.network/doc/Golemwhitepaper.pdf)

# How and why Golem will change the world (or at least the Internet)
### What is Golem?

Golem connects computers in a peer-to-peer network, enabling both application owners and individual users ("**requestors**") to rent resources of other users’ ("**providers**") machines. These resources can be used to complete tasks requiring any amount of computation time and capacity. Today, such resources are supplied by centralized cloud providers which, are constrained by closed networks, proprietary payment systems, and hard-coded provisioning operations. Also core to Golem’s built-in feature set is a dedicated Ethereum-based transaction system, which enables direct payments between requestors, providers, and software developers.

The function of Golem as the backbone of a decentralized market for computing power can be considered both Infrastructure-as-a-Service (IaaS), as well as Platform-as-a-Service (PaaS). However, Golem reveals its true potential by adding dedicated software integrations to the equation. Any interested party is free to create and deploy software to the Golem network by publishing it to the Application Registry. Together with the Transaction Framework, developers can also extend and customize the payment mechanism resulting in unique mechanisms for monetizing software.

### Who can use Golem and why?

The short answer is that Golem can be used (and should be used) by everyone who owns a computer.  

The long answer is that how you use Golem depends on what you use your computer for.

If you are an average user, you are likely to be a provider. Golem gives your computer work to do when it is not being used then you earn money for tasks completed. The money comes from requestors, paying providers for using their machines.

If for any purpose you need more computing time than you have on your own machine - because you are a CGI professional, scientist, financial market tycoon, cryptocurrency miner or anyone else fitting in the wide range of Golem’s use cases - then you can use Golem as a requestor. You submit your task to the network, it is completed by providers and you pay for their machines' time. Additionally, if the task you want to perform needs proprietary software - you can get it through the App Registry.

If you are an owner of an open source or proprietary software (like a rendering engine, analytical packages, trading robots, specialised scientific packages, or a Dapp), you may want to use Golem as a distribution channel and (if you opt to charge for use) as a marketplace. 


### What is the current state of the project and the way ahead?

The alpha version was launched in August 2016, with the code available for review. The alpha version (codename Brass Golem) will be focused on CGI rendering in Blender (blender.org) and will be our MVP, although we expect it will be useful for blender users and once we move to release version will have a group of dedicated users.

You can follow our Brass Golem KanBan here: https://trello.com/b/YL1qZ2pZ/brass-kanban

* [Brass Golem](https://github.com/imapp-pl/golem/wiki/Roadmap#brass-golem) 

> ...these are created to fulfill one goal

Brass Golem is where we are at the moment with our MVP, in alpha testing now. This current version of Golem is only focused on rendering in Blender and LuxRender, and although it will be useful to CGI artists, we consider CGI rendering to be one use case among many, and also a training ground. Brass Golem should be frozen within 6 months after the end of our crowdfunding period and a full battery of tests. Even though we do not expect that Blender CGI rendering will create enough turnover to justify all the work we have put into the project, this will be the first decentralized computation market.

* [Clay Golem](https://github.com/imapp-pl/golem/wiki/Roadmap#clay-golem) 

> There is a chance (...) that a Clay Golem will be possessed by a chaotic evil spirit. 

Clay Golem is a big leap from the Brass milestone. Clay introduces the Task API and the Application Registry, which together are going to make Golem a multi-purpose, generalized distributed computation solution. Developers now have the means to integrate with Golem. This advance, however, may come at the cost of compromised stability and security, so this version should be considered an experiment for early adopters and tech enthusiasts. Prototypes, new ideas and solutions will be built on Clay.

* [Stone Golem](https://github.com/imapp-pl/golem/wiki/Roadmap#stone-golem) 

> Stone Golems do not revoke their creators control like (...) Clay Golems.

Stone Golem will add more security and stability, but also enhance the functionalities implemented in Clay. An advanced version of the Task API will be introduced. The Application Registry will be complemented by the Certification Mechanism that will create a community-driven trust network for applications. Also, the Transaction Framework will create an environment that will allow Golem to be used in a SaaS model.

* [Iron Golem](https://github.com/imapp-pl/golem/wiki/Roadmap#iron-golem)

> Iron Golems are made of iron and are among the strongest type of Golem. They never revoke the control of the wizard that created them.

Iron is a deeply tested Golem that gives more freedom to developers, allowing them to create applications that use an Internet connection or applications that run outside the sandbox. Of course, the decision to accept higher-risk applications will still belong to the providers renting their computing power. Iron Golem should be robust, highly resistant to attacks, stable and scalable. Iron will also introduce various tools for developers that will make application creation far easier. Finally, the Golem Standard Library will be implemented.

### How Golem will help to build a new Internet of tomorrow?

We believe, that in the future, the Internet will be a truly decentralized network, enabling users to securely and directly exchange content, without middlemen. Accordingly, Golem will be used not only to compute specific tasks, but also to bulk-rent machines in order to perform operations within a self-organizing network. Of course, this will require the simultaneous development of other technologies, many of which have gained significant traction in recent years. 

Better data-sharing technologies are necessary, but taking into account the ongoing development of IPFS/Filecoin and Swarm, the appropriate solutions seem to be within reach. Eventually, the Ethereum network will become more scalable, more efficient, and include a fully functional network of micropayment channels. Once these technologies become available, it is easy to imagine Golem primarily as a platform for microservices, allowing users to run both small (e.g. a note-taking app) and large (e.g. a streaming service) applications in a completely decentralized way. Although ambitious, this vision seems to be the ultimate argument for Golem’s long-term potential.

### When will the latest version be released?

Right now we cannot set a specific date for our next release. The best I can say is "as soon as its ready". While this answer in not particularly exciting, our technology certainly is.

We are working on brand-new, uniquely complex, and highly disruptive technology every day. This requires careful research, execution, and testing. We want to release the most secure and user friendly versions of the Golem App. This is not only important for Golem and our users, it is integral to the health of the blockchain ecosystem.

If you want to stay up to date on our progress, please follow our Rocket Chat. We post announcements and dev updates there. You can also connect with our team and fellow users to learn more about Golem. Our Github is also a good source if you want to take a look at our code.

https://chat.golem.network

https://github.com/golemfactory/golem

For specific updates on Brass progress, check our KanBan: 

https://trello.com/b/YL1qZ2pZ/brass-kanban

Thanks for your support and patience while we deliver our product!

### [back to top](https://github.com/golemfactory/golem/wiki/FAQ#jump-to-a-section)

# Golem technology
### How Golem works?

Golem is a p2p network, ie. there is no central server and users are equally privileged. People who want to compute tasks and people who have computer power to rent broadcast their offers in the network. Golem's transaction system matches providers and requestors, taking into account prices, reputations and their machines' performance. Resources, ie. files needed for computation are sent to provider's machine. After computation is completed, the provider's app sends back results to the requestor's app. If the result passes our verification process, the provider is paid. If someone tries to cheat, for instance sends bad results or doesn't pay, he/she will hurt their reputation and won't be chosen again for computations.

Check our [blog post](https://blog.golemproject.net/golem-architecture-bfd75faa8ecc) to learn more.

### How are your going to verify computations?

There will be different methods depending on the task type. In the future, a user who adds a new task can implement a new verification method that suits them. Possible solutions may involve: 
* simple correctness: checking of the result, eg. proof-of-work,
* redundant computation: ie. a few providers compute same part of the task and their results are compared, 
* computing small, random part of the task and comparing this part with the result sent by the provider, ie. comparing the color of few random pixels in rendered picture, 
* analysis of output logs. 

See our blog post for more info on our verification ideas: https://blog.golemproject.net/more-twain-less-cheating-129f7bc93a5c

### Why are you making it decentralized?

We believe that decentralization will be the future of internet development. With decentralization, it will be possible to achieve full scalability without expanding and maintaining our own network and server infrastructure; the solution will also be free from single points of failure and resistant to attempts to disable and censor the network. 

### Why are you using Ethereum?

We are building the transaction framework on top of Ethereum. Ethereum gives us expressive power, which is much-needed when implementing advanced, trustless schemes. Check our [blog post](https://blog.golemproject.net/why-ethereum-b398df34df9b) to learn more. 

### Are you using some external solutions / libraries?

We're using IPFS (https://ipfs.io/) for resource distribution and Docker (https://www.docker.com/) containers as computational environments.

### [back to top](https://github.com/golemfactory/golem/wiki/FAQ#jump-to-a-section)

# Golem business model
### How will payments work in Golem?

When creating something so new, it’s hard if not impossible to predict all the opportunities that will suddenly be possible. Golem is a generalized global supercomputer, and as such, it will no doubt find its niche with vastly varied applications. They might need very diverse remuneration models. We are not able to design a one-size-fits-all payment system for Golem, nor will we attempt to force one upon application authors. 
When a developer integrates her application with Golem, she has the freedom to decide which transaction model she implements, as long as it is compliant with Golem's Transaction Framework. The Transaction Framework will take the form of a set of requirements to follow; basic requirements may include:
* Entry in the Application Registry;
* Use of open source and/or deterministic environment, such as EVM;
* Community approval or rating of transaction model;
* Use of GNT for remunerating software and resource providers
We are building the transaction framework on top of Ethereum. Ethereum gives us expressive power, which is much-needed when implementing advanced, trustless schemes.
Example transaction framework components:
* Diverse payout schemes such as nanopayments, batching
* Off-chain payment channels
* Custom receipts
* Payment to software developer
* Per-unit use of software (per-node, per-hour, etc.)

It is also possible to introduce more sophisticated components into the transaction model design, to meet specific goals not related to payments. For example:
Requestor escrow for tasks where a higher level of commitment is required (high
price because of specialized hardware or long running subtasks); the requestor may
create a two-party escrow account and require providers to take part in it.
* Provider deposit: the requestor may require to be in control of some amount of
timelocked GNT.
* Requestor deposit: the provider may accept tasks only from requestors who are in
control of some amount of timelocked GNT.
* Registration of a task as an anchor for a TrueBit-style conflict resolution fallback
mechanism.

### What are use cases for Golem?

The first and most illustrative use case of Golem is CGI rendering. Other technically similar to implement use cases are scientific, engineering, statistical and financial tasks which need extensive computing and are (technically) feasible to distribute. Check our [blog post](https://blog.golemproject.net/what-can-golem-do-for-you-503b2449767a) to learn more about potential uses.  
We are not going to explore and develop all possible use cases, but we will rather focus on delivering a task API, Golem Standard Library to give developers the ability to integrate any software with the Golem Network.
Many use cases will need proprietary software, either existing or designed specially for Golem. To facilitate the use of both open and proprietary software, we will introduce the Application Registery to enable any requestor to use Golem-ready software. If the software is proprietary, then the requestor will be able to use it in a software-as-a-service model. This way Golem will act not only as a market for computing power, but also as a distribution channel for software creators.  


### Why computing prices will be lower with the Golem Network?

The prices are expected to be low because the market will be very close to textbook "perfect competition":
the product (computations) is homogenous,
the information for both requester and provider is almost complete, 
all requestors and providers have very small market share and have negligible impact on overall prices,
barriers to entry and exit are very low.
In a market with near "perfect competition" the prices are as low as they need to be to keep providers interested - which means that the Golem Network will create a situation that is quite different from today's internet infrastructure - with a few large providers exercising monopolistic control over the market.

Check our [blog post](https://blog.golemproject.net/why-should-render-farms-be-afraid-of-golem-3dd1b9e70f47) to learn more. 

### Why Golem is unlikely to be successfully copied?

Golem software is open-source and as such it can be forked by other parties. We are sure that over time many Golem forks will emerge either for specialised or general purposes. We believe that Golem's core business will remain unaffected by this.
* Golem business model strongly a favors larger network over a smaller network, so the first and largest network will always be preferable over the smaller networks.
* What Golem Network delivers is an infrastructure, open for any project, software, dapp, community etc. willing to use it. So any individual or organisation interested in building a decentralized solution (or a decentralized marketplace) will be able to use Golem as a platform, without a need of copying it. Therefore, developers will not be interested in copying Golem as long as we will be able to provide all the features they need.   
* Requestors choose where to buy computing power based on price and functionality. Our real competitors are Amazon Web Services, Google Cloud and other cloud providers. Our aim is to provide similar functionality at much lower prices.   

### How do you ensure fairness of task assignment in the network?

Right now it's mostly random. The most important is facilitating a direct connection and a quick network which will allow nodes to get tasks assigned to them as quickly as possible. It's a FIFO system. 

Later we'll add competition where the nodes with the best price / benchmark / reputation will be chosen. The Requestor should be able to choose which of this three options is the most important to them.

As the network grows we will be testing and implementing these methods to put the power in the user’s hands and ensure a healthy network.

### How does Golem compare to current/real supercomputers?

Supercomputers use fast low latency links between processors to exchange information about states of computation really (really) fast. Golem is being created to function in a different environment - medium to high latency connections. Golem is solving different sets of tasks at a fraction of the price.

### When will you support GPUs and How?

When we find or create suitable virtualization solution that supports virtual GPU on all our platforms. We’ve done some tests for Nvidia Docker, so there is a chance that Nvidia users may have support for GPU activated earlier. Also, Linux users may expect GPU support sooner than users of another OS. We plan to focus on that after the Brass release and we hope to have it ready with Clay or a little bit earlier.

In the future, as the network evolves and more developers build on top of Golem, we may explore other avenues beyond virtualization for computation environments, like host-direct modes. This is not a priority focus at this time though.


### [back to top](https://github.com/golemfactory/golem/wiki/FAQ#jump-to-a-section)

# Safety and Security
### Can you use private data for computation? Can providers see your data?

Unfortunately, right now Golem cannot support private data. Provider nodes usually need direct access to the data being computed so it will need to be decrypted at some point. 
Curious and technically savvy providers can look at what is being computed for now. We will be working over time on solutions to increase the privacy of computations. We have begun work with QubesOS, discussing the implementation of Intel SGX technology to help verify computations in a more secure manner.

### What if someone would like to use Golem for DDoS, Botnet or other illegal activities?

Computations take place in an isolated environment, so Golem can’t be used for DDoS or Botnet this way. We'll consider preparing special tasks that may have access to external data, but they won't be executed on machines if the provider doesn't deliberately agree to this. 

### Is it safe?

Every new technology is exposed to attacks, some new and unpredictable. All components of the Golem application will be designed to be robust against attacks. 

Key security elements will be:
* computations in isolated environments with minimal privileges and lack of external network connectivity.
* Well-known safety cryptography based on elliptic curves.
* Signed and encrypted messages inside the Golem network ensuring authenticity, which protects against man-in-the-middle attacks and passive data collection.
* Reputation system helping to detect malicious nodes and mitigate them. Evaluating these reputation metrics will assist in secure, efficient and correct task routing.
* Whitelist and blacklist mechanisms allowing providers to build trust networks and run only applications prepared by trusted developers.
* Together, the application registry and transaction framework mitigates Sybil and whitewashing attacks by providing an disincentive to participate, introducing an economic and computational cost to participation, and providing a metric for reputation in order to maintain optimal connectivity.
* The Ethereum integration and transaction framework makes custom payment-based security mechanisms possible, eg. escrows, deposits, insurance and audit proofs.
* Security audits will be conducted for every release, performed by external contractors.

### [back to top](https://github.com/golemfactory/golem/wiki/FAQ#jump-to-a-section)

# Using Golem

### Installing Golem

* [Installation on Mac](https://github.com/golemfactory/golem/wiki/Installation-on-Mac)

* [Installation on Windows 10](https://github.com/golemfactory/golem/wiki/Installation-on-Windows)

* [Installation on Ubuntu](https://github.com/golemfactory/golem/wiki/Installation-on-Ubuntu)

Make sure you choose the latest install package when installing on Windows.

If you don't have a public ip, your router doesn't support uPNP, you need to forward ports 40102,40103 and 3282 to your machine from your router for Golem to accept tasks. Refer https://bitcoin.org/en/full-node#enabling-connections for port forwarding instructions but use above ports instead. You may also need to open the ports through your firewall. For router specific instructions on how to forward your ports go to https://portforward.com/

To check if your ports are forwarded correctly you can use www.canyouseeme.org

### Setting and Saving Your Password

Golem is Open Source software built on the Ethereum blockchain as part of a P2P network, because our network security relies on the decentralized nature of blockchain technology we do not keep backups of your wallet keys or password. We recommend that you backup your keys and password by writing them down and storing them in a safe place. This is the best way to protect your data.

We do not offer password recovery so please write down your password when you first install Golem. We also have documentation on how to backup your app and keys here.


### App Overview

Here are some direct links designed to give you a top to bottom overview of the Golem App. Included in these docs are some troubleshooting tips for common issues. 

* [Getting Started](https://docs.golem.network/01-getting-started.html)

* [Running Golem](https://docs.golem.network/02-running-golem.html)

* [Adding Tasks](https://docs.golem.network/03-adding-tasks.html)

* [Task Settings](https://docs.golem.network/04-task-settings.html)

* [Troubleshooting](https://docs.golem.network/10-troubleshooting.html)

### What are the optimal settings for my machine to run Golem?

In general we recommend a processor with multiple cores and lots of RAM. At minimum, you can run Golem with:

* 2 GB RAM
* 2 cores
* 20 GB HDD
* public IP or ability to forward ports

For more demanding renders like the Production Benchmark (https://www.blender.org/download/demo-files/) you will need at least:

* 16 GB RAM
* 6 cores

In the future we plan to support GPUs for use within Golem. Docker currently only supports virtualization for Nvidia GPUs, so those cards are likely to be supported by Golem before other models. GPU support is planned for the Clay release.

After initial tests we do not have a standard for the "optimal" machine. As the network grows there could be a way to determine which configurations perform better than others. Right now, our main focus it building a strong network. Over time computing standards will become more refined. The best rule of thumb right now is "the more power you are willing to spare, the more tasks you will receive".

### What data do I share with Golem?

We will automatically send any errors that occur in your Golem instance to our dev team so they can improve the product in later releases, your private data will remain private. Specifically, we will be creating a live feed of traceback errors so we can identify bugs more quickly and speed up development on new features.

To be clear we do not store or share any personal data, we only use traceback error data to help improve the app. Because we do not store any other personal data, it is important to write down your password and keys and store them in a safe place.


### How much money can I expect to make with Golem?


It is too early to give estimates like this, but you can refer to our [blog post](https://blog.golemproject.net/why-should-render-farms-be-afraid-of-golem-3dd1b9e70f47) to understand better how we fit in the market and what financial and technical advantages we offer.

As we grow, your earning potential will also grow.

### Why do I need GNT and ETH?

- GNT:

GNT or Golem Network Token is needed to pay for computations on the network and is the currency that drives our marketplace. As a Requestor, you set a bid for an amount of GNT you are willing to pay to have your task completed. As a Provider, you earn GNT by computing tasks for Requestors. You can set your minimum and maximum price thresholds in your settings.

- ETH:

Golem uses the Ethereum blockchain to facilitate fast and secure payments between Requestors and Providers. ETH is the native currency of Ethereum and is used to pay for transaction fees on the network. Only a small amount is needed to complete a transaction. All Applications built on the Ethereum blockchain pay for transactions using ETH.


### Feature Requests

To help get more visibility for your request feel free to send me more details to contact@golem.network. We are always looking to improve our app and your feedback is appreciated.

Be sure to include:
* Screenshots
* Use Case
* Pain points of existing system

If this issue is more severe and disrupting your workflow within the Golem App, you can report it here as well: https://github.com/golemfactory/golem/issues

### Backing Up Your Golem App

We recommend backing up your Golem app when after installing. This will allow you to restore your Golem node if your machine crashes and you need to install your node on another computer without starting from scratch with your reputation.

All you need to do is copy all the files in your app directory. The locations of the app directories for each OS are here:

**Windows:** C:\Documents and Settings\<User>\Application Data\Local Settings\golem\golem\default

**MacOS:** ~/Library/Application Support/golem/default

**Linux:** ~/.local/share/golem/default

Once you’ve copied all the files in your app directory, paste them into an external hard drive, or another storage device of your choosing.

To restore your Golem app, run through an installation and then copy these files back into your app directory.

### Backing Up Your Golem Wallet

Your Golem wallet stores GNT and ETH for use on the network. We highly recommend that you backup your wallet when you begin to use your Golem app. That way if your computer crashes and you cannot recover your files, you have the keys to your wallet to restore Golem on a new machine.

**Finding Your Wallet Keys:**

Your wallet keys can be found in your app directory. The locations of the app directories for each supported OS are below:

**Windows:** C:\Documents and Settings\<User>\Application Data\Local Settings\golem\golem\default

**MacOS:** ~/Library/Application Support/golem/default

**Linux:** ~/.local/share/golem/default

These directories contain everything associated with your Golem account and the app itself. The exact location of the wallet keys are inside those directories under:

 `/keys/keystore.json`



Copy your keys from that file directory onto a piece of paper and store in a safe place. You can also back these files up to another hard drive if you wish, but the safest way to store this data is to write it down (just remember where you put it!).

# Submitting a Task

### Two Ways to Add a Task:

For individual users, there are two ways to add tasks to the Golem desktop app, via the Add Task button (circle with a “+” sign) on the main toolbar which allows the user to select a file through the system chooser or via drag and drop. Both single files or folders can be added.

To add a task via the system chooser, click the Add Task icon, select your file or folder and your task will be added to Golem (after you have filled out the Task Settings).
To add a file via drag and drop, simply drag a file (or multiple files inside a folder, in case of tasks with multiple resources) onto the Task view, and the task will be added.

**Task Settings:**

Your task settings and computing time will vary depending on the complexity of your Blender file, but there are some basic principles to understand and general guidelines to use when submitting a task to the network. Below is a breakdown of all you see on the Task Settings screen. 

**Local Render Test:**

Before Golem can assign your task to other nodes, your machine must first complete a local render test. Golem prompts your machine to render a single low resolution frame of your file to determine if it is a valid blender file. This is integral to our verification process and must be completed to ensure the accuracy of computations.


You will see a small window with an icon showing the status of your local render test. Once the test is completed, you can finish up the rest of the required settings.

### Render Settings:

This section includes all render specific settings:

**Preset:** A dropdown menu where you can choose from saved settings that fit your workflow. This is great for users who render the same or similar files more often.

**Dimensions:** Standard HD dimensions are 1920 x 1080 but you can set whatever dimensions fit your needs in this section.

**Frame Range:** Define frames to render. You can separate frame numbers with ;, eg. 1;4;7 will define frame 1, 4 and 7. You can also define frames ranges with -, eg. 1-4 will define frame 1, 2, 3 and 4. Finally, you can also define every x-th frame with ,, eg. 1-10,2 will define frames 1, 3, 5, 7 and 9. So defining frames to render as 1-4;7;10-30,5 will render frames with numbers: 1, 2, 3, 4, 7, 10, 15, 20, 25, 30.

**Format:** This determines the output format of your render frames. Blender supported formats are PNG and EXR.

**Output to:** Choose your output filepath. This is where your render frames will be saved. This will override your default file location in your App Settings.

**Blender Compositing:** Turn this feature on if your blender file requires the use of compositing. It’s suggested to turn off this option if you have more subtasks than frames, otherwise images may not be rendered correctly. To learn more about compositing go here: https://en.wikibooks.org/wiki/Blender_3D:_Noob_to_Pro/Compositing

*Note: At this point you can save your settings as a preset. If your files uses Cycles, there will be an option to set how many Samples you want instead of Frames.*

### Task and Subtask Timeouts:

Task and Subtask timeouts are the most important settings when submitting a task. So be sure to carefully consider the size and complexity of your blender file when setting timeouts.

**Task Timeout:** Determines how long you are willing to wait for your task to be computed. This setting should be much higher than your subtask timeout and significantly higher than you expect your render to take. If you render takes 4 hours on your personal machine, then set your Task timeout to 8-10hrs. It is likely that your render will take less time, but you need to be safe since you are paying for the render and you do not want to accidently timeout before the render is completed if your personal connection is slow or if network traffic is low.

**Subtask Amount:** Tells the system how many subtasks to break a task into. Generally if you are rendering a number of frames you should set subtasks to the same number.

**Subtask Timeout:** Determines the timeout threshold of every individual subtask. This setting should be significantly lower than your overall task timeout. You can use the following formula to determine a starting point for your subtask timeouts:

	Overall Task Timeout / Subtask Amount + 1 hr

	10hr Overall Task Timeout / 5 subtasks + 1 hr = 3hr subtask timeout

If you set your subtask timeout too high, you can get stuck with a weak node trying to compute your subtask which could lead to network performance issues. If your subtask timeout is too low, then you run the risk of even high powered nodes not finishing your task.

Note: If your task times out halfway through, you will still pay for subtasks computed. If you are rendering an animation rather than a still image, it is best to have your subtask amount match your frame amount. This means that if a timeout occurs, but some of your subtasks were still computed, you can re-submit the task with the previously completed subtasks removed to avoid rendering them twice (and paying for them twice).

From: https://en.wikibooks.org/wiki/Blender_3D:_Noob_to_Pro/Basic_Animation/Rendering

“Animation rendering can take a while. Consider a short animation sequence of, say 10 seconds at 25 frames per second—250 frames. If a single frame takes 10 seconds to render, then the whole sequence will take about 40 minutes. If a single frame takes a minute, then the whole animation will need over 4 hours to render. And it gets worse the longer the movie is. And so it goes.”

This is why Golem exists, to save you time while rendering.

Once your settings are complete you can set your price. Learn more about price here. (link to pricing best practices below.


Local render test determines if the file is valid, if it uses cycles, if it is valid blender file. Imperative to verification and accuracy.

https://docs.golem.network/04-task-settings.html
Determining whether or not your blender has cycles
File Guidelines

You cannot submit a file that is IP protected, this includes rendering copyrighted material without the license to do so.
Pre-Baking must be completed on any files which require it before rendering with Golem
Using the Particle System to create randomly generated objects (ie. trees, fire, snow) may not work with Golem. You must pre-bake the file and attach the added elements to your task
If your machine is not powerful enough to create the local test render, you will not be able to submit your task

Figure out all variables and most common uses - provide recommended settings

If task times out they cannot start again in middle. Halfway timeout, start again, start from beginning paying 1.5x

Video: Submitting a task (wait til last moment); Timeouts explained (benchmarking files); Pricing best practices

You cannot submit any task with asserts that are IP protected
Pre baking scene - need to be done before using render farm or use special instructions
Randomly created object - trees, shifted or gone, wont be able to use Golem (Particle System?) Do not use in Golem

Pre bake scene, attach element with particle add multiple elements to the blender task, fire, trees, snow. Submit to Golem:

Multiple elements - Drag and drop only for windows, Plus only for Mac.

https://docs.blender.org/manual/en/dev/render/blender_render/bake.html


### Pricing Best Practices

Pricing Best Practices:*

The formula for calculating the estimated cost of a task: 

{subtask amount*GNT/h*Subtask timeout settings in hourly increments}

Examples:

5 substasks * 0.5 GNT/hr * 30mins Subtask Timeout = 1.25 GNT

  - or 5 * 0.5 * (30/60) = 1.25

10 subtasks * 1 GNT/hr * 1hr Subtask Timeout = 10 GNT

  - or 10 * 1 * 1 = 10

**Note: If your settings result in a number with long decimal, Golem will round to the nearest 100th.**

3 substasks * 0.5 GNT/hr * 12mins 30sec Substask Timeout = 0.31 GNT

  - or 3 * 0.5 * (12.5/60) = 0.3125 rounded down to 0.31

5 subtasks * 0.5 GNT/hr * 15mins 30sec Subtask Timeout = 0.65 GNT

  - or 5 * 0.5 GNT/hr * (15.5/60) = 0.645833333~ rounded up to 0.65



Since price is directly tied to your subtask timeouts, it is important to test your typical workflow a few times in our alpha app to determine the best settings for the lowest price.

User is paying for payment for task (cost: nodes-that-are-computing-tasks*price-estimation*GNT-price)


### What do I do if something goes wrong?

The first things to do if you have any error while running Golem are:

* Make sure you have the [latest version](https://github.com/golemfactory/golem#installing-and-testing) installed

* Make sure your ports are forwarded properly or have a router that supports uPNP

* [Check your logs](https://github.com/golemfactory/golem/wiki/Testing#where-are-the-logs), copy any Error or Critical message you find and search for them on our Github. This will help you find any related issues, open bugs, or troubleshooting tips

* [Check our troubleshooting doc](https://docs.golem.network/10-troubleshooting.html) for related errors and fixes

* Reach out to us on [Rocket Chat](chat.golem.network) with a detailed description of the issue

* Send a detailed description of the issues along with attached log files to contact@golem.network

* If you feel confident you discovered a bug in the system or a missing critical feature, you can [create an issue on GitHub](https://github.com/golemfactory/golem/issues). Please provide relevant log entries, screenshots, and detailed descriptions of expected vs. actual app behavior. Fore more instruction on reporting issues [check here](https://github.com/golemfactory/golem/wiki/Testing#what-kind-of-comments-do-we-expect)

### My task is stuck and not rendering

* Make sure you have the latest versions of both Golem and Blender installed
* Check if you can see your node on https://stats.golem.network/show
* Test for open ports 3282, 40102 and 40103 with an external tool like canyouseeme.org ( app must be running )
* Adjust your Network Trust settings to accept more incoming nodes
* Check your task settings to see if you set high enough task and subtask timeouts, if not, retest with higher timeout thresholds
* Test a smaller blender file to see if it renders: [Golem Logo Demo](http://golem.timjones.id.au/)
* Check for errors in your logs [found here](https://github.com/golemfactory/golem/wiki/Testing#where-are-the-logs)
* If you still cannot render a task send the following to contact@golem.network:
    - A screenshot or description of your task settings and network trust settings
    - Your Golem.log and Hyperg.log files
    - The name and size of the blender file you were attempting to render

### [back to top](https://github.com/golemfactory/golem/wiki/FAQ#jump-to-a-section)

### Docker Errors

If you receive any errors regarding the Docker VM in the GUI or in your logs it is always to try the following steps to troubleshoot:

* Shutdown the Golem App

* `Docker-machine ls`

     - This command shows if docker is running any errors. It is good to run this command before and after running any of the following docker commands to see if the error is solved.

* `Docker-machine restart golem`

     - This will restart docker’s golem instance.

* `Docker-machine rm golem`

     - This will remove the docker container. If you see an error when running this command contact Golem Support.

* `Docker-machine create --driver xhyve --xhyve-virtio-9p golem`

     - This will create and engage the necessary drivers for your docker machine


* Now you can restart Golem and test.


# Comparing Golem to Other Services

### Golem vs iExec

iEXEC’s idea sounds very similar to Golem, but it is not exactly so, as iEXEC focuses on requestors, defined as dApps creators, that want to run off-chain computations. At least over the course of the next year we will be addressing non-overlapping use cases and users. At some point our technologies may come closer and we can learn from each other, which would likely be beneficial for both projects, as iEXEC the team seems to be competent & delivering.

### Golem vs SONM

SONM’s goal is similar to what we are trying to achieve. According to SONM’s team, it is a "secure and cost-effective fog supercomputer, designed for general-purpose computing, from mobile app hosting to video rendering to DNA analysis. Miners all over the world can leverage their idle computer power to become part of the SONM network." But, although we have tried really hard to comprehend their development process, it's really hard to tell where are they heading at the moment. We have yet to see how they have solved fundamental problems for such a design to work. 

For now it is safe to say that the main difference between us is license (Golem: GPLv3, SONM: Apache Licence 2.0) - they announced that their main framework or a platform is called COCAINE (Configurable Omnipotent Custom Applications Integrated Network Engine) https://tech.yandex.com/cocaine/. In addition, we are not using any third party frameworks.

### Golem vs BOINC

* BOINC is not a marketplace
* It is a centralized solution (you cannot just join as requestor)
* BOINC verification is based on excessive redundancy (everything is computed 3 times)
* trust comes from centralization (because providers get tasks only from whitelisted requestors, requestors are trusted)

Also, because there is no market and BOINC is based on computing time donations, you have to jump through many hoops to be able to become a requestor. 


### Does Golem Factory invest in other businesses? ICOs?

We do not invest in ICOs. We should not speculate with ETH and nowadays ICOs have enough traction to fund themselves without our help. We want to support other projects where our technology overlaps or which would make good use cases for Golem. In such a case we might invest time and resources in cooperation with in another business for our mutual benefit.

Golem would prefer to work together to achieve mutual goals than to speculate and invest capital.

### [back to top](https://github.com/golemfactory/golem/wiki/FAQ#jump-to-a-section)


# Golem Token

### What is the purpose of Golem Network Token?

GNT is used to pay for rented computing power on the network. For more information about how GNT fits into the network, see our blog post on the [Economics of the Golem Network Token](https://blog.golemproject.net/the-economics-of-the-golem-network-token-d64c1a50b1d5)

### Can I deposit and withdraw real GNT and ETH during the Alpha test?

Since we are in the Alpha stage our first POC, all GNT on the app is test GNT (tGNT) and has no value outside of the app. We have purposely removed deposit and withdrawal options from the Alpha test because they are not necessary. Do not under any circumstances attempt to send real GNT to your node ID, you will lose your tokens permanently and we cannot get them back for you.

The same goes for ETH. All ETH balances you see on the Alpha app are test ETH (tETH). The Golem alpha is being run on the Rinkeby Testnet, and no ETH holds value on this testnet. Please do not send any real ETH to your node ID or the Golem Smart Contract address. You will lose your tokens forever, and we cannot get them back for you.

When we launch the mainnet version of the app, we will have deposit and withdrawal options for real GNT.

### Where to Purchase GNT

While we do not endorse or work with any exchanges directly, you can find a list of exchanges that offer GNT here:


https://coinmarketcap.com/currencies/golem-network-tokens/#markets

### What wallet should I use to store GNT?

The two most popular wallets used to store Golem are:

https://www.myetherwallet.com
https://github.com/ethereum/mist/releases


Be sure to read and follow all of their safety instructions before sending your GNT to your new wallet. There are a lot of phishing scams out there, and if you are not careful, you can easily compromise your wallet security. If you follow their instructions carefully you should have no problem.

For more wallet suggestions from our users [go to our chat and pose your question in the #wallets room](chat.golem.network)



### "I sent my tokens to the wrong address and my GNT is gone"

At Golem we do not work directly with any exchanges or facilitate transactions of GNT from Wallets to Exchanges or vice versa. For that reason we cannot help you get your tokens back or reverse the transaction. Transactions on the blockchain are irreversible.

But we can still offer some help.

The best thing you can do going forward is:

* Search for the transaction on etherscan.io
* You can use your public key
* Gather information from etherscan and send to your exchanges support team
* If the support team is unresponsive, sometimes posting on the exchanges subreddit can get exposure for your issue

At Golem we are only working on the App. The GNT token is an important part of our ecosystem but we are powerless to help with transactions between independent investors and 3rd party exchanges.

### [back to top](https://github.com/golemfactory/golem/wiki/FAQ#jump-to-a-section)