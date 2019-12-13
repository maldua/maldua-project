# maldua-project
Humble attempt to fork Zimbra project

# 2020 year objectives
 * Document Ubuntu 16.04 build
 * Automate Ubuntu 16.04 builds and releases thanks to github actions (or equivalent)
 * Document changes needed to decouple current build from Zimbra (or other external) servers (I.e. https://github.com/Zimbra/zm-zextras/blob/4e3bc897ecff92e64516c69d08c0b5c36430de08/Makefile which relies on AWS servers).

# 2019 year objectives
 * Mirror current github Zimbra repos (and automate it) [**Done**]
 * Write FAQ explaining the project [**Done**]

# FAQ about maldua-project
## What about the maldua name?
The [@ (at) symbol](https://en.wikipedia.org/wiki/At_sign) is called:
 - **Mal**pa in Polish language.
 - Bil**dua** in Basque language.
 
 You mix the two of them and **maldua** appears.
 As a bonus maldua was not a github username.
 
 The maldua name is just an excuse to be able to name this mirror/fork project.
 
 I'm sure that a better name will be choosen in the future if this is no longer a **humble** attempt.
## If you want to maintain a fork you need people and money
 For now, the fork will be kept on the technical side. Later on we might seek for money.
## Current ZCS 8.8.x needs help
 - Q: Current ZCS 8.8.x versions need help on adding stuff, improving security and integration with third party tools. You might want to focus your effort there.
 - A: Getting up and running a fork is not done in one month. I prefer to focus on the fork so that we can ready in a few years.
## Is Zimbra X not being suitable for on-premise the main concern?
  - Q: My main concern is that Zimbra 8.8.x which it is on-premise will be deprecated. Synacor might focus its development power into Zimbra X and on-premise might die. Is it also the reason for starting this fork?
  - A: Not at all. We are quite convinced that you will be able to deploy Zimbra X on-premise despite you having to invert on some virtualisation improvements. Anyways, our main concern is Zimbra X not becoming open source on a first step and much later on Zimbra 8.8.x also not keeping its open source license.
  - A: Being able to use Zimbra on-premise is secondary. Once Zimbra on-premise is no longer open source the Zimbra product will no longer be competing to equivalent open source products. Instead it will be competing to both privative and open source products. Many more improvements than current features will be needed to be a competitive product in that new market.
## Doing a fork is a massive undertaking
 - Q: Doing a fork is a massive undertaking. You need a real commitment. A commercial incentive.
 - A: We know. Commercial part can be postponed for now.
## If I ever decided to use a Zimbra fork I would need an associated credible support plan
That's a good point. Some kind of company or foundation will need to put in place in the future in order to offer credible support plans. For now we will focus on the technical side of things.
## Zimbra community is too selfish
 - Q: My experience on the current Zimbra community has been disappointing. When I explained some of the current European Zimbra partners about Zeta Alliance there was almost no useful contribution back. Every one of the partners just talk about their book (their own interests) ant that's it. How are you supposed to create such a fork if there is no community?
 - A: Zimbra has never been actually *ethical open source*. The different companies backing Zimbra product never encouraged a true open-source development community around it. There was never a public development mailing list where Zimbra employees and foreign developers could work with equal commit permissions on the FOSS products.
 - A: Zimbra has never been actually *ethical open source*. Not being able to sell the open-source version of Zimbra while also being a Zimbra partner for so many years has left many open-source actors from Zimbra.
 - A: So, yes, what you explain here makes sense. If the only difference between Zimbra and privative products is not a community-driven development but just a source code addendum (which only the most savvy will look into from time to time) then the Zimbra community is left with privative-alike companies supporting it. Private-alike companies tend to be selfish, yes.
 - A: This Zimbra fork will encourage a community driven development from its start in order not to repeat old Zimbra errors on this matter.
## On the Owncloud/Nextcloud fork
 - Q: Doing a fork does not need to a good thing. Some of the [Owncloud developers](https://karlitschek.de/2016/04/big-changes-i-am-leaving-owncloud-inc-today/) forked Owncloud into Nextcloud on [april 2016](https://civihosting.com/blog/nextcloud-vs-owncloud/). Now Nextcloud adds new features on each one of its releases. Is that a good thing? I'm not sure that's a good thing. It might not be a good thing for an entreprise where you want a more stable product.
 - A: Well, as a company you would be able to fork again this Zimbra fork if you find its development pace to be too fast. Just make your own stable version as Redhat does with RHEL out of Fedora. If making your own stable version is too daunting you can either propose a joint-venture or foundation with other Zimbra interested companies or you can stick with the original Zimbra. Zimbra has a lot of traction and will have it for many years. It's not going to disappear interest for Zimbra once this fork is alive.
## Partners will not help you
 - Q: You might think that current Zimbra partners, the companies that might be more interested in a Zimbra fork will help you. But they won't. Why? Because they are not allowed to sell open source.
 - A: As we commented before once Zimbra on-premise is no longer open source the Zimbra product will no longer be competing to equivalent open source products. Instead it will be competing to both privative and open source products. Many more improvements than current features will be needed to be a competitive product in that new market. That means that the current Zimbra partners in a few years might need to decide what they do about Zimbra.

This might not be like this in the future but let's sci-fi a bit:

If they embrace the open source Zimbra fork:

 - Pro: They won't be lossing their clients whom care on Zimbra being open-source product.
 - Con: They might have another alternative support unknown to them
 - Con: Might need to migrate to a new platform if the fork has diverged too much

If they keep using original Zimbra:

 - Con: Their clients whom care on Zimbra being open-source product might leave for another company.
 - Pro: Already known Zimbra support.
 - Pro: No need to migrate to a new platform if the fork has diverged too much

If my company relied on an 80% percentage on clients whom care on Zimbra being open-source product and it was sure that Zimbra was no longer going to be released under an open source license I would plan on switching to the Zimbra fork while at the same time contributing to it.

## What if Zimbra is always open-source
 - Q: I think you assume too fast that Zimbra is going to be privative and not being kept released under an open-source license. What will happen to this fork if Synacor states that Zimbra is going to be release under an open-source license for the next several years? What will happen to this fork if Synacor states that Zimbra X is going to be release under an open-source license for the next several years?
 - A: As I said before Zimbra has never been actually *ethical open source*. I believe that a healthy open source community is the one who can fork a current project under one year without too much hassle with around 20% of the community members.
 
 If Zimbra is kept under an acceptable open-source license our efforts might be redirected to:
  - Allow the community to build and fork Zimbra just in case it's once again needed in the future
  - Help to teach new developers on how to contribute source code back to Zimbra
  - Contribute with extra addons for Zimbra which might be integrated into Zeta Alliance
  - If Zimbra X is privative we might attempt to extend current Zimbra so that it has an equivalent functionality

# maldua-mirror
[maldua-mirror](https://github.com/maldua-mirror/maldua-mirror) updates its own git repo fork for each one of the Zimbra organization repos daily at 05:30 UTC. You can explore the forked repos at the [madua-mirror organization page](https://github.com/maldua-mirror).
