# What Are the Differences Between Advanced Mode and Standard Mode for Gas Fee Settings?

The key differences between Advanced Mode and Standard Mode lie in the protocol used and the fee control mechanism:

* **Advanced Mode**:\
  This mode adopts the EIP-1559 protocol, which uses a new fee calculation method. It allows for faster transaction confirmation and theoretically reduces fee volatility. Advanced Mode is ideal for users requiring high-priority confirmations. Users can customize **Max Fee** (maximum fee) and **Max Priority Fee** (priority fee) for precise control.
* **Standard Mode**:\
  Based on the traditional gas fee structure, this mode requires manual input of **Gas Price** and **Gas Limit**. It offers less flexibility but suits users unfamiliar with EIP-1559 or those who prefer the traditional setup.

Compared to Standard Mode, Advanced Mode provides more cost savings and stable performance, while Standard Mode continues the conventional fee-setting approach.
