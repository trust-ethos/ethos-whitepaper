# Contracts and Ownership

Smart contracts are managed by multisigs in a [Safe](https://app.safe.global/home?safe=base:0xB4a9bc5fb037eBd805a405F2b53cFadF4bCB4774).&#x20;

`0xB4a9bc5fb037eBd805a405F2b53cFadF4bCB4774` has owner permissions of the smart contracts and requires 3 of 5 signatures to manage the Ethos smart contracts

| "Owner" wallets (3/5 multi-sig)              |
| -------------------------------------------- |
| `0xF66F66Bd3f35dba8a49866e42A7A9666fcAf9e42` |
| `0x2a721196C5ea068EE17Afe3A70ce68746171De0d` |
| `0x88ADa959a9dA289abe667362caF02755F34C552D` |
| `0xefa91bD0c7a608B41A300Ae1C3a9f0AA16A41726` |
| `0x7437c2BC96e062C009B8885B7c9ACa8F77302682` |

Ethos also uses an Admin permission and separate multisig for non-withdraw operations. This is also protected by a multi-sig [Safe](https://app.safe.global/home?safe=base:0x72F04d999E12D456FE7eE0Acaa345124A081018D) and requires 2 of 4 signatures to manage non-withdraw operations. The address for this Safe is `0x72F04d999E12D456FE7eE0Acaa345124A081018D`

| "Admin" wallets (2/4 multi-sig)              |
| -------------------------------------------- |
| `0xF66F66Bd3f35dba8a49866e42A7A9666fcAf9e42` |
| `0x88ADa959a9dA289abe667362caF02755F34C552D` |
| `0xefa91bD0c7a608B41A300Ae1C3a9f0AA16A41726` |
| `0x7437c2BC96e062C009B8885B7c9ACa8F77302682` |

Lastly, Ethos has a Bank wallet where all protocol fees are sent. It is also protected by a [Safe](https://app.safe.global/home?safe=eth:0x9C98258da66Ed095948CE4774e541C9FE978e946) behind 2 of 3 multi-sig. The address for this Safe is `0x9C98258da66Ed095948CE4774e541C9FE978e946`&#x20;

| "Bank" wallets (2/3 multi-sig)               |
| -------------------------------------------- |
| `0x5f88E65DC9baC9C74825B67f19f0FC8006A30336` |
| `0x6dcf5CB170CfBb06e7ae410B8f3Fb3E6afbBB35f` |
| `0x8d37e6cb3C4d4e50B0a3870d3346485E17775e45` |

Here is a list of all Ethos smart contracts:

<table data-full-width="true"><thead><tr><th>Contract Name</th><th>Address</th><th data-type="content-ref">Basescan Link</th></tr></thead><tbody><tr><td>ContractAddressManager</td><td><code>0xC31252d6bE0252018F1b12deF25f6582dB0f3E9a</code></td><td><a href="https://basescan.org/address/0xC31252d6bE0252018F1b12deF25f6582dB0f3E9a">https://basescan.org/address/0xC31252d6bE0252018F1b12deF25f6582dB0f3E9a</a></td></tr><tr><td>EthosAttestation</td><td><code>0x27499D9A439D1c7B4538f247625cc7aA159D3c14</code></td><td><a href="https://basescan.org/address/0x27499D9A439D1c7B4538f247625cc7aA159D3c14">https://basescan.org/address/0x27499D9A439D1c7B4538f247625cc7aA159D3c14</a></td></tr><tr><td>EthosDiscussion</td><td><code>0x2820b3aB3543ADB80810f11F2651f0DD9A04E801</code></td><td><a href="https://basescan.org/address/0x2820b3aB3543ADB80810f11F2651f0DD9A04E801">https://basescan.org/address/0x2820b3aB3543ADB80810f11F2651f0DD9A04E801</a></td></tr><tr><td>EthosProfile</td><td><code>0x209820B843900Ef77BD639455cDE15F38A252a36</code></td><td><a href="https://basescan.org/address/0x209820B843900Ef77BD639455cDE15F38A252a36">https://basescan.org/address/0x209820B843900Ef77BD639455cDE15F38A252a36</a></td></tr><tr><td>EthosReview</td><td><code>0x6D3A8Fd5cF89f9a429BFaDFd970968F646AFF325</code></td><td><a href="https://basescan.org/address/0x6D3A8Fd5cF89f9a429BFaDFd970968F646AFF325">https://basescan.org/address/0x6D3A8Fd5cF89f9a429BFaDFd970968F646AFF325</a></td></tr><tr><td>Reputation Market </td><td><code>0xC26F339F4E46C776853b1c190eC17173DBe059Bf</code></td><td><a href="https://basescan.org/address/0xC26F339F4E46C776853b1c190eC17173DBe059Bf">https://basescan.org/address/0xC26F339F4E46C776853b1c190eC17173DBe059Bf</a></td></tr><tr><td>EthosVote</td><td><code>0x89e6Ff2Ce8318433E011d848D8a35FbFeE60c2Ed</code></td><td><a href="https://basescan.org/address/0x89e6Ff2Ce8318433E011d848D8a35FbFeE60c2Ed">https://basescan.org/address/0x89e6Ff2Ce8318433E011d848D8a35FbFeE60c2Ed</a></td></tr><tr><td>EthosVouch</td><td><code>0xD89E6B7687f862dd6D24B3B2D4D0dec6A89A6fdd</code></td><td><a href="https://basescan.org/address/0xD89E6B7687f862dd6D24B3B2D4D0dec6A89A6fdd">https://basescan.org/address/0xD89E6B7687f862dd6D24B3B2D4D0dec6A89A6fdd</a></td></tr><tr><td>InteractionControl</td><td><code>0x0A31c99B8eDD563CDF01534a82956Eda5CDB4CE5</code></td><td><a href="https://basescan.org/address/0x0A31c99B8eDD563CDF01534a82956Eda5CDB4CE5">https://basescan.org/address/0x0A31c99B8eDD563CDF01534a82956Eda5CDB4CE5</a></td></tr><tr><td>SignatureVerifier</td><td><code>0x78a32a705bFc1600e0A2E056316E44877BDa7f57</code></td><td><a href="https://basescan.org/address/0x78a32a705bFc1600e0A2E056316E44877BDa7f57">https://basescan.org/address/0x78a32a705bFc1600e0A2E056316E44877BDa7f57</a></td></tr><tr><td>EthosSlash</td><td>0xB2C41DebA270E1eA6abBe0e2fA70432630634a59</td><td><a href="https://basescan.org/address/0xB2C41DebA270E1eA6abBe0e2fA70432630634a59">https://basescan.org/address/0xB2C41DebA270E1eA6abBe0e2fA70432630634a59</a></td></tr></tbody></table>

