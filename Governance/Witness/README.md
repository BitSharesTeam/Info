
https://roelandp.nl/bitshareswitnesslog/  вот табличка котировок !!!

_________________________________________________________________________________________________________________________________

Нужно с серваками ещё разобраться
выбрать хорошие и недорогие
https://www.worldstream.nl/en/dedicated/premium/info

_________________________________________________________________________________________________________________________________

вот пример как мы запостим на форуме чтобы люди голосовали за наших витнессов
нужно еще провести анализ других постов на форуме
https://bitsharestalk.org/index.php/topic,24017.msg304832.html

_________________________________________________________________________________________________________________________________

Гид по созданию witness ноды
https://bitsharestalk.org/index.php?topic=23925.0

_________________________________________________________________________________________________________________________________

Тестовая сеть BitShares (тестовая биржа/кошелек)
это тестовые битшары где мы и будем сначала запускать наши серваки
вернее для тестовой сети наши серваки будем запускать чтобы всем показать, 
что мы реально справляемся с этой работой и на нас можно положиться и мы не зря 
получаем вознаграждение за каждый новый проверенный и 
подписанный блок во всей цепочке блоков битшар 
за каждый новый созданный блок 1 BTS вознаграждение (примерно 30 000 блоков 1 witness в месяц создает)
https://testnet.bitshares.eu/

_________________________________________________________________________________________________________________________________

витнессы - это создатели новых блоков во всей цепочке блоков
типа как майнеры в Биткоине
только майнить биткоин любой может, а тут только через голосование тебе разрешают официально майнить
и получать вознаграждение
проверяют блоки и создают блоки

_________________________________________________________________________________________________________________________________

witness_node combines several functions:
1. Apply incoming blocks
2  Apply incoming transactions for validation
3. Generate blocks (witness only)
4. Respond to API requests

All of these interfere with each other!

_________________________________________________________________________________________________________________________________

Just thought of this too: have we forgotten why we have a role called "witness"? They are called that to insulate witnesses (from liability, accusations of price manipulation or favoritism of feed supliers for starters), to be independant observers and reliable publishers of those observations, be they about feeds or missed blocks or anything else that could be independently verified by multiple, distributed entities, such as other witnesses.


1. The settlement price (SP), given as bitUSD/BTS - someone who owns bitUSD can request settlement and will have their bitUSD converted to BTS 24 hours later, at the settlement price.

2. The margin call ratio (MCR) - in order to borrow x bitUSD you have to provide at least (x*MCR/SP) BTS as collateral. If the settlement price goes down, at some point SP/MCR will drop below your debt/collateral ratio, and you will be margin called.

3. The maximum short squeeze ratio (MSSR or MSQR) - a debt position that is margin called will automatically try to buy bitUSD from the market, paying up to MSSR/SP BTS per bitUSD.

https://steemit.com/bitshares/@cyrano/how-bitshares-protects-mpas-using-margin-calls

http://docs.bitshares.org/bitshares/user/mpa.html

_________________________________________________________________________________________________________________________________

http://docs.bitshares.org/bitshares/tutorials/publish-feed.html

```
{
  "publisher": "1.2.0",
  "asset_id": "1.3.0",
  "feed": {
    "settlement_price": {
      "base": {
        "amount": 0,
        "asset_id": "1.3.0" },
      "quote": {
        "amount": 0,
        "asset_id": "1.3.0" }
    },
    "maintenance_collateral_ratio": 1750,
    "maximum_short_squeeze_ratio": 1200,
    "core_exchange_rate": {
      "base": {
        "amount": 0,
        "asset_id": "1.3.0" },
      "quote": {
        "amount": 0,
        "asset_id": "1.3.0" }
    }
  }
 }
 ```
_________________________________________________________________________________________________________________________________

# Buy Servers info

https://www.worldstream.nl/en/dedicated/custom/info

https://www.hetzner.com/?country=us
Intel® Core™ i7-8700 Hexa-Core Coffee Lake 2 x 512 gb NVMe SSDs in RAID 64GB ram

https://bitsharestalk.org/index.php?topic=24046.msg305206#msg305206
https://bitsharestalk.org/index.php/topic,24005.0.html
https://bitsharestalk.org/index.php/topic,23925.0.html

_________________________________________________________________________________________________________________________________

## ./programs/cli_wallet/cli_wallet --server-rpc-endpoint=wss://node.bitshares.eu
### Main Chain ID: 4018d7844c78f6a6c41c6a552b898022310fc5dec06da467ee7905a8dad512c8

## ./programs/cli_wallet/cli_wallet --server-rpc-endpoint=wss://node.testnet.bitshares.eu
## ./programs/cli_wallet/cli_wallet --server-rpc-endpoint=wss://node.testnet.bitshares.ws
### Test Chain ID: 39f5e2ede1f8bc1a3a54a7914414e3779e33193f1f5693510e73cb7a87617447

_________________________________________________________________________________________________________________________________

## Price Feed publishing

https://github.com/cogutvalera/bitshares-pricefeed

_________________________________________________________________________________________________________________________________
