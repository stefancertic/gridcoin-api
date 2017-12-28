# gridcoin-api
Classes to communicate with GridCoin Wallet via PHP used by gridcoins.org

Usage:

require_once('main.php');
$gridcoin = new Gridcoin('username','password');


API Calls:

Create new address and account if not exsist

$address =$gridcoin->getaccountaddress($username);

Get account balance:

$gridcoin->getbalance('accountname');

Dump account private key:

$gridcoin->dumpprivkey($gridcoin->getaccountaddress('account name'));
