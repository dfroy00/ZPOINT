# AI 圖檔 prompt 對照（codex-image 產出）

> **範圍**：僅封面主視覺 + 好壞照片對比示意等**環境圖 / 情境圖**；LINE 對話與 LIFF UI **一律真截圖或 HTML mock**，絕不 AI 生成。
> **紀律**：見 `../content_draft.md` §F。禁止中文字 / 品牌商標 / 人物臉部 / 車牌 / 門牌 / 真 QR / UI 元素。
> **重生**：若原檔遺失，直接複製本檔對應 prompt 進 codex-image 重跑即可（key = 圖檔用途）。
> **產出日期**：2026-07-09

---

## cover_hero.png · 封面主視覺（頁 1）

**用途**：簡報第 1 頁封面右半視覺，暖綠調 4:5 直式版面。

**prompt**（英文）：

```
A warm, welcoming photograph of a person's hand holding a smartphone,
capturing a clean empty transparent plastic water bottle placed on a light wooden desk.
Bright natural office daylight from the left, soft shadows, shallow depth of field.
Slight bokeh of green plants in the background.
Warm off-white and sage green color palette.
Realistic, photographic, no text, no watermark, no logos, no brand marks,
no visible faces, no license plates, no house numbers, no QR codes,
no UI overlays or phone screen content (screen shows blurred generic camera viewfinder only),
clean and minimal composition, editorial quality.
Aspect ratio 4:5 portrait.
```

**禁止項**：中文字、任何文字、品牌商標（大豐 / 全聯 / LINE / 環境部）、人物臉部、車牌、門牌、真 QR code、LINE / LIFF UI 疊加。

---

## tip_good.png · 好照片示意（頁 9 上半）

**用途**：簡報第 9 頁「拍照訣竅 · 好照片 ✓」示意圖。

**prompt**（英文）：

```
A well-lit photograph of a single empty recycling item on a plain neutral surface,
brightly and evenly illuminated by natural daylight,
sharp focus, clean background, the object clearly centered and fully in frame,
warm off-white and sage green color palette.
Realistic, photographic, no text, no watermark, no logos, no brand marks,
no visible faces, no license plates, no house numbers, no QR codes,
no UI overlays, editorial quality.
Aspect ratio 4:3 landscape.
```

**禁止項**：同 `cover_hero.png`。

---

## tip_bad.png · 壞照片示意（頁 9 下半）

**用途**：簡報第 9 頁「拍照訣竅 · 壞照片 ✗」對比示意圖。

**prompt**（英文）：

```
A poorly-lit photograph showing multiple mixed recycling items cluttered together
on a messy surface, dimly and unevenly lit, out of focus and slightly blurry,
the objects are hard to distinguish from each other, cluttered composition,
muted desaturated color palette, low contrast.
Realistic, photographic, no text, no watermark, no logos, no brand marks,
no visible faces, no license plates, no house numbers, no QR codes,
no UI overlays.
Aspect ratio 4:3 landscape.
```

**禁止項**：同 `cover_hero.png`。

---

## 產出 / 重生指令範例

若需重跑，透過 codex-image skill：

```
/codex-image 產出 cover_hero.png，prompt 見 docs/promo/employee_collection_intro/assets/prompts.md
```

或直接把上述 prompt block 複製、指定輸出路徑到 `docs/promo/employee_collection_intro/assets/`。
