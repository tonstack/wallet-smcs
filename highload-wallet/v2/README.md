## highload-wallet v2

```
name: highload-wallet
version: 2
revision: -

author: ton <github.com/ton-blockchain>
        akifoq <github.com/akifoq>
```

### Original description:

Heavy-duty wallet for mass transfers (e.g., for cryptocurrency exchanges) accepts orders for up to 254 internal messages (transfers) in one external message this version does not use seqno for replay protection; instead, it remembers all recent query_ids in this way several external messages with different query_id can be sent in parallel.

### Additional description

Initially, the wallet was presented in the [ton repository](https://github.com/newton-blockchain/ton/commit/ecb3e06a06628c358b42ac43c96168d51dbb92e3#diff-c7e0e4eba5dd27ad37d0981cf798d9ecddd2e61f3cf79b5dc7ca60785b2941a5), and then the Fift scripts were finalized by [akifoq](https://github.com/akifoq). 

It is often impossible for one reason or another to send 254 transactions, we recommend sending no more than 100 at a time. 

### How to build

```bash
mkdir auto
func -SPA -o auto/code.fif func/stdlib.fc func/highload-wallet-v2-code.fc
```

### Compiled code

The results are obtained using the `fift -s ./fift/get-code.fif`

Source code BOC in hexadecimal:
```text
B5EE9C724101090100E5000114FF00F4A413F4BCF2C80B010201200203020148040501EAF28308D71820D31FD33FF823AA1F5320B9F263ED44D0D31FD33FD3FFF404D153608040F40E6FA131F2605173BAF2A207F901541087F910F2A302F404D1F8007F8E16218010F4786FA5209802D307D43001FB009132E201B3E65B8325A1C840348040F4438AE63101C8CB1F13CB3FCBFFF400C9ED54080004D03002012006070017BD9CE76A26869AF98EB85FFC0041BE5F976A268698F98E99FE9FF98FA0268A91040207A0737D098C92DBFC95DD1F140034208040F4966FA56C122094305303B9DE2093333601926C21E2B39F9E545A
```

Source code cell human readable:
```text
x{FF00F4A413F4BCF2C80B}
 x{2_}
  x{4}
   x{D030}
   x{2_}
    x{BD9CE76A26869AF98EB85FFC_}
    x{BE5F976A268698F98E99FE9FF98FA0268A91040207A0737D098C92DBFC95DD1F14_}
  x{F28308D71820D31FD33FF823AA1F5320B9F263ED44D0D31FD33FD3FFF404D153608040F40E6FA131F2605173BAF2A207F901541087F910F2A302F404D1F8007F8E16218010F4786FA5209802D307D43001FB009132E201B3E65B8325A1C840348040F4438AE63101C8CB1F13CB3FCBFFF400C9ED54}
   x{208040F4966FA56C122094305303B9DE2093333601926C21E2B3}
```

Source code cell sha256 hash in hex:
```text
9494D1CC8EDF12F05671A1A9BA09921096EB50811E1924EC65C3C629FBB80812
```