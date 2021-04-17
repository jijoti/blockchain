Run your http server with cmd `python blockchain.py`.

Add a transaction with:
`
curl -X POST -H "Content-Type: application/json" -d '{
 "sender": "d4ee26eee15148ee92c6cd394edd974e",
 "recipient": "someone-other-address",
 "amount": 5
}' "http://localhost:5000/transactions/new"
`

Mine a block with:
`
curl -X GET "http://localhost:5000/mine"
`

Get the chain with:
`
curl -X GET "http://localhost:5000/chain"
`
