# 2.1 状态通道（原型机：状态通道）

说起Layer2，很多人可能听说过BTC的闪电网络，以太坊完全可以用相同的技术部署“雷电网络”，它们背后的技术都是“状态通道”。

状态通道使用了多签，允许两个个体之间提前存入一笔资金锁定在智能合约中建立一个内部通道，然后双方可以在通道内进行多笔小额转账，速度极快，成本极低，再在一段时间后用转账证明一次性提款。

[【图：2.1.1 单通道闪电网络.gif】](https://www.notion.so/2-1-1-ef0eb7ad6193495ebc2e65cf8f39797f)

![Untitled](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F1e556aad-d303-4a00-9c75-e281e195fbdf%2FUntitled.png?id=c4904364-3f87-4651-9109-9044adc3b667\&table=block\&spaceId=b1dd17ad-aa83-4faf-9395-5329c519d830\&width=2000\&userId=e298088e-2c93-42ed-870b-b44d950d1eae\&cache=v2)

雷电网络节点越多，整个网络能处理交易的规模也将越大，并且用户能通过多个节点的中转，向更多人转账。

[【图：2.1.2 闪电网络.gif】](https://www.notion.so/2-1-2-030048211df446dfb5e40951ff201c63)

![Untitled](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fa84415ef-393f-4864-8cda-ad1335778022%2FUntitled.png?id=19f1b366-e61a-4b10-a1c2-2226adace016\&table=block\&spaceId=b1dd17ad-aa83-4faf-9395-5329c519d830\&width=2000\&userId=e298088e-2c93-42ed-870b-b44d950d1eae\&cache=v2)

状态通道技术本质上是使用了中心化的节点，用户在链下用“小票”进行付款，积攒了一定量的小票之后，一次性在一层网络中提款。

但这样做存在2个明显的缺点：

1. **无法执行复杂交易**，仅适合最简单的转账交易。
2. **无法给未参与闪电网络的个体发送资金**。（或两个闪电网络节点之间不存在支付通路，同样无法转账）
