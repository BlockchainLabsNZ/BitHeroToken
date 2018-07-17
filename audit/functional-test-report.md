# Functional tests
Tests are conducted on the Kovan test network. The following contracts has been verified on Etherscan.
 
## [`CrowdsaleToken[0xb60237]`](https://kovan.etherscan.io/address/0xef32068b9921231d27d37b177a986c3afab3d140#code)
## [`AllocatedCrowdsale[0xe9c590]`](https://kovan.etherscan.io/address/0x92d9bfd9a76f2f2e7ec04e7e763da10b3ee03f5e#code)
## [`UpgradeAgent[0x780a56]`](https://kovan.etherscan.io/address/0x780a566020076b9f1fd8c993f6be80fa7c885730#code)
## [`MultiSigWallet[0x9226fd]`](https://kovan.etherscan.io/address/0x9226fd784bf8d5615bf9547014840fffdea6a18e#code)
## [`FlatPricing[0x799e9d]`](https://kovan.etherscan.io/address/0x799e9d3191b5f59cd2a604140f07b1bac0385e01#code)
## [`DefaultFinalizeAgent[0xebc06a]`](https://kovan.etherscan.io/address/0x1e1bbdb147fb59d3f08fd67c2bf2f535b41d6b92#code)
 
## Accounts
 
* Owner: [0x006F3FCdDaf248D1a4C9A7fd62939963AAAe5a67](https://kovan.etherscan.io/address/0x006F3FCdDaf248D1a4C9A7fd62939963AAAe5a67)
 
## Expected behaviour tests of CrowdsaleToken
 
- [x] Owner can change the name and symbol of token after deployment. [0x16a980](https://kovan.etherscan.io/tx/0x16a98074d2b3761b3b5e9a2229589c4e2cfc56e080d9ff3a3c6130f634e696b6).
- [x] No one can mint when mint is finalized. [0x086cee](https://kovan.etherscan.io/tx/0x086ceef6162b27aed702fac46b6fac366e18e25393d7b959ac2c0f3df756a9b7)
- [x] Owner can set transfer agent. [0x9118e5](https://kovan.etherscan.io/tx/0x9118e5d510399aaac5fcfc2b89bc3016b7b1816f9b73817a1aaa35eacd4bc598)
- [x] Owner can set upgrade master. [0xa43474](https://kovan.etherscan.io/tx/0xa434745d74d9f9d32e8788014e3a661f6ea47d186fe902338acb8bd74bc60fa2)
- [x] Owner can set release agent.[0xc54151](https://kovan.etherscan.io/tx/0x2a10c3104e177da00f0f674be60b5c21ef2275c10cec40ee8d5c16c1dd59c11d)
- [x] Upgrade Master can set upgrade agent.[0x898467](https://kovan.etherscan.io/tx/0x8984674ba23e5b6c8874a25dd4bfed8b499b0e5544c9ca6f73149377774a1892)
- [x] Approve() is working.[0x7cc010](https://kovan.etherscan.io/tx/0x7cc0107f89d76eb0e274eeb59826b9bbc96807f011b042797b87f24bba931e66)
- [x] TransferFrom() is working.[0x683830](https://kovan.etherscan.io/tx/0x6838308c5ad568d28c300b3c6082129d64bbc25f3ffcedb2e13cb232da1065ba)
- [x] Upgrade master can upgrade token to new token address. [0x02e8ec](https://kovan.etherscan.io/tx/0x02e8ec77419da025a173639da23dd1ca201fc34b86c6d2d942b8ac69a0de07ec)
- [x] Anyone can transfer tokens to the contract.[0xc732eb](https://kovan.etherscan.io/tx/0xc732eb73af1c320fe6a1b1f64f2d61c94abfb635b5101b9943544273a6d471a1)
- [x] Owner can recover/invoke tokens from the contract. [0xd53176](https://kovan.etherscan.io/tx/0xd53176d539854102c01f675ad9c502f9e41c8c82617cb16c9c07f061c5a0a93c)
- [x] Owner can renounce the ownership of the contract. [0x7e18fd](https://kovan.etherscan.io/tx/0x7e18fd7aa11344afcfdffc3680dd8c1088944c5ae793897cb50d2b43deadaf99)
 
## Expected behaviour tests of AllocatedCrowdsale
 
- [x] Owner can halt the crowdsale. [0x64c269](https://kovan.etherscan.io/tx/0x64c26919448bc6ef43b691d54a768f0866dd0bdb2a5a723ff58442d53f8a73f5)
- [x] Owner can unhalt the crowdsale.[0x5dbee7](https://kovan.etherscan.io/tx/0x5dbee701295efca0f3c2cca0921bdb224eeff1d8cf982f0cd477c5223bbc254f)
- [x] Owner can set an address early participant whitelisted. [0x7da501](https://kovan.etherscan.io/tx/0x7da501e15f868e251e932ad577c6a9af81ebc4603412d49c52068dc2423fca9b)
- [x] Owner can set pricing strategy contract.[0x766d06](https://kovan.etherscan.io/tx/0x766d06f28e55c037cd518a58a502c82ed0eead36583c724a01fa64aff209057f)
- [x] Owner can set multisig wallet contract. [0x5dbfb8](https://kovan.etherscan.io/tx/0x5dbfb88cc40a359147e0873fc3838b6cc123cb802a92f3f298691c6ca6c33d56)
- [x] Owner can set finalize agent contract. [0xb85268](https://kovan.etherscan.io/tx/0xdbc16e6b98cd22a2dbcc6c1951eee80e86c6d80d5cf20d4ff7979b7720fee213)
- [x] Owner can transfer ownership to other address. [0xa61eab](https://kovan.etherscan.io/tx/0xa61eab7b4ada4fe06be18770ed90a3d69e833bed52b4bf38244b9e564d32d231)
- [x] Owner can set the end time of crowdsale. [0xcc7b56](https://kovan.etherscan.io/tx/0xcc7b56c570b1dd9ca2b80f1d2426a02dd23020b86916f9c88f7e9a3ecf57e226)
- [x] Transfer agent can preallocate token to any investors. [0x60fbad](https://kovan.etherscan.io/tx/0x60fbad40f1a083961453b6570d0e951e3c997867099b3de25a3363117699ac79)
- [x] Token can be bought when state is Funding. [0xbe1f9b](https://kovan.etherscan.io/tx/0xbe1f9bf6eb5fa95887e9ce3619b58e78dbd970ce2bb25db2093cb36837503cdb)
- [x] Owner can call finalize of the crowdsale. [0xd1cf01](https://kovan.etherscan.io/tx/0xd1cf010590af558666a08d9110cd6bc72cf946c45e0ebdc6dff17094440be222)
 
 
