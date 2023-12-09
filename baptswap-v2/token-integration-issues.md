---
description: Fee-on-transfer tokens will not function on the future v3 contracts.
---

# Token Integration Issues

### Fee-on-transfer Tokens[​](https://docs.uniswap.org/concepts/protocol/integration-issues#fee-on-transfer-tokens) <a href="#fee-on-transfer-tokens" id="fee-on-transfer-tokens"></a>

Fee-on-transfer tokens will not function with our router future v3 contracts. As a workaround, the token creators may create a customized router. We will not be making a router that supports fee-on-transfer tokens in the future for v3.

However, the fee-on-transfer support will continue on the v2 contracts. The v2 contracts will still be available on Baptswap after the implementation of the future v3 contracts, where the two concepts will work seamlessly alongside each other within the same protocol.
