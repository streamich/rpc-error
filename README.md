# RPC errors

A class for handling RPC errors. Instances of `RpcError` are assumed to be
public errors, which are safe to expose to the client.

```ts
import {RpcError} from 'rpc-error';

const error = RpcError.notFound();
```
