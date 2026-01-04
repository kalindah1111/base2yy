# base2yy
Tracking Small Dust Transfers
dust = w3.to_wei(0.00001, "ether")
for tx in block.transactions:
    if tx["value"] < dust:
        print("Dust tx:", tx["hash"].hex())
