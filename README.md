# RPC errors

A class for handling RPC errors. Instances of `RpcError` are assumed to be
public errors, which are safe to expose to the client.

```ts
import {RpcError} from 'rpc-error';

const error = RpcError.notFound();
```

Create a public "internal error":

```ts
const publicError = RpcError.from(privateError);
```

Create error using a custom code:

```ts
const error = RpcError.create('CUSTOM_ERROR_CODE');
```
