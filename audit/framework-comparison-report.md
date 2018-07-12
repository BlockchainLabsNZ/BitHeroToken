## Framework used

Generally, this project is using a solidity framework [TokenMarket ico](https://github.com/TokenMarketNet/ico), the latest version currently. After comparison, 12/19 of all contracts stay the same.See details from the [list](https://gist.github.com/ryu9827/cfe97495f4d2186606c1bf766d8220d1). However, some contracts have slight modifications from original framework, which are listed below: 

* AllocatedCrowdsaleMixin.sol
```
//Line 41-46, add an if statement
...
else{
    if (weiAmount < 10**17) {
        return true;
      }
      else {
        return false;
      }
    }
...
```

* Imported path in some contracts are changed from `zeppelin` to `zeppelin-solidity`. That is necessary due to the name changing of `zeppelin`.<br>

```
//FractionalERC20.sol, line 9
import "zeppelin-solidity/contracts/token/ERC20/ERC20.sol";
```

```
//Haltable.sol, line 9
import "zeppelin-solidity/contracts/ownership/Ownable.sol";
```

```
//MintableToken.sol, line 7
import "zeppelin-solidity/contracts/token/ERC20/ERC20.sol";
```

```
//Recoverable.sol, line 9-10
import "zeppelin-solidity/contracts/ownership/Ownable.sol";
import "zeppelin-solidity/contracts/token/ERC20/ERC20Basic.sol";
```

```
//StandardTokenExt.sol, line 9
import "zeppelin-solidity/contracts/token/ERC20/StandardToken.sol";
```

```
//UpgradeableToken.sol, line 9
import "zeppelin-solidity/contracts/token/ERC20/ERC20.sol";
```
* All JavaScript scripts in the repo seems self-developed.