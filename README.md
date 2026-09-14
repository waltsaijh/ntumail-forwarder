# NTUMail 自動轉寄

## 功能

透過 Github Action 每十分鐘將新郵件從 NTUMail 轉寄到指定信箱。

## 設定

1. 複製此 Template，名稱隨意
2. 進入新打開的 Repository
3. 在導覽列 (最上方那排) 點選 Settings => Secrets & Variables => Actions
4. 新增三個 Secrets，可防止帳密外洩
    - `NTUMAIL_ADDRESS`: 你的 NTUMail 信箱 (...@ntu.edu.tw)
    - `NTUMAIL_PASSWORD`: 你的密碼
    - `FORWARDING_ADDRESSES`: 目標轉寄信箱，超過一個則用 `, ` 隔開
5. 完成!

## 補充事項

請注意，此應用只會轉寄新進入的郵件，故啟動前的所有郵件均會被忽略，而不會被轉寄至其他信箱。
