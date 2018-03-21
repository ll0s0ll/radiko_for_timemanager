radikoの聴取をTimeManagerにスケジュールするためのプログラムです。

標準では繰り返し実行されます。繰り返す回数、間隔はオプションで設定できます。

## SYNOPSIS
```
radiko_for_timemanager.py [-h] [-i INTERVAL] [-r REPEAT] [-v] {TBS,QRR,LFR,JORF,INT,FMT,FMJ,BAYFM78,NACK5,YFM} schedule duration caption
```

## EXAMPLE  
```
# Fm yokohamaのPRIME TIME(毎週 月-木曜日 19:00-22:00)を予約する。
$ radiko_for_timemanager.py YFM "0 19 * * 1-4" 10800 "Fm yokohama PRIME TIME"
```

## NOTE
内部で以下のプログラムを呼び出しています。別途ご準備ください。
- [play_radiko.sh](https://gist.github.com/ihsoy-s/5292735#file-play_radiko-sh)
- [TimeManager](https://github.com/ll0s0ll/TimeManager)

## SEE ALSO
[TimeManagerを使って、聴きたいラジオ番組が流れてくる、自分だけのラジオを作る](https://ll0s0ll.wordpress.com/raspberrypi/automated_radio_station/)
