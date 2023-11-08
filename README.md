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

## Why this idea ?

We can also think about a two step push with pushing image on Ordinals and after trigger a `minsta mint` operation but it will more expensive. Minsta is already stored on [arweave](https://docs.arweave.org/developers/).

So, it's cheaper and it's a first easy implementation of a cross protocol between mintbase and ordinal.

## Go beyond

What we can see with this technical purpose is anyone can mint a bitcoin only transaction without beeing related to mintbase.

To solve this issue, the Near BOS with 

1. Create a create-near-app : `git clone git@github.com:near/create-near-app.git`

2. Fork minsta template : `git clone git@github.com:Mintbase/minsta.git`

3. Fork atomicals-js or be able to call `yarn cli mint-nft file`.



