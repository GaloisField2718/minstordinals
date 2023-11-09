# Goal 

Create a new [json-based protocol](https://medium.com/@MySsistant/what-is-the-ordinals-protocol-that-brc20-tokens-are-based-on-a1ebe4f00f96) on top of [Ordinals](https://docs.ordinals.com/) related to minsta NFTs.

## Idea 💡

When you mint a nft via minsta it triggers a transaction on Ordinals with pushing a json which should looks like : 
```json
{
  "p": "minsta",
  "op" : "mint",
  "minsta-account" : "my_account.minsta.near",
  "minsta_id" : "aef...",
  "file" : "https://mintbase.com/aef...",
  "meta" : "Your description and much more coming soon ;)"
}
```

## Why this idea ❓

We can also think about a two step push with pushing image on Ordinals and after trigger a `minsta mint` operation but it will more expensive. Minsta is already stored on [arweave](https://docs.arweave.org/developers/).

So, it's cheaper and it's a first easy implementation of a cross protocol between mintbase and ordinal.

## Go beyond 🚀

What we can see with this technical purpose is anyone can mint a bitcoin only transaction without beeing related to mintbase.

To solve this issue, the Near BOS with indexers could be solution [NEAR Lake Indexer | NEAR Documentation](https://docs.near.org/tools/near-lake). We will try to show you how it can works in theory to be sure that only valid inscriptions regarding minsta mints are valid to use into Near Ecosystem. 




# Step-by-step implementation 👣

[IN PROGRESS] `/docs` : should contains technical documentation of our project 📂. The main technical vision should be present in it. The slides will be here also.
  [x] `/schemas` : Roadmap and workflows.
  [IN PROGRESS] `whitepaper.pdf` : Describe each part of minstordinals, its implementation and its vision. 
  [] `doc.pdf` : A more complete documentation with technical information.

[] `/minsta` : should contains technical implementations and integrate the call for ordinals inscriptions.

  [] Modify colors and appareance. 
  
  [] Check nft deployment. The goal is to understand what data are required, what are given and what can we get from deployment. 

  [] Write the script to push json file on Ordinals. 

  [] Push one basic `minsta mint` json file with [Testing - Ordinal Theory Handbook](https://docs.ordinals.com/guides/testing.html).


[x] `/ressources` : every ressources used during this hackathon should be contained here. The `README.md` file into it would contain links for references. 

  
[x] `README.md` : should be our organisation point. 



# Tools 🧰

- [binary -> ordinals/ord: 🗨 Rare and exotic sats](https://github.com/ordinals/ord/releases/tag/0.11.0)



