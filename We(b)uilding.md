
Who's workflow process for fxwho.xyz


December 30, 2022NEW

 ![](https://cdn.discordapp.com/avatars/898548471223685130/45488199977e1b6ca72750ffe06d565f.webp?size=16)@x0y0z0
    
    @who? hi, sorry for disturbing you, are you the developer of fxwho? I like that web, what tools did you use to build it? I would like to learn more about how to build dapps? do you have some recommendations to read about it? until now I have been reading the website opentezos
    
    ![](https://cdn.discordapp.com/avatars/909756354871320606/aac9c0e4cc59e24fd349340fb1ea8514.webp?size=80)
    
    ### who?![](https://cdn.discordapp.com/role-icons/928606673931739136/4c9d8379884230c344c56ab7dc76e097.webp?size=20&quality=lossless) _—_ Today at 10:38 AM
    
    No worries, always happy to chat about it! Some quick bullets about what I use - Typescript everywhere - essential - Vanilla React as the application layer - npm + webpack for the bundling - anything works here - Cloudflare pages for deploy - unlimited fast serving for free, highly recommend - Custom data routing, no Redux or similar - Taquito for the contract operations up (and their beacon wallet wrapper). Getting this to build is a bit of a pain, their codebase seems a bit questionable - need to include a bunch of shims in your build system - Apollo for graphql queries (fxhash / tzprofiles apis) - tzkt typescript apis for most data fetching - I use the tzkt indexer for almost all of the data I pull from the chain - Very minor use of conseiljs for some Micheline / Michelson data packing / unpacking - Taquito can do this but I found conseil a little faster in some cases - The usual assortment of normal web dev stack for the app itself - immer, react table, sass, etc As far as resources, opentezos is definitely a good place to start. Building a view-only app (pulling and displaying data from tzkt) is a good easy place to start if you have something in that space that interests you - [https://api.tzkt.io/](https://api.tzkt.io/ "https://api.tzkt.io/") and [https://better-call.dev/](https://better-call.dev/ "https://better-call.dev/") will be your friend here. If realtime speed isn't your goal, pulling everything from the fxhash graphql API via Apollo is a really good option - lots of great fxhash tools do this. Digging through the graphql API at [https://studio.apollographql.com/sandbox?endpoint=https%3A%2F%2Fapi.fxhash.xyz%2Fgraphql](https://studio.apollographql.com/sandbox?endpoint=https%3A%2F%2Fapi.fxhash.xyz%2Fgraphql "https://studio.apollographql.com/sandbox?endpoint=https%3A%2F%2Fapi.fxhash.xyz%2Fgraphql") is super helpful. For fxhash tool development specifically, the integration guide on the site is a great intro too- [https://www.fxhash.xyz/doc/fxhash/integration-guide](https://www.fxhash.xyz/doc/fxhash/integration-guide "https://www.fxhash.xyz/doc/fxhash/integration-guide"). Once you move on to interacting with the chain, [https://tezostaquito.io/docs/tutorial_links/](https://tezostaquito.io/docs/tutorial_links/ "https://tezostaquito.io/docs/tutorial_links/") is a great place to start. The `ghostnet` will be your friend here! It's definitely not a soft landing, but my best tip if you want to really dive in is to get familiar with the fxhash website codebase, which is open source at [https://github.com/fxhash/fxhash-website](https://github.com/fxhash/fxhash-website "https://github.com/fxhash/fxhash-website"). I've spent many hours combing through this and it does help give a sense of how a high quality dApp can be laid out. Some of the decisions there are definitely made with scale in mind so might not make sense to follow, but it's a great place to get a feel for what an end to end site can look like.
    
4.  _[_10:39 AM_]_
    
    That was a bit of a meandering response with a lot of run-on sentences, but hope it gives you a few places to get started!


