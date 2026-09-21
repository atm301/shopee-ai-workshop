# AI 電商實戰工作坊｜學員站

蝦皮大學 × 圭話行銷；講師 何佳勳（小圭）。2026/09/22（二）13:00-16:00，蝦皮總部 9F。單頁 HTML、GitHub Pages。

- **index.html**：桌號（第 1 到 7 桌）＋暱稱報到、8 分頁（開始／素材／決策／流程／提示詞／工具／上傳／帶走）、8 題現場互動（含五題互動題投完即看解答）、開場與收尾的時間差計算機、16 張提示詞一鍵複製直開 ChatGPT／Gemini、36 個工具連結（自家網域全帶 UTM）、分組作業上傳（文字或圖片，append-only 多版全留）、各桌即時分數、7 天行動清單與列印卡。
- **admin.html**：後台（noindex）上傳牆／計分（簡報三種加分預設按鈕）／投票（標示正解）／學員，全部可匯出 CSV。
- **board.html**：投影用各桌即時積分，每 6 秒更新。

後端：共用 Supabase `lw_line_students`（course=`shopee-ai-workshop`，唯一鍵 course+cohort+code）＋ `lw_workshop_submissions`（上傳，append-only）＋ `lw_workshop_scores`（加減分流水帳）＋ `lw-workshop` storage bucket（10MB、圖片 MIME、不可覆蓋，前端會先縮圖成 JPEG）。

⚠️ 課程網站短網址 `atmtut.com/0922`（簡報 p9 的 QR）目前指向 ecom.atmarketing.tw，要在 Lihi 後台改成本站網址。
