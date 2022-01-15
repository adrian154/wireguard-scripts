# wireguard-scripts
Some cursed scripts for wireguard management.

# Usage

To start, configure `ListenPort` and `PrivateKey` in `wg0.conf` and `PublicKey` and `Endpoint` in user-config.template.

Now, you're ready to add peers:

```
./add-peer.sh chuck 10.0.0.2
```

Peer configurations are stored to `configs/` automatically. To remove a peer just get rid of them from `wg0.conf`. This script does not recreate the interface for you, and unless you do that changes will not be applied.

# License

All these scripts are in the public domain.
