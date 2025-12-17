# 交易加速及取消

当交易因矿工费太低而无法完成时，用户可以进行加速或取消交易的操作。请注意，此功能仅适用于BTC和ETH系列的加密货币。

<figure><img src="https://0xcregis.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=OTY2MTE0ZjhhMzcwMzE4ODBjNWNkNGZiMDIzNjVjZWRfRmllcnpjOXBhbDBkOEFwWmpTak9hZnZiNGdCdE1makpfVG9rZW46TmtJTGJZY29lb2lYTzR4VHlWSmxha3VuZ1lmXzE3NjU5NjcwODM6MTc2NTk3MDY4M19WNA" alt=""><figcaption></figcaption></figure>

## ETH系列 <a href="#eth-xi-lie" id="eth-xi-lie"></a>

### 交易加速 <a href="#jiao-yi-jia-su" id="jiao-yi-jia-su"></a>

在待确认的交易内点击“加速”。

![](https://0xcregis.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=ZDkwZWJjNjMyMThhOTQ2YzhlYjljZGY2MGZiOTE5MWVfWWxjUDBNUzA0ZmtsNUdEYzBUVUNhQXFla2pYOTEwMHJfVG9rZW46UnRuRWJjRmFJb3I5ODJ4SXd1aWxkZzNCZ2pGXzE3NjU5NjcxMDM6MTc2NTk3MDcwM19WNA)

点击后如果该代币有大于1条待确认交易，会弹出交易加速列表页面，请根据 Nonce 从小到大依次操作，点击「加速」，如果该代币只有 1 条待确认交易，则跳过该步骤。

<figure><img src="https://0xcregis.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=NmQxOGE4MzlkNWQ1MGZjZmQ1NjZjN2QzOTBjZTY3YzZfZldwbGVPNlRMaEJGeERPWGNiY2FBVE1WWDF4V2NLcW9fVG9rZW46SDdBQWJvendEb3NLUXB4QTlkNWxROExSZ3VmXzE3NjU5NjcxMjA6MTc2NTk3MDcyMF9WNA" alt=""><figcaption></figcaption></figure>

点击「加速」后会展开交易详情，同时提供加速矿工费的选项，点击后可以选择不同的矿工费选项，用户也可以自定义矿工费。

<figure><img src="https://0xcregis.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=M2Q4YjRhZmFjM2RiMThkMjdhZGM3MTExOWI4NGUwZjlfbml1Z0ZSTWZySVEyS2dYZ2FmZ0E0dVNNcWpaNWtDWmFfVG9rZW46QTFDbWIxV2Jib2lWdDV4ZjdYaGw0WVhQZ296XzE3NjU5NjcxNDA6MTc2NTk3MDc0MF9WNA" alt=""><figcaption></figcaption></figure>

自定义的矿工费设置分为<mark style="color:green;">**高级模式**</mark>和<mark style="color:green;">**普通模式**</mark>：

* **高级模式**：采用了<mark style="color:green;">**EIP-1559**</mark>协议，这种模式利用新的费用计算方式，使得交易的确认速度更快，同时在理论上相比普通模式减少矿工费用。在高级模式中，用户可以自定义Max Fee（最大费用）和Max Priority Fee（优先费用），以实现精准控制，确保交易优先进行。这种模式特别适合需要高优先级确认且希望节省费用的用户。
* **普通模式**：基于传统的矿工费结构，用户可以设置Gas Price和Gas Limit来决定交易费用。此模式逐渐被EIP-1559协议取代，但仍适合对新模式不熟悉或希望保持传统费用设置的用户。

<figure><img src="../../.gitbook/assets/image (718).png" alt=""><figcaption></figcaption></figure>

设置完成后，点击确认并进行身份认证。

<figure><img src="https://0xcregis.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=YTM2NDdkYTdjOTQzNTFlYmVkYTdmMjQ1OTA5ODdmZmRfODg0RVJTRjhHd1hnZjhXY1l5UjhmNDVJUFRHb0xnaUpfVG9rZW46QjU2VGJBU3pOb3JZQW54OHpFTGw4MHd1ZzJjXzE3NjU5NjcxODI6MTc2NTk3MDc4Ml9WNA" alt=""><figcaption></figcaption></figure>

认证完成后可见到加速中的标签

<figure><img src="https://0xcregis.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=MWIyNDNiNTIyNzRkOGMwNzJiNDM3YThkZjA3Y2Q4NjBfM1pJR084dTEzUkttRVpvV3p5RngwWG1vT3VjeFluTnZfVG9rZW46V0EwOWJYU0x1b0pXbG94RzlQb2xiTlp5Z1VlXzE3NjU5NjcyMTA6MTc2NTk3MDgxMF9WNA" alt=""><figcaption></figcaption></figure>

加速完成后可看到已加速的标签。<img src="https://support.cregis.com/~gitbook/image?url=https%3A%2F%2F3200384756-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FPoazW59IJbERNbp3S6uz%252Fuploads%252F50YfgwttMldHGmab9kDT%252Fimage.png%3Falt%3Dmedia%26token%3Df2202a51-0a77-4db2-a745-53edb7cd2454&#x26;width=55&#x26;dpr=4&#x26;quality=100&#x26;sign=5ab4c3d&#x26;sv=1" alt="" data-size="line">

<figure><img src="https://0xcregis.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=ZjIxZGM0ZDEwNWU1NGNhNDI4YmUwNDJhYTNjNjYzZTNfWHZkYTcyb2l3dmxxc3lmZG5lTmZvNmVya2R1V0h5MkxfVG9rZW46Tnd4NGJ2TUlhb1BSbld4QVdaNGw1NTJ2Z25kXzE3NjU5NjcyMjM6MTc2NTk3MDgyM19WNA" alt=""><figcaption></figcaption></figure>

### 交易取消 <a href="#jiao-yi-qu-xiao" id="jiao-yi-qu-xiao"></a>

於待確認的交易內點擊「取消」

<figure><img src="https://0xcregis.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=NGY5MGRkNDI5OTBhNzJjOGI5Nzc1YzllMDUyY2U5YzhfU2xtN0hnVTFtdDluMGJzOHVKaDRsdXlSelRxV2VjN0VfVG9rZW46QVJjY2JKekpvb3dQR2R4R2xOQ2xUNjR5Z2dnXzE3NjU5NjcyNDA6MTc2NTk3MDg0MF9WNA" alt=""><figcaption></figcaption></figure>

点击后如果该代币有大于1条待确认交易，会弹出交易取消列表页面，请根据 Nonce 从小到大依次操作，点击「取消」，如果该代币只有 1 条待确认交易，则跳过该步骤。

<figure><img src="https://0xcregis.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=MzkyYTkyNzU1Y2JkZmRkMmZkMjZiN2JkOWRiMWEyOWFfQ1U5cFNab3lFVjd3bkE5bUVkaFE1WDMwOVlrcExGYWhfVG9rZW46Q3FHVmJtajU5b1N4OUh4bGUzT2xIdU9mZ0llXzE3NjU5NjcyNjM6MTc2NTk3MDg2M19WNA" alt=""><figcaption></figcaption></figure>

点击「取消」后会展开交易详情，同时有取消矿工费的选项，点开可选择不同的矿工费选项，用户也可以自定义矿工费。由于取消交易时重发一条金额为$0 的交易，因此这里的发送金额显示为0。

<figure><img src="https://0xcregis.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=YmExMjNlYjZkM2QwMDI4M2I2ZDEyNDQ2YTFiMDY4OTVfWTZPTmJaeFlJTk1TcG00dmROOEE3RXZHTHlFRm9yVDZfVG9rZW46RW82Z2JqVG5qb3IxREh4QmdJNmxDVGpNZzliXzE3NjU5NjcyODE6MTc2NTk3MDg4MV9WNA" alt=""><figcaption></figcaption></figure>

設置完成後進行身份認證。

<figure><img src="../../.gitbook/assets/image (245).png" alt=""><figcaption></figcaption></figure>

成功取消後用戶介面上會看到兩條交易記錄，金額為0的那條是取消請求的交易記錄，而前一條記錄則會有「已取消」的標籤。

### BTC系列 <a href="#btc-xi-lie" id="btc-xi-lie"></a>

#### 交易加速 <a href="#jiao-yi-jia-su-1" id="jiao-yi-jia-su-1"></a>

於待確認的交易內點擊「加速」

<figure><img src="../../.gitbook/assets/image (246).png" alt=""><figcaption></figcaption></figure>

點擊後會有交易詳情展開，同時有加速礦工費的選項，點開可選擇不同的礦工費選項，用戶亦可以自定義礦工費。

<figure><img src="../../.gitbook/assets/image (247).png" alt=""><figcaption></figcaption></figure>

自定義礦工費可以讓用戶設定Gas Price及Gas Limit，系統亦會自動估算礦工費作參考。

<figure><img src="../../.gitbook/assets/image (248).png" alt=""><figcaption></figcaption></figure>

設定完成後按確定並進行身份認證。

<figure><img src="../../.gitbook/assets/image (249).png" alt=""><figcaption></figcaption></figure>

認證成功後便可以看到「加速中」的標籤，如等待時間過久用戶亦可選擇再加速調礦工費。

<figure><img src="../../.gitbook/assets/image (250).png" alt=""><figcaption></figcaption></figure>

加速完成後可看到已加速的標籤<img src="https://support.cregis.com/~gitbook/image?url=https%3A%2F%2F3200384756-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FPoazW59IJbERNbp3S6uz%252Fuploads%252F50YfgwttMldHGmab9kDT%252Fimage.png%3Falt%3Dmedia%26token%3Df2202a51-0a77-4db2-a745-53edb7cd2454&#x26;width=55&#x26;dpr=4&#x26;quality=100&#x26;sign=5ab4c3d&#x26;sv=1" alt="" data-size="line">。

<figure><img src="../../.gitbook/assets/image (254).png" alt=""><figcaption></figcaption></figure>

#### 交易取消 <a href="#jiao-yi-qu-xiao-1" id="jiao-yi-qu-xiao-1"></a>

於待確認的交易內點擊「取消」。

<figure><img src="../../.gitbook/assets/image (251).png" alt=""><figcaption></figcaption></figure>

點擊後會有交易詳情展開，同時有取消礦工費的選項，點開可選擇不同的礦工費選項，用戶亦可以自定義礦工費。 由於BTC取消交易是通過手續費替換（Replace-by-fee，RBF）的方式，發送一筆與之前相同（UTXO）的交易，因此這裡的**金額顯示為0**。

<figure><img src="../../.gitbook/assets/image (252).png" alt=""><figcaption></figcaption></figure>

設置完成後可進行身份認證。

<figure><img src="../../.gitbook/assets/image (255).png" alt=""><figcaption></figcaption></figure>

成功取消後用戶介面上會看到兩條交易記錄，金額為0的那條是取消請求的交易記錄，而前一條記錄則會有「已取消」的標籤。

<figure><img src="../../.gitbook/assets/image (253).png" alt=""><figcaption></figcaption></figure>
