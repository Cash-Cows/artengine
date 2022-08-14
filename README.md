# Cash Cows Art Engine

By CAO order of [CCIP4: Open Source](https://dao.wearecashcows.com/#/proposal/0xccb5e6d7e9fa1ed02e9429327b14995bdaa78e6ffc55a01b17a10806df4831b7), 
The Cash Cows project is now open source. Please observe and respect our
[open source license](https://github.com/Cash-Cows/artengine/blob/main/LICENSE).

```
Cows do not guarantee that this code, is the one actually used right now.
Cows cannot guarantee that this code will work for everyone. If cows want 
to use this, you can! But cows must also open source their code too.
```

Moo. 

## About Cash Cows

[wearecashcows.com](https://www.wearecashcows.com/)

Cash Cows is an NFT experiment about sharing the creator fees with its
holders. We aim to lead this space in Web3 with innovations that the 
World has never seen before.

 - [ERC721B](https://www.npmjs.com/package/erc721b) gas efficient minting
 - First collection in history to design and implement a community royalty splitter 
 - Zero-Gas marketplace listings
 - First design and implementation of ERC721Soulbound
 - First enterprise grade digital asset store
 - Economics centered design

[Join the Cowmmunity on Opensea](https://opensea.io/collection/cash-cows-crew)

## Install

```bash
$ git clone https://github.com/Cash-Cows/artengine.git
```

## Usage

1. Run the following command `npm run setup`. This itemizes the usable 
layers and saves in `config/layers.json`

2. Setup `config/engine.js`. Cows have added all the layer 
configurations actually used to generate the collection.

3. Run the following command `npm run bulld`. This will create a new 
`build` folder in your root project directory. It will take a while 
to complete. Inside the `build` you should see the final images in
the `image` folder and metadata in the `json` folder.

4. Run the following command `npm run rarity`. This will make a file 
called `rarity.html` in the `build` folder. Open this in the browser
to check the rarity results and determine if you should tweak the layers
in `config/engine.js` again and build again. We did this step for 
several days.

Upload and pin on either **Pinata** *(paid, but reliable)* or 
**nft.storage** *(free, but takes a while to pin)*. 

5. Copy the contents from `.env.sample` to a new file called `.env`

6. Whichever you choose, obtain the API keys and set it in `.env`

7. Run the following applicable command 

 - `npm run nft.storage`
 - `npm run pinata`

This will take a few hours depending on the size of the collection. 
You can stop these commands anytime and restart without losing your 
place.
