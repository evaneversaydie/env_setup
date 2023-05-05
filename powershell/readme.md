

# Useage
- `Microsoft.PowerShell_profile.ps1`: 設定檔。
- `My_theme.omp.json`：修改後的主題。
    - 想要有:
        - 使用者
        - 主機名稱
        - 執行時間/日期
        - GPU CPU
        - 目前的檔案位置(可分層標示也可以不用)
        - 是否為git
    - 本次修改結果
        - 原始檔案:qiuick-term
        - 增加
            - 主機名稱
            - 修改時間格式
            - GPU/CPU:(參考wholesplace 主題的寫法)
            - 在使用者後面新增尖隔:可以善用<transparent,#516BEB>\ue0b2</>
                - ">" 符號字元: \ue0b0 \ue0b1 \ue0b2
                - style: psline(segment開始結尾相同)、diamond(前後不同)....
                - invert_powerline:ture (顏色顛倒)
            - `搜尋"\\":看註解`

## TODO
- auto compelete (PSReadLine設定在畚箕安裝時有出現問題)
- 自動安裝設定的SCRIPT檔
