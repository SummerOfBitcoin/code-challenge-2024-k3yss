- Remove invalid blocks
  - How do you remove invalid blocks?
    - 




I'll keep appending invalid transactions here. current list:

    bad-txns-vout-empty

how to invalidate transactions:

    check if transaction id calculation logic is correct in json-to-tx-object.py (my main concern! 🚩)
    Run using python3 json-to-tx-object.py mempool/0e71cf1ed24c5354e48846486e1075d5aa37f437bcc6dedf57022be0657cfcef.json
    See if output displayed at very end - "hash of comput txid" matches the filename (in this case: 0e71cf1ed24c5354e48846486e1075d5aa37f437bcc6dedf57022be0657cfcef)
    Copy transaction into new file (ex: bad-xxxxx.json)
    Then invalidate the transaction
    Print hash of newly computed txid and rename file


- How to do it in reference to grokkking bitcoin?
  - [claude-clarity](calude-clarity.md)


- Signature verification:
  -  https://sahaflores.medium.com/public-private-keys-generation-signature-verification-using-ecdsa-algorithm-51cb4f656257

-  https://cryptobook.nakov.com/digital-signatures/ecdsa-sign-verify-messages

- verifyECDSAsecp256k1

- https://github.com/bitcoin/bips/blob/master/bip-0143.mediawiki