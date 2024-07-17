# hive-keychain-bundlejs
Bundle JS file for frontends to interact with the [Hive Keychain](https://github.com/hive-keychain/hive-keychain-extension) extension installed in browsers.

**Example**
```
<script src="bundle.js"></script>

// Example interaction with Hive Keychain
window.hive_keychain.requestSendToken(to, symbol, quantity, memo, response => {
    if (response.success) {
        console.log("Transfer successful:", response);
        alert("Transfer successful!");
        // Handle success scenario
    } else {
        console.error("Transfer failed:", response);
        alert("Transfer failed: " + response.error);
        // Handle failure scenario
    }
});
```
