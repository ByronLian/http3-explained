# 快速交握

QUIC 提供 0-RTT 和 1-RTT 的連接建立，這意味著 QUIC 在最佳情況下不需要任何額外往返時間便可以建立新連接。
兩者中較快的 0-RTT 僅在兩主機之間建立過連接且緩存了該連接的 "秘密"（secret）時才能使用。

## 早期資料（Early data）

QUIC 允許客戶端在 0-RTT 的情況下直接攜帶資料。這使得客戶端能儘早向對方傳送資料，當然也使得伺服器端能更快地發回響應。