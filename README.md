# jmaster
用Jmeter設計的自動抓取寵物機器人

## 必要套件
Apache JMeter

[https://jmeter.apache.org/download_jmeter.cgi](https://jmeter.apache.org/download_jmeter.cgi)

## 資料夾結構

cat.jmx 抓取寵物用程式

env.csv.swp 程式參數檔

reserve.jmx 預約寵物用程式

## 使用說明
將.env.csv.swp改成.env.csv，並修改裡面所需之內容

## 運行方式
```
#預約寵物
./jmeter -n -t [go to path]/reserve.jmx -Jlevel=[寵物等級]

#抓取寵物
./jmeter -n -t [go to path]/cat.jmx -Jlevel=[寵物等級] -Jcount=[線程數] -Jid=[寵物id]
```

## 如何修改本程式

到JMeter資料夾裡面的bin底下，下此指令打開JMeter GUI編輯器
```
sh jmeter.sh
```