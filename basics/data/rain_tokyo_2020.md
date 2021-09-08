# Precipitation, Tokyo 2020

Source: 気象庁
- ホーム > 各種データ・資料 > 過去の気象データ・ダウンロード
- parameters:
  - place: Tokyo
  - data:
    - the total amount of the day
    - the max amount in 60 min of the day
  - date range:
    - from: May 1, 2020
    - to: September 30, 2020

Data file format
- rows:
  - 1 to 6: headers (encoded in Shit JIS)
  - 7 to 159: observations
- columns:
  - separator: `,`
  - A: date
    - yyyy/m/d
  - B: the total amount of the day (mm)
    - float
  - C: the flag for the column B
    - integer
    - 0: it rained (the value B can be 0.0)
    - 1: no rainfall at all
  - D, E: not necessary for analysis
  - F: the max amount in 60 min of the day (mm)
    - float
  - G: the flag for the column F
    - integer
    - 0: it rained (the value F can be 0.0)
    - 1: no rainfall at all
  - H, I: not necessary for analysis