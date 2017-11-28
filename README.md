# Ruby blockchain

Simple implementation of a blockchain with transaction logic and a script to simulate network activity.

Following a  [presentation](https://www.youtube.com/watch?v=3aJI1ABdjQk&feature=youtu.be&t=17m23s) by Haseeb Qureshi

## Run

```
cd ruby_blockchain
ruby token.rb PEER_PORT
```

For every new peer you want to add to the network
```
ruby token.rb PEER_PORT MY_PORT
```

We expose an endpoint `/send_money` to create transactions
```
pry
Client.send_money(FROM_PORT, TO_PORT, amount)
```
