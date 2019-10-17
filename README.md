# MAN Box

Matrix AI Network block chain contracts default config and man address support
## Init man contract
    cd {yourcontractdir}
    truffle unbox https://github.com/MatrixAINetwork/manbox.git
## truffle-config
##### Each network properties add type,dryRun,skipDryRun setting like this:
    development: {
        type = "matrix",
        skipDryRun: true,
    }
#### Add manUtils.sol support
###### Convert address to man address(string)
    function toMan(address _addr)  public pure returns (string)
###### Convert man address(string) to address
    function toAddress(string _manAddr) public pure returns(address)
