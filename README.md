# V2RayAggregator


[![Collect](https://github.com/mahdibland/SSAggregator/actions/workflows/Collector.yml/badge.svg)](https://github.com/mahdibland/SSAggregator/actions/workflows/Collector.yml) [![Airport Collect](https://github.com/mahdibland/SSAggregator/actions/workflows/Airport_Collector.yml/badge.svg)](https://github.com/mahdibland/SSAggregator/actions/workflows/Airport_Collector.yml)

## Quick Note & Updates
🔴 ~~This project is still under maintance. so don't use it until further announcement cause there is a chance you will get errors while updating the nodes, etc.~~  

🟢 11/1/2022: from now you can use this project. also readme file updated with the recent changes so you can find out which file to use.

## Introduction

The automation functions of this repository are all implemented based on `GitHub Actions`

Test the speed of each free node pool on the network and the nodes shared by bloggers to screen out relatively stable and high-speed nodes, and then import them into the warehouse for sharing records.

The speed measurement function is implemented in the `GitHub Actions` environment using [LiteSpeedTest](https://github.com/xxf098/LiteSpeedTest), so there are many nodes in the United States, which cannot well represent the node availability in the domestic network environment.

## Features
- Lots of sources 😯
- Remove all duplicate nodes 🤤
- Providing nodes in major formats (YAML, clash, v2ray, base64) 🦋
- No additional conversion to prevent breaking the nodes 🌿
- Filtering best nodes by testing them and sorting them based on their average speed 🍀

## Recent Todos
- [x] ~~Fix region based lite speed test (mainly EU)~~ 👀
- [x] Fix Sort Based on the Avg Speed 👀
- [x] Update required softwares to latest version 👀
- [x] Fix sources that subconvertor unable to convert 👀
- [x] Add separate files & functions for airport 👀
- [x] Fix name (emoji+ip) for all log files 👀
- [x] Separate sub list for airports & other nodes 👀
- [x] Fixed clash template 👀
- [ ] Cleanup redundant files and functions (dev Branch) 🧲

## Visualizer

- Log Visualizer on Netlify 
> if you click on any node url it will copy to clipboard



|                  |             Link to Log              |
|:----------------:|:-----------------------------:|
|   Public Nodes   |   <a href="https://55292969231427515295.netlify.app/" target="_blank"><img src="https://i.ibb.co/g32RmJy/netlify.png" width="35"/></a>   |
|     Airport      |   <a href="https://55292969231427515295.netlify.app?type=airport" target="_blank"><img src="https://i.ibb.co/g32RmJy/netlify.png" width="35"/></a>   |

## Instructions & Usage

### Tips
- If you see an IP repeated more than once it's usually because of the different ports.
- (Group 2) Some free airports only provide 1GB of traffic or have limited time to use that's why I update the airport node every 2 hours. so if you want to use them set the auto-update option on your client to get fresh nodes.
- (Group 1) Other public nodes are more stable and will be updated every 12 hours.
- Depending on your internet provider and location, some nodes might not work.


### Ready to import (200 filtered nodes)
> Just import the following subscription link into the corresponding client. Use a client that atleast support ss + ssr + vmess + trojan.

Nodes filtered using speedtest measurement will be stored in following files:  

* Group 1 (Contains free public nodes)
- [Base64](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/Eternity)
- [Mixed](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/Eternity.txt)
- [Clash](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/Eternity.yml)

* Group 2 (Contains only free airports)
- [Base64](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/EternityAir)
- [Mixed](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/EternityAir.txt)
- [Clash](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/EternityAir.yml)

### For Local Testing (all nodes)
> Only for local testing because the number of nodes is too high and your client will crash if you import them  

All of the nodes merged together will be stored in following files:  

* Group 1 (Contains free public nodes)
- [Base64](https://raw.githubusercontent.com/mahdibland/SSAggregator/master/sub/sub_merge_base64.txt)
- [Mixed](https://raw.githubusercontent.com/mahdibland/SSAggregator/master/sub/sub_merge.txt)
- [Clash](https://raw.githubusercontent.com/mahdibland/SSAggregator/master/sub/sub_merge_yaml.yml)

* Group 2 (Contains only free airports)
- [Base64](https://raw.githubusercontent.com/mahdibland/SSAggregator/master/sub/airport_merge_base64.txt)
- [Mixed](https://raw.githubusercontent.com/mahdibland/SSAggregator/master/sub/airport_sub_merge.txt)
- [Clash](https://raw.githubusercontent.com/mahdibland/SSAggregator/master/sub/airport_merge_yaml.yml)

### Manual Subs Conversion
- If your client does not support the formats that provided here use below services to convert them to your client format (like surfboard)
> Services for online sub conversion: 
- [sub-web-modify](https://sub.v1.mk/)
- [bianyuan](https://bianyuan.xyz/)  

- **If you don't like the groups and rules that are already set, you can simply use bianyuan API like this::**  
> don't use this API for your personal airport subs! Pls run the subconverter locally
```
https://pub-api-1.bianyuan.xyz/sub?target=(OutputFormat)&url=(SubUrl)&insert=false

For Example:
(OutputFormat) = clash
(SubUrl) = https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/Eternity.yml

https://pub-api-1.bianyuan.xyz/sub?target=clash&url=https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/Eternity.yml&insert=false

Now you can use the link above to import the subs into your client
```

<br/>

## Node Information

### high-speed node
high-speed node quantity: `200`

<details>
    trojan://dfbf0d67-f03d-4184-a224-c2d64a571f99@s1.hass.win:12340?allowInsecure=1&sni=static.dingtalk.com#%F0%9F%87%BA%F0%9F%87%B8US-147.182.224.102-12778
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpvX0E3aW5OMXlxZVd0T1RM@104.207.155.64:1633#%F0%9F%87%BA%F0%9F%87%B8US-104.207.155.64-0665
    vmess://ewogICAgImFkZCI6ICJsaW4wNTAyLmh3Y2FyLnNicyIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImxpbmphMDUuaHdjYXIuc2JzIiwKICAgICJpZCI6ICIzOWNlYzE4Zi1hNDM5LTQyN2MtOWE0ZS1hZWI2ZmNkZjZmNTMiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvbGlua3dzIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMjEuOTQuNjQtMDQ0NiIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://YWVzLTEyOC1nY206WWMyQ3RySXo4TA==@75.102.51.61:16899#%F0%9F%87%BA%F0%9F%87%B8US-75.102.51.61-0853
    vmess://ewogICAgImFkZCI6ICJqcC5ybm1jbm0uY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAianAucm5tY25tLmNvbSIsCiAgICAiaWQiOiAiNTY2MjcxOGYtZTNlNi00YTk2LWNhNDMtMjM5NDIxOWNmYjQ3IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiLyIsCiAgICAicG9ydCI6IDgwLAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMjEuNzAuMTQ1LTA2NjkiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    trojan://ypDt8RkT7J@185.180.13.70:43118?security=tls&sni=earya.phooeyunfold.com#%F0%9F%87%BA%F0%9F%87%B8US-185.180.13.70-0829
    ss://YWVzLTEyOC1jZmI6c2hhZG93c29ja3M=@184.170.241.194:443#%F0%9F%87%BA%F0%9F%87%B8US-184.170.241.194-0674
    vmess://ewogICAgImFkZCI6ICIxODguMTE0Ljk5LjIwNSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImxpbmRlMDYuaW5kaWF2aWRlby5zYnMiLAogICAgImlkIjogImVkYmIxMDU5LTE2MzMtNDI3MS1iNjZlLWVkNGZiYTQ3YTFiZiIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9saW5rd3MiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTE4OC4xMTQuOTkuMjA1LTA0NjQiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IGZhbHNlLAogICAgInNuaSI6ICJsaW5kZTA2LmluZGlhdmlkZW8uc2JzIgp9
    vmess://ewogICAgImFkZCI6ICIxOTIuMy4xNTAuMjMzIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJhNmEzN2UwNC01ZTgxLTQ0YzktYmU1My1iYWEzZmY0NmViOGIiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvOGNkYTQ4YjMiLAogICAgInBvcnQiOiA4NDQzLAogICAgInBzIjogIvCfh7rwn4e4VVMtMTkyLjMuMTUwLjIzMy04NDM5IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIyMy4yNTQuMTY2LjIzNyIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIjIzLjI1NC4xNjYuMjM3IiwKICAgICJpZCI6ICI4ZDBmZDYxOC01ZDYwLTQwZDYtOWYyMy1lNTAzNTU1ZjQ5NmYiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvIiwKICAgICJwb3J0IjogMjA4NiwKICAgICJwcyI6ICLwn4e68J+HuFVTLTIzLjI1NC4xNjYuMjM3LTA2NzciLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICJzLm1hcmt0cmVkLmNvbSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImF2ZWlyb3IuY29tIiwKICAgICJpZCI6ICIwM2ZjYzYxOC1iOTNkLTY3OTYtNmFlZC04YTM4Yzk3NWQ1ODEiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvbGlua3Z3cyIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjIxLjUyLjEwMy0wNDIyIiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiBmYWxzZSwKICAgICJzbmkiOiAiYXZlaXJvci5jb20iCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTo5QnZrdzVhdXBOeTg=@205.134.180.147:443#%F0%9F%87%BA%F0%9F%87%B8US-205.134.180.147-0736
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpoZ0xDZ2ZMUmdCNmQ=@205.134.180.145:443#%F0%9F%87%BA%F0%9F%87%B8US-205.134.180.145-0678
    trojan://ypDt8RkT7J@89.187.181.172:43118?security=tls&sni=egcmi.phooeyunfold.com#%F0%9F%87%BA%F0%9F%87%B8US-89.187.181.172-0681
    trojan://ypDt8RkT7J@138.199.41.25:43118?security=tls&sni=dngn.phooeyunfold.com#%F0%9F%87%BA%F0%9F%87%B8US-138.199.41.25-0689
    vmess://ewogICAgImFkZCI6ICIxNTguNTEuMTIxLjM2IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICIwM2ZjYzYxOC1iOTNkLTY3OTYtNmFlZC04YTM4Yzk3NWQ1ODEiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvbGlua3Z3cyIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4eo8J+HpkNBLTE1OC41MS4xMjEuMzYtMTIzMiIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTo1Y3A5WjNpV25KWjI=@205.134.180.151:443#%F0%9F%87%BA%F0%9F%87%B8US-205.134.180.151-0680
    vmess://ewogICAgImFkZCI6ICIxMDQuMTguODQuMTA0IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAicm4xLmhvc3RtamouY29tIiwKICAgICJpZCI6ICIyMTFkOGEzNC05YzQ4LTQ0MzUtYjRiZi0zNDNhZTFjYmRhMGUiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvIiwKICAgICJwb3J0IjogODAsCiAgICAicHMiOiAi8J+PgVJFTEFZLTEwNC4xOC44NC4xMDQtMDY3MyIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogZmFsc2UsCiAgICAic25pIjogInJuMS5ob3N0bWpqLmNvbSIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTp4UHJLVUJRUHdDRmVYRVE1dVhsUk5Y@13.94.117.31:10238#%F0%9F%87%AE%F0%9F%87%AAIE-13.94.117.31-0697
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpnMTNTN2RvWGFyMEE=@205.134.180.137:443#%F0%9F%87%BA%F0%9F%87%B8US-205.134.180.137-8387
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@195.154.169.198:989#%F0%9F%87%AB%F0%9F%87%B7FR-195.154.169.198-0730
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@195.154.185.174:989#%F0%9F%87%AB%F0%9F%87%B7FR-195.154.185.174-0726
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpCb2cwRUxtTU05RFN4RGRR@4.158.26.91:443#%F0%9F%87%AC%F0%9F%87%A7GB-4.158.26.91-0720
    vmess://ewogICAgImFkZCI6ICJkZW5jMzYueHRvb2x0ZWNoLmNmZCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImFkZW5jMzZ2Lnh0b29sdGVjaC5jZmQiLAogICAgImlkIjogImIzMjFmZDVkLWU2ZWMtNDI5My1hNjQ0LTE2NGUzODg1ZjUyZSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9saW5rd3MiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTEwNC4yMS4yNC4xNzAtMDQ4OSIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@51.159.111.208:989#%F0%9F%87%AB%F0%9F%87%B7FR-51.159.111.208-0731
    ss://YWVzLTEyOC1jZmI6c2hhZG93c29ja3M=@109.201.152.181:443#%F0%9F%87%B3%F0%9F%87%B1NL-109.201.152.181-0724
    vmess://ewogICAgImFkZCI6ICIzOC45NS4xMTUuMTc2IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICI5ZWVkYjBkNC0yN2ZiLTQ3ZTYtYjNiNS0zMDE3MTIzMzdlY2YiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvIiwKICAgICJwb3J0IjogMTY0MjQsCiAgICAicHMiOiAi8J+HuvCfh7hVUy0zOC45NS4xMTUuMTc2LTAzOTEiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.195:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.195-0706
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.81:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.81-0716
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@uk-dc1.yangon.club:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.197-0717
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.197:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.197-0712
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.196:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.196-0711
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.79:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.79-0710
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.198:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.198-0718
    trojan://M3lOal9RPR@kkr100515a.go02.top:30056?security=tls&sni=kkr100515a.go02.top#%F0%9F%87%B0%F0%9F%87%B7KR-146.56.171.71-0698
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTptcHMzRndtRGpMcldhT1Zn@series-a2.samanehha.co:443#%F0%9F%87%AC%F0%9F%87%A7GB-18.135.151.44-0729
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.194:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.194-0097
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@51.15.27.48:989#%F0%9F%87%AB%F0%9F%87%B7FR-51.15.27.48-0722
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpXNzRYRkFMTEx1dzZtNUlB@series-a1.samanehha.co:443#%F0%9F%87%AC%F0%9F%87%A7GB-18.135.151.44-0728
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.78:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.78-5070
    trojan://M3lOal9RPR@146.56.171.71:30056?security=tls&sni=kkr100515a.go02.top#%F0%9F%87%B0%F0%9F%87%B7KR-146.56.171.71-0700
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.80:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.80-0714
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.193:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.193-0704
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpsV2FHUFZGam1uYWc=@205.134.180.139:443#%F0%9F%87%BA%F0%9F%87%B8US-205.134.180.139-0682
    trojan://ypDt8RkT7J@138.199.23.100:43118?security=tls&sni=radtz.phooeyunfold.com#%F0%9F%87%AF%F0%9F%87%B5JP-138.199.23.100-0707
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpJNTN1SnNaYzZkelRCWURFcWcxYTMwQmgxaEFkNEhRemdwd0NWZHB6S3dmRjJaVWg=@168.119.57.171:51348#%F0%9F%87%A9%F0%9F%87%AADE-168.119.57.171-0545
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuNTEuMjMyIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiaXAwMDUuZHRrdTQ3Lnh5eiIsCiAgICAiaWQiOiAiMjllZWJiNjAtYjI3Yi00YTlkLWJiYTUtOTQ3NzYzZDkyMDVlIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDg2LAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMTkuNTEuMjMyLTAyMDgiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@194.71.126.31:989#%F0%9F%87%B7%F0%9F%87%B8RS-194.71.126.31-0744
    trojan://ypDt8RkT7J@138.199.57.185:43118?security=tls&sni=eiety.phooeyunfold.com#%F0%9F%87%A8%F0%9F%87%A6CA-138.199.57.185-0691
    vmess://ewogICAgImFkZCI6ICIxODUuMTQ2LjE3My41OSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIm9iZGlpLmNmZCIsCiAgICAiaWQiOiAiMDU2NDFjZjUtNThkMi00YmE0LWE5ZjEtYjNjZGEwYjFmYjFkIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2xpbmt3cyIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4+BUkVMQVktMTg1LjE0Ni4xNzMuNTktMDMxNyIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@121.127.46.147:989#%F0%9F%87%B8%F0%9F%87%AASE-121.127.46.147-0742
    trojan://ypDt8RkT7J@151.115.83.239:43118?security=tls&sni=egajz.phooeyunfold.com#%F0%9F%87%B5%F0%9F%87%B1PL-151.115.83.239-0741
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@194.14.217.115:989#%F0%9F%87%B7%F0%9F%87%B4RO-194.14.217.115-0747
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@192.71.166.102:989#%F0%9F%87%AC%F0%9F%87%B7GR-192.71.166.102-0750
    vmess://ewogICAgImFkZCI6ICIzOC40Ni40LjE4MiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIjM4LjQ2LjQuMTgyIiwKICAgICJpZCI6ICI1MjkwMDcyMC0wNDc5LTQ4Y2MtYjJkOC05ZThhZGJmNWFiNDciLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvNTI5MDA3MjAiLAogICAgInBvcnQiOiA1Nzc3NiwKICAgICJwcyI6ICLwn4e68J+HuFVTLTM4LjQ2LjQuMTgyLTAzMDIiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    trojan://ypDt8RkT7J@62.210.83.57:43118?security=tls&sni=ruvil.phooeyunfold.com#%F0%9F%87%AB%F0%9F%87%B7FR-62.210.83.57-0800
    trojan://ypDt8RkT7J@51.158.217.197:43118?security=tls&sni=riyyy.phooeyunfold.com#%F0%9F%87%AB%F0%9F%87%B7FR-51.158.217.197-0757
    ssr://anAtYW00OC02LmVxbm9kZS5uZXQ6ODA4MTpvcmlnaW46YWVzLTI1Ni1jZmI6dGxzMS4yX3RpY2tldF9hdXRoOlpVRnZhMkpoUkU0Mi8/b2Jmc3BhcmFtPSZyZW1hcmtzPThKJTJCSHIlMkZDZmg3VktVQzB4T0M0eE56Y3VNVE0yTGpFME5pMHdOamt6JnByb3RvcGFyYW09
    trojan://ypDt8RkT7J@51.159.102.179:43118?security=tls&sni=tpzmg.phooeyunfold.com#%F0%9F%87%AB%F0%9F%87%B7FR-51.159.102.179-0764
    trojan://ypDt8RkT7J@62.210.82.54:43118?security=tls&sni=wuxgk.phooeyunfold.com#%F0%9F%87%AB%F0%9F%87%B7FR-62.210.82.54-0768
    trojan://ypDt8RkT7J@51.158.217.57:43118?security=tls&sni=tojzy.phooeyunfold.com#%F0%9F%87%AB%F0%9F%87%B7FR-51.158.217.57-0753
    trojan://ypDt8RkT7J@169.150.206.186:43118?security=tls&sni=tpmem.phooeyunfold.com#%F0%9F%87%A9%F0%9F%87%AADE-169.150.206.186-0748
    trojan://ypDt8RkT7J@51.158.217.60:43118?security=tls&sni=ewxig.phooeyunfold.com#%F0%9F%87%AB%F0%9F%87%B7FR-51.158.217.60-0754
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@31.171.153.181:989#%F0%9F%87%A6%F0%9F%87%B1AL-31.171.153.181-0772
    trojan://ypDt8RkT7J@213.186.36.123:43118?security=tls&sni=wylbe.phooeyunfold.com#%F0%9F%87%AB%F0%9F%87%B7FR-213.186.36.123-0766
    trojan://ypDt8RkT7J@51.158.217.130:43118?security=tls&sni=toflf.phooeyunfold.com#%F0%9F%87%AB%F0%9F%87%B7FR-51.158.217.130-0765
    trojan://ypDt8RkT7J@89.187.189.88:43118?security=tls&sni=tpmrr.phooeyunfold.com#%F0%9F%87%A8%F0%9F%87%BFCZ-89.187.189.88-0779
    trojan://ypDt8RkT7J@51.158.217.161:43118?security=tls&sni=tewmk.phooeyunfold.com#%F0%9F%87%AB%F0%9F%87%B7FR-51.158.217.161-0770
    vmess://ewogICAgImFkZCI6ICJ1cGxvYWQuaXIiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJhZnJobXMxNnYuYmVzdHhyYXkuYnV6eiIsCiAgICAiaWQiOiAiZjU4NGRlMTUtMjAzNC00MTcwLWE3MjMtZjQ4YzJiYWU1ZTBmIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2xpbmt3cyIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjIxLjEzLjEyNS0wNDYxIiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    trojan://ypDt8RkT7J@121.127.46.131:43118?security=tls&sni=tpmrt.phooeyunfold.com#%F0%9F%87%B8%F0%9F%87%AASE-121.127.46.131-0767
    trojan://ypDt8RkT7J@212.102.54.11:43118?security=tls&sni=tpmrq.phooeyunfold.com#%F0%9F%87%AE%F0%9F%87%B9IT-212.102.54.11-0776
    vmess://ewogICAgImFkZCI6ICIxNTIuNjkuMTk3Ljc0IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJiOGE2YmY1OC00ODVhLTQwNDYtYjM4Ni1iMzY2MWJmNjVlZmYiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvYmIiLAogICAgInBvcnQiOiAxMjM0NSwKICAgICJwcyI6ICLwn4ev8J+HtUpQLTE1Mi42OS4xOTcuNzQtMjM0NiIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxMDQuMjEuMjQuMTcwIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiYWRlbmMzNnYueHRvb2x0ZWNoLmNmZCIsCiAgICAiaWQiOiAiYjMyMWZkNWQtZTZlYy00MjkzLWE2NDQtMTY0ZTM4ODVmNTJlIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2xpbmt3cyIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjIxLjI0LjE3MC0wMjU3IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIyMy4yMjcuMzguNiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImlwMDA2LmR0a3U0Ny54eXoiLAogICAgImlkIjogIjI5ZWViYjYwLWIyN2ItNGE5ZC1iYmE1LTk0Nzc2M2Q5MjA1ZSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA4NiwKICAgICJwcyI6ICLwn4+BUkVMQVktMjMuMjI3LjM4LjYtMDI3OCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpINVMwaHZjeFJpI1lMbWdV@38.107.226.146:1230#%F0%9F%87%BA%F0%9F%87%B8US-38.107.226.146-0802
    trojan://ypDt8RkT7J@51.158.217.195:43118?security=tls&sni=wnbtg.phooeyunfold.com#%F0%9F%87%AB%F0%9F%87%B7FR-51.158.217.195-0771
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuMzguNjIiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJpcDAwNS5kdGt1NDcueHl6IiwKICAgICJpZCI6ICIyOWVlYmI2MC1iMjdiLTRhOWQtYmJhNS05NDc3NjNkOTIwNWUiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICJnaXRodWIuY29tL0FsdmluOTk5OSIsCiAgICAicG9ydCI6IDIwODYsCiAgICAicHMiOiAi8J+PgVJFTEFZLTEwNC4xOS4zOC42Mi0wMzE0IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiBmYWxzZSwKICAgICJzbmkiOiAiaXAwMDUuZHRrdTQ3Lnh5eiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxMDQuMjEuOTUuMTY1IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAic2FyZWlrZWxhLmNvbSIsCiAgICAiaWQiOiAiMDNmY2M2MTgtYjkzZC02Nzk2LTZhZWQtOGEzOGM5NzVkNTgxIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2xpbmt2d3MiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTEwNC4yMS45NS4xNjUtMDUxNyIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    trojan://ypDt8RkT7J@207.211.215.169:43118?security=tls&sni=tpmwf.phooeyunfold.com#%F0%9F%87%B9%F0%9F%87%B7TR-207.211.215.169-0825
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpKSWhONnJCS2thRWJvTE5YVlN2NXJx@142.4.216.225:80#%F0%9F%87%A8%F0%9F%87%A6CA-142.4.216.225-0759
    vmess://ewogICAgImFkZCI6ICIyMy4yMjcuMzguNiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImlwMDA1LmR0a3U0Ny54eXoiLAogICAgImlkIjogIjI5ZWViYjYwLWIyN2ItNGE5ZC1iYmE1LTk0Nzc2M2Q5MjA1ZSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA4NiwKICAgICJwcyI6ICLwn4+BUkVMQVktMjMuMjI3LjM4LjYtMTE4NyIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogZmFsc2UsCiAgICAic25pIjogImlwMDA1LmR0a3U0Ny54eXoiCn0=
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@41.203.4.34:989#%F0%9F%87%BF%F0%9F%87%A6ZA-41.203.4.34-0795
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@185.164.35.9:989#%F0%9F%87%A7%F0%9F%87%A6BA-185.164.35.9-0763
    vmess://ewogICAgImFkZCI6ICIxMDQuMjUuOTEuMTk1IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAicnUyLnZtZXNzLnNpdGUiLAogICAgImlkIjogIjBjMzY3ZGE3LWU4ODItNDcyNy04YzI5LWVjYjBiZGE5MDUyOCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi8iLAogICAgInBvcnQiOiA4MCwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjI1LjkxLjE5NS0wNzg3IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuNDYuMjMzIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiaXAwMDUuZHRrdTQ3Lnh5eiIsCiAgICAiaWQiOiAiMjllZWJiNjAtYjI3Yi00YTlkLWJiYTUtOTQ3NzYzZDkyMDVlIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDg2LAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMTkuNDYuMjMzLTExODYiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IGZhbHNlLAogICAgInNuaSI6ICJpcDAwNS5kdGt1NDcueHl6Igp9
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@138.186.142.4:989#%F0%9F%87%B5%F0%9F%87%A6PA-138.186.142.4-8791
    vmess://ewogICAgImFkZCI6ICIxMDQuMTYuMTQ4LjI0NCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImlwMDA2LmZyZWVncmFkZWx5Lnh5eiIsCiAgICAiaWQiOiAiMjllZWJiNjAtYjI3Yi00YTlkLWJiYTUtOTQ3NzYzZDkyMDVlIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDg2LAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMTYuMTQ4LjI0NC0wNDEyIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiBmYWxzZSwKICAgICJzbmkiOiAiaXAwMDYuZnJlZWdyYWRlbHkueHl6Igp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@134.195.196.178:804#%F0%9F%87%A8%F0%9F%87%A6CA-134.195.196.178-0788
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@77.72.5.150:989#%F0%9F%87%AC%F0%9F%87%A7GB-77.72.5.150-0719
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuNDcuNDUiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJpcDE0LmZyZWVncmFkZWx5Lnh5eiIsCiAgICAiaWQiOiAiZTllM2NjMTMtZGI0OC00Y2MxLThjMjQtNzYyNjQzOWE1MzM5IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDg2LAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMTkuNDcuNDUtMDIwNyIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICJhejA1LmJleW9uZHkuY2ZkIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiYXowNS5iZXlvbmR5LmNmZCIsCiAgICAiaWQiOiAiM2Y2MzhmMzQtOGRiYS00MTg2LWJjNDMtMjcxNmE3ZGRkNGJlIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2xpbmsiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+Hq/Cfh7dGUi0xNDYuMTkuMTY4LjE2MS0wNDg3IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.178.87.37:805#%F0%9F%87%AB%F0%9F%87%B7FR-51.178.87.37-0585
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuMzguNjIiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJpcDAwNi5mcmVlZ3JhZGVseS54eXoiLAogICAgImlkIjogIjI5ZWViYjYwLWIyN2ItNGE5ZC1iYmE1LTk0Nzc2M2Q5MjA1ZSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA4NiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjE5LjM4LjYyLTExODEiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IGZhbHNlLAogICAgInNuaSI6ICJpcDAwNi5mcmVlZ3JhZGVseS54eXoiCn0=
    vmess://ewogICAgImFkZCI6ICIxNzIuNjcuNzQuMTEyIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiaXAxMS5mcmVlZ3JhZGVseS54eXoiLAogICAgImlkIjogImU5ZTNjYzEzLWRiNDgtNGNjMS04YzI0LTc2MjY0MzlhNTMzOSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA4NiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTcyLjY3Ljc0LjExMi0wMzM2IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxNzIuNjQuOTkuMjIiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJpcDExLmZyZWVncmFkZWx5Lnh5eiIsCiAgICAiaWQiOiAiZTllM2NjMTMtZGI0OC00Y2MxLThjMjQtNzYyNjQzOWE1MzM5IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDg2LAogICAgInBzIjogIvCfj4FSRUxBWS0xNzIuNjQuOTkuMjItMDMzNCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@31.171.153.178:989#%F0%9F%87%A6%F0%9F%87%B1AL-31.171.153.178-0863
    vmess://ewogICAgImFkZCI6ICIxMDQuMTYuNjAuOCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInVzLWNjcy55dWppMjAyMi5ldS5vcmciLAogICAgImlkIjogIjRiNWU0NTY1LTMyMmYtNDIyMy1hODkxLTc4YTg0ZjE4OTcyNiIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9YU2plZzczbzZaZHNoZWFoQ2I1SkciLAogICAgInBvcnQiOiA4ODgwLAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMTYuNjAuOC0wNDk5IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxMDQuMjYuNy4xMzIiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJpcDIuMTQ1NzIzMC54eXoiLAogICAgImlkIjogImU5ZTNjYzEzLWRiNDgtNGNjMS04YzI0LTc2MjY0MzlhNTMzOSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA4NiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjI2LjcuMTMyLTAyMTUiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@37.143.129.230:989#%F0%9F%87%AB%F0%9F%87%AEFI-37.143.129.230-4933
    vmess://ewogICAgImFkZCI6ICJ1czNlLW1tbm5mcjlkb3AwLnYyZnJlZXZwbi5jb20iLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJ1czNlLW1tbm5mcjlkb3AwLnYyZnJlZXZwbi5jb20iLAogICAgImlkIjogIjJhOGExMGZiLTljYTMtMzY3ZS1hMjM0LWNmMDlmODQxYmU0ZiIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi92MTE4LWZjY3hteG0zNSIsCiAgICAicG9ydCI6IDgwLAogICAgInBzIjogIvCfj4FSRUxBWS0xNzIuNjcuMTcwLjc1LTAzMDAiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICJzdHJlYW1kZXcuYnV6eiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInN0cmVhbWRldy5idXp6IiwKICAgICJpZCI6ICI2ZmJhOWRlZC1iYjE5LTQzOWMtYjBmYy0zM2FiNmMwM2MzOWIiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvNmZiYTlkZWQtYmIxOS00MzljLWIwZmMtMzNhYjZjMDNjMzliIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfh7rwn4e4VVMtMTMyLjIyNi4xNDkuMTgwLTEyNDEiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxMDQuMjYuMC41NiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImlwMTQuZnJlZWdyYWRlbHkueHl6IiwKICAgICJpZCI6ICJlOWUzY2MxMy1kYjQ4LTRjYzEtOGMyNC03NjI2NDM5YTUzMzkiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICJnaXRodWIuY29tL0FsdmluOTk5OSIsCiAgICAicG9ydCI6IDIwODYsCiAgICAicHMiOiAi8J+PgVJFTEFZLTEwNC4yNi4wLjU2LTEyMjYiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuNDUuODMiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJvbmVhLmZsaGEucnUiLAogICAgImlkIjogIjdhNzM3ZjQxLWI3OTItNDI2MC05NGZmLTNkODY0ZGE2N2I4MCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi8iLAogICAgInBvcnQiOiAyMDk1LAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMTkuNDUuODMtMDIyNiIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuNDUuMzEiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJpcDEzLmZyZWVncmFkZWx5Lnh5eiIsCiAgICAiaWQiOiAiZTllM2NjMTMtZGI0OC00Y2MxLThjMjQtNzYyNjQzOWE1MzM5IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDg2LAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMTkuNDUuMzEtMDMwMyIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxMDQuMTguNTcuMTExIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiaXAyLjE0NTcyMzAueHl6IiwKICAgICJpZCI6ICJlOWUzY2MxMy1kYjQ4LTRjYzEtOGMyNC03NjI2NDM5YTUzMzkiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICJnaXRodWIuY29tL0FsdmluOTk5OSIsCiAgICAicG9ydCI6IDIwODYsCiAgICAicHMiOiAi8J+PgVJFTEFZLTEwNC4xOC41Ny4xMTEtMjc5MCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxMDQuMjAuMTcuMTg2IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiY2RuMS5mcmVlZ3JhZGVseS54eXoiLAogICAgImlkIjogImQ2YjZkOTgyLWQ1MmYtNDY1YS1iOTg4LTg1NjcwYjIzZjY0YSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA1MiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjIwLjE3LjE4Ni0xMDk3IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxNjIuMTU5LjE0MC43NyIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImlwMS4xNzg5MDM0Lnh5eiIsCiAgICAiaWQiOiAiZTllM2NjMTMtZGI0OC00Y2MxLThjMjQtNzYyNjQzOWE1MzM5IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDg2LAogICAgInBzIjogIvCfj4FSRUxBWS0xNjIuMTU5LjE0MC43Ny0xMTM3IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiBmYWxzZSwKICAgICJzbmkiOiAiaXAxLjE3ODkwMzQueHl6Igp9
    vmess://ewogICAgImFkZCI6ICIxNjIuMTU5LjE0MC4xOSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImlwMS4xNzg5MDM0Lnh5eiIsCiAgICAiaWQiOiAiZTllM2NjMTMtZGI0OC00Y2MxLThjMjQtNzYyNjQzOWE1MzM5IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDg2LAogICAgInBzIjogIvCfj4FSRUxBWS0xNjIuMTU5LjE0MC4xOS0xMTM4IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiBmYWxzZSwKICAgICJzbmkiOiAiaXAxLjE3ODkwMzQueHl6Igp9
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuNTguMTg1IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiY2RuMy5mcmVlZ3JhZGVseS54eXoiLAogICAgImlkIjogImQ2YjZkOTgyLWQ1MmYtNDY1YS1iOTg4LTg1NjcwYjIzZjY0YSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA1MiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjE5LjU4LjE4NS0xMjA4IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiBmYWxzZSwKICAgICJzbmkiOiAiY2RuMy5mcmVlZ3JhZGVseS54eXoiCn0=
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuMjEuMjIwIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiY2RuMi5mcmVlZ3JhZGVseS54eXoiLAogICAgImlkIjogImQ2YjZkOTgyLWQ1MmYtNDY1YS1iOTg4LTg1NjcwYjIzZjY0YSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA1MiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjE5LjIxLjIyMC0wMjg1IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@190.120.231.45:989#%F0%9F%87%A8%F0%9F%87%B4CO-190.120.231.45-8445
    vmess://ewogICAgImFkZCI6ICIxNzIuNjQuMTk4LjI0OSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImlwMTQuZnJlZWdyYWRlbHkueHl6IiwKICAgICJpZCI6ICJlOWUzY2MxMy1kYjQ4LTRjYzEtOGMyNC03NjI2NDM5YTUzMzkiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICJnaXRodWIuY29tL0FsdmluOTk5OSIsCiAgICAicG9ydCI6IDIwODYsCiAgICAicHMiOiAi8J+PgVJFTEFZLTE3Mi42NC4xOTguMjQ5LTAyMjIiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuNDYuMzYiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJpcDEzLmZyZWVncmFkZWx5Lnh5eiIsCiAgICAiaWQiOiAiZTllM2NjMTMtZGI0OC00Y2MxLThjMjQtNzYyNjQzOWE1MzM5IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDg2LAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMTkuNDYuMzYtMDM0MCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxNjIuMTU5LjE0MC44OSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImlwMS4xNzg5MDM0Lnh5eiIsCiAgICAiaWQiOiAiZTllM2NjMTMtZGI0OC00Y2MxLThjMjQtNzYyNjQzOWE1MzM5IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDg2LAogICAgInBzIjogIvCfj4FSRUxBWS0xNjIuMTU5LjE0MC44OS0xMTM2IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiBmYWxzZSwKICAgICJzbmkiOiAiaXAxLjE3ODkwMzQueHl6Igp9
    vmess://ewogICAgImFkZCI6ICIxNzIuNjQuMTc1LjIyMyIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNkbjIuZnJlZWdyYWRlbHkueHl6IiwKICAgICJpZCI6ICJkNmI2ZDk4Mi1kNTJmLTQ2NWEtYjk4OC04NTY3MGIyM2Y2NGEiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICJnaXRodWIuY29tL0FsdmluOTk5OSIsCiAgICAicG9ydCI6IDIwNTIsCiAgICAicHMiOiAi8J+PgVJFTEFZLTE3Mi42NC4xNzUuMjIzLTAyNTQiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxNzIuNjcuNzQuMTIyIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiY2RuMy5mcmVlZ3JhZGVseS54eXoiLAogICAgImlkIjogImQ2YjZkOTgyLWQ1MmYtNDY1YS1iOTg4LTg1NjcwYjIzZjY0YSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA1MiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTcyLjY3Ljc0LjEyMi0xMjE4IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiBmYWxzZSwKICAgICJzbmkiOiAiY2RuMy5mcmVlZ3JhZGVseS54eXoiCn0=
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuNDUuMjQxIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAib25lYS5mbGhhLnJ1IiwKICAgICJpZCI6ICI3YTczN2Y0MS1iNzkyLTQyNjAtOTRmZi0zZDg2NGRhNjdiODAiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvIiwKICAgICJwb3J0IjogMjA5NSwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjE5LjQ1LjI0MS0wMjMwIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxMDQuMjAuMjUuMTc2IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiY2RuMy5mcmVlZ3JhZGVseS54eXoiLAogICAgImlkIjogImQ2YjZkOTgyLWQ1MmYtNDY1YS1iOTg4LTg1NjcwYjIzZjY0YSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA1MiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjIwLjI1LjE3Ni0xMjE2IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiBmYWxzZSwKICAgICJzbmkiOiAiY2RuMy5mcmVlZ3JhZGVseS54eXoiCn0=
    vmess://ewogICAgImFkZCI6ICIxMDQuMjAuMjUuMTY2IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiY2RuMy5mcmVlZ3JhZGVseS54eXoiLAogICAgImlkIjogImQ2YjZkOTgyLWQ1MmYtNDY1YS1iOTg4LTg1NjcwYjIzZjY0YSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA1MiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjIwLjI1LjE2Ni0xMjE1IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiBmYWxzZSwKICAgICJzbmkiOiAiY2RuMy5mcmVlZ3JhZGVseS54eXoiCn0=
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuNTcuNCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNkbjEuZnJlZWdyYWRlbHkueHl6IiwKICAgICJpZCI6ICJkNmI2ZDk4Mi1kNTJmLTQ2NWEtYjk4OC04NTY3MGIyM2Y2NGEiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICJnaXRodWIuY29tL0FsdmluOTk5OSIsCiAgICAicG9ydCI6IDIwNTIsCiAgICAicHMiOiAi8J+PgVJFTEFZLTEwNC4xOS41Ny40LTA0NDkiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxNjIuMTU5LjE0MC41NiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImlwMS4xNzg5MDM0Lnh5eiIsCiAgICAiaWQiOiAiZTllM2NjMTMtZGI0OC00Y2MxLThjMjQtNzYyNjQzOWE1MzM5IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDg2LAogICAgInBzIjogIvCfj4FSRUxBWS0xNjIuMTU5LjE0MC41Ni0xMTc1IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiBmYWxzZSwKICAgICJzbmkiOiAiaXAxLjE3ODkwMzQueHl6Igp9
    vmess://ewogICAgImFkZCI6ICIxMDQuMjYuNS4xMDMiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJpcDEuMTc4OTAzNC54eXoiLAogICAgImlkIjogImU5ZTNjYzEzLWRiNDgtNGNjMS04YzI0LTc2MjY0MzlhNTMzOSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA4NiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjI2LjUuMTAzLTExNzIiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IGZhbHNlLAogICAgInNuaSI6ICJpcDEuMTc4OTAzNC54eXoiCn0=
    vmess://ewogICAgImFkZCI6ICIxMDQuMjYuNS45MCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImlwMS4xNzg5MDM0Lnh5eiIsCiAgICAiaWQiOiAiZTllM2NjMTMtZGI0OC00Y2MxLThjMjQtNzYyNjQzOWE1MzM5IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDg2LAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMjYuNS45MC0xMTMzIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiBmYWxzZSwKICAgICJzbmkiOiAiaXAxLjE3ODkwMzQueHl6Igp9
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuNTguMTc1IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiY2RuMS5mcmVlZ3JhZGVseS54eXoiLAogICAgImlkIjogImQ2YjZkOTgyLWQ1MmYtNDY1YS1iOTg4LTg1NjcwYjIzZjY0YSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA1MiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjE5LjU4LjE3NS0wMzMwIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxMDQuMjYuNS4xMjMiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJpcDEuMTc4OTAzNC54eXoiLAogICAgImlkIjogImU5ZTNjYzEzLWRiNDgtNGNjMS04YzI0LTc2MjY0MzlhNTMzOSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA4NiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjI2LjUuMTIzLTExMzIiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IGZhbHNlLAogICAgInNuaSI6ICJpcDEuMTc4OTAzNC54eXoiCn0=
    vmess://ewogICAgImFkZCI6ICIxMDQuMTguNTcuMTIxIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiY2RuMi5mcmVlZ3JhZGVseS54eXoiLAogICAgImlkIjogImQ2YjZkOTgyLWQ1MmYtNDY1YS1iOTg4LTg1NjcwYjIzZjY0YSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA1MiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjE4LjU3LjEyMS0wMjc3IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxMDQuMjYuNS44OCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImlwMS4xNzg5MDM0Lnh5eiIsCiAgICAiaWQiOiAiZTllM2NjMTMtZGI0OC00Y2MxLThjMjQtNzYyNjQzOWE1MzM5IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDg2LAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMjYuNS44OC0xMTMxIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiBmYWxzZSwKICAgICJzbmkiOiAiaXAxLjE3ODkwMzQueHl6Igp9
    vmess://ewogICAgImFkZCI6ICIxMDQuMjYuNS4xMTIiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJpcDEuMTc4OTAzNC54eXoiLAogICAgImlkIjogImU5ZTNjYzEzLWRiNDgtNGNjMS04YzI0LTc2MjY0MzlhNTMzOSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA4NiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjI2LjUuMTEyLTExMjYiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuNDcuNjUiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJpcDE0LmZyZWVncmFkZWx5Lnh5eiIsCiAgICAiaWQiOiAiZTllM2NjMTMtZGI0OC00Y2MxLThjMjQtNzYyNjQzOWE1MzM5IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDg2LAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMTkuNDcuNjUtMDM0NyIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxNzIuNjQuMTk4LjIyOSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNkbjMuZnJlZWdyYWRlbHkueHl6IiwKICAgICJpZCI6ICJkNmI2ZDk4Mi1kNTJmLTQ2NWEtYjk4OC04NTY3MGIyM2Y2NGEiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICJnaXRodWIuY29tL0FsdmluOTk5OSIsCiAgICAicG9ydCI6IDIwNTIsCiAgICAicHMiOiAi8J+PgVJFTEFZLTE3Mi42NC4xOTguMjI5LTExOTgiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IGZhbHNlLAogICAgInNuaSI6ICJjZG4zLmZyZWVncmFkZWx5Lnh5eiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxMDQuMjYuNy4xMzIiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJjZG4xLmZyZWVncmFkZWx5Lnh5eiIsCiAgICAiaWQiOiAiZDZiNmQ5ODItZDUyZi00NjVhLWI5ODgtODU2NzBiMjNmNjRhIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDUyLAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMjYuNy4xMzItMDQ1MiIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxMDQuMjAuMTcuMTk2IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiY2RuMy5mcmVlZ3JhZGVseS54eXoiLAogICAgImlkIjogImQ2YjZkOTgyLWQ1MmYtNDY1YS1iOTg4LTg1NjcwYjIzZjY0YSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA1MiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjIwLjE3LjE5Ni0wMzgwIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxMDQuMTcuMTA2LjE3MSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNkbjIuZnJlZWdyYWRlbHkueHl6IiwKICAgICJpZCI6ICJkNmI2ZDk4Mi1kNTJmLTQ2NWEtYjk4OC04NTY3MGIyM2Y2NGEiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICJnaXRodWIuY29tL0FsdmluOTk5OSIsCiAgICAicG9ydCI6IDIwNTIsCiAgICAicHMiOiAi8J+PgVJFTEFZLTEwNC4xNy4xMDYuMTcxLTAzNDUiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuMjEuNzEiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJjZG4xLmZyZWVncmFkZWx5Lnh5eiIsCiAgICAiaWQiOiAiZDZiNmQ5ODItZDUyZi00NjVhLWI5ODgtODU2NzBiMjNmNjRhIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDUyLAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMTkuMjEuNzEtMDQzMiIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuNDYuMjciLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJpcDE0LmZyZWVncmFkZWx5Lnh5eiIsCiAgICAiaWQiOiAiZTllM2NjMTMtZGI0OC00Y2MxLThjMjQtNzYyNjQzOWE1MzM5IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDg2LAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMTkuNDYuMjctMDIyOSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuNDYuNjMiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJpcDIuMTQ1NzIzMC54eXoiLAogICAgImlkIjogImU5ZTNjYzEzLWRiNDgtNGNjMS04YzI0LTc2MjY0MzlhNTMzOSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA4NiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjE5LjQ2LjYzLTAyNzkiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxMDQuMTguNTcuMTExIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiaXAxMS5mcmVlZ3JhZGVseS54eXoiLAogICAgImlkIjogImU5ZTNjYzEzLWRiNDgtNGNjMS04YzI0LTc2MjY0MzlhNTMzOSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA4NiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjE4LjU3LjExMS0wMzU0IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiBmYWxzZSwKICAgICJzbmkiOiAiaXAxMS5mcmVlZ3JhZGVseS54eXoiCn0=
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuNDcuNjUiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJjZG4xLmZyZWVncmFkZWx5Lnh5eiIsCiAgICAiaWQiOiAiZDZiNmQ5ODItZDUyZi00NjVhLWI5ODgtODU2NzBiMjNmNjRhIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDUyLAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMTkuNDcuNjUtMDQ2OSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuMjEuNzMiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJjZG4zLmZyZWVncmFkZWx5Lnh5eiIsCiAgICAiaWQiOiAiZDZiNmQ5ODItZDUyZi00NjVhLWI5ODgtODU2NzBiMjNmNjRhIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDUyLAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMTkuMjEuNzMtMTIwMCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogZmFsc2UsCiAgICAic25pIjogImNkbjMuZnJlZWdyYWRlbHkueHl6Igp9
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuMjEuODEiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJjZG4xLmZyZWVncmFkZWx5Lnh5eiIsCiAgICAiaWQiOiAiZDZiNmQ5ODItZDUyZi00NjVhLWI5ODgtODU2NzBiMjNmNjRhIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDUyLAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMTkuMjEuODEtMDI3MiIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://YWVzLTI1Ni1nY206ZTRGQ1dyZ3BramkzUVk=@38.68.134.9:9102#%F0%9F%87%BA%F0%9F%87%B8US-38.68.134.9-6056
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuNTkuODkiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJpcDIuMTQ1NzIzMC54eXoiLAogICAgImlkIjogImU5ZTNjYzEzLWRiNDgtNGNjMS04YzI0LTc2MjY0MzlhNTMzOSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA4NiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjE5LjU5Ljg5LTAyMzEiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuNDUuMTciLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJpcDIuMTQ1NzIzMC54eXoiLAogICAgImlkIjogImU5ZTNjYzEzLWRiNDgtNGNjMS04YzI0LTc2MjY0MzlhNTMzOSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA4NiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjE5LjQ1LjE3LTExMDYiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuNDUuMzUiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJpcDEzLmZyZWVncmFkZWx5Lnh5eiIsCiAgICAiaWQiOiAiZTllM2NjMTMtZGI0OC00Y2MxLThjMjQtNzYyNjQzOWE1MzM5IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDg2LAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMTkuNDUuMzUtMDI4OCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuMzguMTIiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJjZG4xLmZyZWVncmFkZWx5Lnh5eiIsCiAgICAiaWQiOiAiZDZiNmQ5ODItZDUyZi00NjVhLWI5ODgtODU2NzBiMjNmNjRhIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDUyLAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMTkuMzguMTItMDI5MCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxNzIuNjQuMTc1LjIyMyIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNkbjMuZnJlZWdyYWRlbHkueHl6IiwKICAgICJpZCI6ICJkNmI2ZDk4Mi1kNTJmLTQ2NWEtYjk4OC04NTY3MGIyM2Y2NGEiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICJnaXRodWIuY29tL0FsdmluOTk5OSIsCiAgICAicG9ydCI6IDIwNTIsCiAgICAicHMiOiAi8J+PgVJFTEFZLTE3Mi42NC4xNzUuMjIzLTAyMTMiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://YWVzLTI1Ni1nY206S2l4THZLendqZWtHMDBybQ==@23.157.40.113:8080#%F0%9F%87%BA%F0%9F%87%B8US-23.157.40.113-0604
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuNDIuNDkiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJpcDE0LmZyZWVncmFkZWx5Lnh5eiIsCiAgICAiaWQiOiAiZTllM2NjMTMtZGI0OC00Y2MxLThjMjQtNzYyNjQzOWE1MzM5IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiZ2l0aHViLmNvbS9BbHZpbjk5OTkiLAogICAgInBvcnQiOiAyMDg2LAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMTkuNDIuNDktMDI4NiIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://YWVzLTI1Ni1nY206ZmFCQW9ENTRrODdVSkc3@38.114.114.69:2376#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.69-7389
    ss://YWVzLTI1Ni1nY206VEV6amZBWXEySWp0dW9T@38.114.114.69:6697#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.69-7008
    ss://YWVzLTI1Ni1nY206a0RXdlhZWm9UQmNHa0M0@38.114.114.69:8882#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.69-6962
    ss://YWVzLTI1Ni1nY206Y2RCSURWNDJEQ3duZklO@38.114.114.69:8118#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.69-7618
    ss://YWVzLTI1Ni1nY206S2l4THZLendqZWtHMDBybQ==@38.114.114.69:8000#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.69-6968
    ss://YWVzLTI1Ni1nY206ZmFCQW9ENTRrODdVSkc3@23.157.40.102:2375#%F0%9F%87%BA%F0%9F%87%B8US-23.157.40.102-0550
    ss://YWVzLTI1Ni1nY206cEtFVzhKUEJ5VFZUTHRN@38.114.114.69:443#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.69-6255
    ss://YWVzLTI1Ni1nY206ZTRGQ1dyZ3BramkzUVk=@38.114.114.69:9102#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.69-7733
    ss://YWVzLTI1Ni1nY206UmV4bkJnVTdFVjVBRHhH@38.114.114.69:7001#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.69-6888
    ss://YWVzLTI1Ni1nY206WTZSOXBBdHZ4eHptR0M=@38.121.43.71:5000#%F0%9F%87%BA%F0%9F%87%B8US-38.121.43.71-5192
    ss://YWVzLTI1Ni1nY206S2l4THZLendqZWtHMDBybQ==@38.114.114.69:5500#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.69-7154
    ss://YWVzLTI1Ni1nY206UmV4bkJnVTdFVjVBRHhH@38.114.114.69:7002#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.69-7661
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuNDUuMTEiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJpcDEuMTQ1NzIzMC54eXoiLAogICAgImlkIjogImU5ZTNjYzEzLWRiNDgtNGNjMS04YzI0LTc2MjY0MzlhNTMzOSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA4NiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjE5LjQ1LjExLTAyNTgiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://YWVzLTI1Ni1nY206Y2RCSURWNDJEQ3duZklO@38.114.114.69:8119#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.69-6562
    ss://YWVzLTI1Ni1nY206WTZSOXBBdHZ4eHptR0M=@23.157.40.113:8888#%F0%9F%87%BA%F0%9F%87%B8US-23.157.40.113-0610
    ss://YWVzLTI1Ni1nY206VEV6amZBWXEySWp0dW9T@38.114.114.69:6679#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.69-7471
    ss://YWVzLTI1Ni1nY206Rm9PaUdsa0FBOXlQRUdQ@38.68.135.19:7306#%F0%9F%87%BA%F0%9F%87%B8US-38.68.135.19-6239
    ss://YWVzLTI1Ni1nY206ekROVmVkUkZQUWV4Rzl2@38.114.114.69:6379#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.69-7620
    ss://YWVzLTI1Ni1nY206a0RXdlhZWm9UQmNHa0M0@23.157.40.10:8881#%F0%9F%87%BA%F0%9F%87%B8US-23.157.40.10-0563
    ss://YWVzLTI1Ni1nY206WTZSOXBBdHZ4eHptR0M=@38.143.66.87:3306#%F0%9F%87%BA%F0%9F%87%B8US-38.143.66.87-7502
    ss://YWVzLTI1Ni1nY206WTZSOXBBdHZ4eHptR0M=@23.157.40.10:5000#%F0%9F%87%BA%F0%9F%87%B8US-23.157.40.10-0555
    ss://YWVzLTI1Ni1nY206Y2RCSURWNDJEQ3duZklO@23.157.40.113:8118#%F0%9F%87%BA%F0%9F%87%B8US-23.157.40.113-0605
    ss://YWVzLTI1Ni1nY206ZmFCQW9ENTRrODdVSkc3@38.68.135.19:2375#%F0%9F%87%BA%F0%9F%87%B8US-38.68.135.19-6243
    ss://YWVzLTI1Ni1nY206Y2RCSURWNDJEQ3duZklO@23.157.40.113:8119#%F0%9F%87%BA%F0%9F%87%B8US-23.157.40.113-0608
    ss://YWVzLTI1Ni1nY206Y2RCSURWNDJEQ3duZklO@23.157.40.10:8119#%F0%9F%87%BA%F0%9F%87%B8US-23.157.40.10-0613
    ss://YWVzLTI1Ni1nY206ekROVmVkUkZQUWV4Rzl2@38.68.134.9:6379#%F0%9F%87%BA%F0%9F%87%B8US-38.68.134.9-6057
    ss://YWVzLTI1Ni1nY206Rm9PaUdsa0FBOXlQRUdQ@38.114.114.69:7307#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.69-7452
    ss://YWVzLTI1Ni1nY206WTZSOXBBdHZ4eHptR0M=@38.68.134.9:3306#%F0%9F%87%BA%F0%9F%87%B8US-38.68.134.9-6049
    ss://YWVzLTI1Ni1nY206WEtGS2wyclVMaklwNzQ=@38.114.114.69:8008#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.69-6943
    ss://YWVzLTI1Ni1nY206WEtGS2wyclVMaklwNzQ=@38.114.114.69:8009#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.69-7005
    ss://YWVzLTI1Ni1nY206WTZSOXBBdHZ4eHptR0M=@23.157.40.115:8888#%F0%9F%87%BA%F0%9F%87%B8US-23.157.40.115-0559
    ss://YWVzLTI1Ni1nY206WTZSOXBBdHZ4eHptR0M=@23.157.40.47:3389#%F0%9F%87%BA%F0%9F%87%B8US-23.157.40.47-1235
    ss://YWVzLTI1Ni1nY206ekROVmVkUkZQUWV4Rzl2@38.68.135.19:6379#%F0%9F%87%BA%F0%9F%87%B8US-38.68.135.19-6246
    ss://YWVzLTI1Ni1nY206cEtFVzhKUEJ5VFZUTHRN@38.114.114.143:443#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.143-6043
    ss://YWVzLTI1Ni1nY206WTZSOXBBdHZ4eHptR0M=@38.114.114.69:5601#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.69-7137
    ss://YWVzLTI1Ni1nY206WTZSOXBBdHZ4eHptR0M=@38.68.134.9:3389#%F0%9F%87%BA%F0%9F%87%B8US-38.68.134.9-6059
    ss://YWVzLTI1Ni1nY206ZTRGQ1dyZ3BramkzUVk=@38.68.135.19:9102#%F0%9F%87%BA%F0%9F%87%B8US-38.68.135.19-6665
    vmess://ewogICAgImFkZCI6ICIxMDQuMTkuMjEuMjMwIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiY2RuMS5mcmVlZ3JhZGVseS54eXoiLAogICAgImlkIjogImQ2YjZkOTgyLWQ1MmYtNDY1YS1iOTg4LTg1NjcwYjIzZjY0YSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogImdpdGh1Yi5jb20vQWx2aW45OTk5IiwKICAgICJwb3J0IjogMjA1MiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjE5LjIxLjIzMC0xMTM0IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiBmYWxzZSwKICAgICJzbmkiOiAiY2RuMS5mcmVlZ3JhZGVseS54eXoiCn0=
    ss://YWVzLTI1Ni1nY206cEtFVzhKUEJ5VFZUTHRN@38.114.114.69:4444#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.69-7385
    ss://YWVzLTI1Ni1nY206Rm9PaUdsa0FBOXlQRUdQ@38.121.43.71:7307#%F0%9F%87%BA%F0%9F%87%B8US-38.121.43.71-6693
    ss://YWVzLTI1Ni1nY206VEV6amZBWXEySWp0dW9T@38.143.66.87:6697#%F0%9F%87%BA%F0%9F%87%B8US-38.143.66.87-7580
    ss://YWVzLTI1Ni1nY206WEtGS2wyclVMaklwNzQ=@38.68.134.9:8009#%F0%9F%87%BA%F0%9F%87%B8US-38.68.134.9-7701
    ss://YWVzLTI1Ni1nY206ZmFCQW9ENTRrODdVSkc3@38.121.43.51:2376#%F0%9F%87%BA%F0%9F%87%B8US-38.121.43.51-6042
    ss://YWVzLTI1Ni1nY206WTZSOXBBdHZ4eHptR0M=@23.157.40.10:5001#%F0%9F%87%BA%F0%9F%87%B8US-23.157.40.10-0575
    ss://YWVzLTI1Ni1nY206Y2RCSURWNDJEQ3duZklO@38.68.135.19:8119#%F0%9F%87%BA%F0%9F%87%B8US-38.68.135.19-2856
    ss://YWVzLTI1Ni1nY206Y2RCSURWNDJEQ3duZklO@23.157.40.102:8118#%F0%9F%87%BA%F0%9F%87%B8US-23.157.40.102-0543
    ss://YWVzLTI1Ni1nY206UmV4bkJnVTdFVjVBRHhH@38.68.135.19:7001#%F0%9F%87%BA%F0%9F%87%B8US-38.68.135.19-7369
    ss://YWVzLTI1Ni1nY206ZzVNZUQ2RnQzQ1dsSklk@38.68.135.19:5003#%F0%9F%87%BA%F0%9F%87%B8US-38.68.135.19-6728
    ss://YWVzLTI1Ni1nY206ZzVNZUQ2RnQzQ1dsSklk@38.114.114.69:5003#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.69-6521
    ss://YWVzLTI1Ni1nY206a0RXdlhZWm9UQmNHa0M0@23.157.40.113:8882#%F0%9F%87%BA%F0%9F%87%B8US-23.157.40.113-0609
    ss://YWVzLTI1Ni1nY206WTZSOXBBdHZ4eHptR0M=@38.68.134.9:5600#%F0%9F%87%BA%F0%9F%87%B8US-38.68.134.9-6045
    ss://YWVzLTI1Ni1nY206S2l4THZLendqZWtHMDBybQ==@38.68.135.19:5500#%F0%9F%87%BA%F0%9F%87%B8US-38.68.135.19-6702
    ss://YWVzLTI1Ni1nY206WTZSOXBBdHZ4eHptR0M=@38.143.66.87:5000#%F0%9F%87%BA%F0%9F%87%B8US-38.143.66.87-6874

    vmess://ewogICAgImFkZCI6ICJ3d3cuZ292LmhrIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAibGludXMuY2xvdWRmbGFyZS5xdWVzdCIsCiAgICAiaWQiOiAiMWFiOTFmMTgtNjE2OC00Y2I2LWM5Y2EtMmMzYzcxNThmZTRjIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2FyaWVzIiwKICAgICJwb3J0IjogMjA4NiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjE2LjI0OS4xMzAtMTMwMSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://YWVzLTEyOC1jZmI6c2hhZG93c29ja3M=@156.146.38.163:443#%F0%9F%87%BA%F0%9F%87%B8US-156.146.38.163-0799
    vmess://ewogICAgImFkZCI6ICJ4ci0xLmhlcm9rdWFwcC5jb20iLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJ4ci0xLmhlcm9rdWFwcC5jb20iLAogICAgImlkIjogIjE3YWY3NmUxLWE1ZDctNDFhYi1hZTg3LWI0OGYxODUwNzVkMSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi8xN2FmNzZlMS1hNWQ3LTQxYWItYWU4Ny1iNDhmMTg1MDc1ZDEtdm1lc3MiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HuvCfh7hVUy01NC4yNDMuMTI5LjIxNS0xOTA1MCIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDM=@172.96.192.58:254#%F0%9F%87%BA%F0%9F%87%B8US-172.96.192.58-0463
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDM=@97.64.31.80:247#%F0%9F%87%BA%F0%9F%87%B8US-97.64.31.80-0461
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDM=@144.168.60.70:252#%F0%9F%87%BA%F0%9F%87%B8US-144.168.60.70-15607
    vmess://ewogICAgImFkZCI6ICIxNDEuMTAxLjExNC4yMCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNsYXNoMS50cnVtcDIwMjMubmV0IiwKICAgICJpZCI6ICIxNzZiNTk4Zi00NDViLTQxYWMtOWQyYS00MzBjNWM0ZGYyNmEiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvZG9uZ3RhaXdhbmcuY29tIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfj4FSRUxBWS0xNDEuMTAxLjExNC4yMC0wMjk0IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDU=@172.96.192.100:246#%F0%9F%87%BA%F0%9F%87%B8US-172.96.192.100-15615
    vmess://ewogICAgImFkZCI6ICI2Ny4yMS43Mi40MSIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICJ3d3cuMTcwODAxMDAueHl6IiwKICAgICJpZCI6ICIyNTY2ZDAwZi0yMThjLTQ4ZjctOWEzNi0xM2QzZDZmMWE3MjQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvcGF0aC8xNzM0MTgxNDExMjMiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HuvCfh7hVUy02Ny4yMS43Mi40MS01NTE4IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDY=@95.169.4.174:254#%F0%9F%87%BA%F0%9F%87%B8US-95.169.4.174-15616
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDM=@104.243.25.95:253#%F0%9F%87%BA%F0%9F%87%B8US-104.243.25.95-0436
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDU=@144.168.58.170:254#%F0%9F%87%BA%F0%9F%87%B8US-144.168.58.170-15618
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDU=@107.182.177.136:256#%F0%9F%87%BA%F0%9F%87%B8US-107.182.177.136-0659
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDY=@93.179.112.70:253#%F0%9F%87%BA%F0%9F%87%B8US-93.179.112.70-15619
    vmess://ewogICAgImFkZCI6ICI2Ny4yMS43Mi40MSIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICI2Ny4yMS43Mi40MSIsCiAgICAiaWQiOiAiMjU2NmQwMGYtMjE4Yy00OGY3LTlhMzYtMTNkM2Q2ZjFhNzI0IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL3BhdGgvMTczNDE4MTQxMTIzIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfh7rwn4e4VVMtNjcuMjEuNzIuNDEtOTg3OCIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDU=@97.64.122.63:253#%F0%9F%87%BA%F0%9F%87%B8US-97.64.122.63-15606
    vmess://ewogICAgImFkZCI6ICI2Ny4yMS43Mi40MSIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjI1NjZkMDBmLTIxOGMtNDhmNy05YTM2LTEzZDNkNmYxYTcyNCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9wYXRoLzE3MzQxODE0MTEyMyIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4e68J+HuFVTLTY3LjIxLjcyLjQxLTQ4OTQiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICJ2dXMyLjBiYWQuY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAidnVzMi4wYmFkLmNvbSIsCiAgICAiaWQiOiAiOTI3MDk0ZDMtZDY3OC00NzYzLTg1OTEtZTI0MGQwYmNhZTg3IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2NoYXQiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HuvCfh7hVUy00NS4zMy4xMDUuMjM5LTEwODE3IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICJ2dXMzLjBiYWQuY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAidnVzMy4wYmFkLmNvbSIsCiAgICAiaWQiOiAiOTI3MDk0ZDMtZDY3OC00NzYzLTg1OTEtZTI0MGQwYmNhZTg3IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2NoYXQiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HuvCfh7hVUy00NS43OS4yMjQuNTMtMTExNyIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICI2Ny4yMS43Mi40NCIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICJ3d3cuNDg4MTY2MjYueHl6IiwKICAgICJpZCI6ICIyNTY2ZDAwZi0yMThjLTQ4ZjctOWEzNi0xM2QzZDZmMWE3MjQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvcGF0aC8xMjAyMDgzMDE0MjIiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HuvCfh7hVUy02Ny4yMS43Mi40NC00ODkxIiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDU=@198.181.56.163:238#%F0%9F%87%BA%F0%9F%87%B8US-198.181.56.163-15629
    vmess://ewogICAgImFkZCI6ICI2Ny4yMS43Mi40NCIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjI1NjZkMDBmLTIxOGMtNDhmNy05YTM2LTEzZDNkNmYxYTcyNCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9wYXRoLzEyMDIwODMwMTQyMiIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4e68J+HuFVTLTY3LjIxLjcyLjQ0LTEwMzA5IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICI2Ny4yMS43Mi40NCIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICI2Ny4yMS43Mi40NCIsCiAgICAiaWQiOiAiMjU2NmQwMGYtMjE4Yy00OGY3LTlhMzYtMTNkM2Q2ZjFhNzI0IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL3BhdGgvMTIwMjA4MzAxNDIyIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfh7rwn4e4VVMtNjcuMjEuNzIuNDQtMTAyODEiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.198:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.198-0803
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.79:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.79-0800
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.193:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.193-0998
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.81:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.81-0561
    trojan://e23f408a-012e-4030-8b31-02022031cb50@fhcamd1.gaox.ml:443?allowInsecure=1#%F0%9F%87%BA%F0%9F%87%B8US-129.146.135.157-16738
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.194:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.194-0535
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.195:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.195-0802
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.78:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.78-0533
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.196:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.196-1355
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.80:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.80-0997
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.197:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.197-0562
    vmess://ewogICAgImFkZCI6ICIxMjkuMTU5LjQxLjIzMyIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiMzQxYTkxODItYzQyMy00OTljLWM0NmUtZDE3ODM4YjI5MDM3IiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDMyNTg2LAogICAgInBzIjogIvCfh7rwn4e4VVMtMTI5LjE1OS40MS4yMzMtMDIzOSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxMjkuMTQ2LjEzMy4xNTciLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjgxNzE0Y2VmLTliZGUtNGEwOC1hYTUwLWQ2YmMwMTcyZDc4YiIsCiAgICAibmV0IjogInRjcCIsCiAgICAicGF0aCI6ICIiLAogICAgInBvcnQiOiA1MTAwOSwKICAgICJwcyI6ICLwn4e68J+HuFVTLTEyOS4xNDYuMTMzLjE1Ny0wMjc1IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxNzIuNjQuMTU0LjE1MCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNsYXNoNi5zc3ItZnJlZS54eXoiLAogICAgImlkIjogIjVmNjRmYTY1LTdiMTQtNDljNS05NTRkLWFhMTVjNmJmY2FjZCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9kb25ndGFpd2FuZy5jb20iLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTE3Mi42NC4xNTQuMTUwLTAyNTEiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@78.129.253.9:808#%F0%9F%87%AC%F0%9F%87%A7GB-78.129.253.9-15647
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@78.129.253.9:809#%F0%9F%87%AC%F0%9F%87%A7GB-78.129.253.9-1394
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDE=@65.49.204.125:254#%F0%9F%87%BA%F0%9F%87%B8US-65.49.204.125-15627
    vmess://ewogICAgImFkZCI6ICJ2dWsyLjBiYWQuY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAidnVrMi4wYmFkLmNvbSIsCiAgICAiaWQiOiAiOTI3MDk0ZDMtZDY3OC00NzYzLTg1OTEtZTI0MGQwYmNhZTg3IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2NoYXQiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HrPCfh6dHQi0xMDkuNzQuMTk0LjIwOC0xMjQ5IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.161.118.38:808#%F0%9F%87%A8%F0%9F%87%A6CA-51.161.118.38-15739
    vmess://ewogICAgImFkZCI6ICIxNzIuNjQuMTU1LjIwMSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNsYXNoMy50cnVtcDIwMjMub3JnIiwKICAgICJpZCI6ICIyOGRhZDY5Yy1jOWQ2LTQ3YzUtYWQwNS1jNjZhZmI4N2NjYmQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvZG9uZ3RhaXdhbmcuY29tIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfj4FSRUxBWS0xNzIuNjQuMTU1LjIwMS0wMjY2IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxOTguNDEuMjEyLjEwMCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImZyMS5jZmNkbjEueHl6IiwKICAgICJpZCI6ICJmYjViYmM4Yy1mNmVjLTQ2MjktOGM5ZS0yM2YwMjc4MWEyMGQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvZG9uZ3RhaXdhbmcuY29tIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfj4FSRUxBWS0xOTguNDEuMjEyLjEwMC04NjEwIiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.161.118.38:800#%F0%9F%87%A8%F0%9F%87%A6CA-51.161.118.38-15732
    vmess://ewogICAgImFkZCI6ICJ2ZGUxLjBiYWQuY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAidmRlMS4wYmFkLmNvbSIsCiAgICAiaWQiOiAiOTI3MDk0ZDMtZDY3OC00NzYzLTg1OTEtZTI0MGQwYmNhZTg3IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2NoYXQiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HqfCfh6pERS0xNzIuMTA1LjI0NS43OS0wMjk4IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICJ2ZGUyLjBiYWQuY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAidmRlMi4wYmFkLmNvbSIsCiAgICAiaWQiOiAiOTI3MDk0ZDMtZDY3OC00NzYzLTg1OTEtZTI0MGQwYmNhZTg3IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2NoYXQiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HqfCfh6pERS0xMzkuMTQ0LjE3Ni43Ni0xMjgwIiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@134.195.196.178:804#%F0%9F%87%A8%F0%9F%87%A6CA-134.195.196.178-14790
    vmess://ewogICAgImFkZCI6ICJzdHJlYW0uYXphZHJhaDIyLmNvbSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInN0cmVhbS5hemFkcmFoMjIuY29tIiwKICAgICJpZCI6ICI3NmUxNTFhNy05OTgwLTQwNzctYmQ1Mi0wN2VmNGU5Y2I0OTYiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvdXNlciIsCiAgICAicG9ydCI6IDgwLAogICAgInBzIjogIvCfh67wn4e3SVItMTg1LjE0My4yMzQuMTIwLTE5NDk5IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.161.118.38:805#%F0%9F%87%A8%F0%9F%87%A6CA-51.161.118.38-15756
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.161.118.38:806#%F0%9F%87%A8%F0%9F%87%A6CA-51.161.118.38-15744
    vmess://ewogICAgImFkZCI6ICJzdHVkeW5ldy5jbiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInN0dWR5bmV3LmNuIiwKICAgICJpZCI6ICJiYjg0NzI1YS1mNzI2LTRiY2ItODEzMS00NGRmMTIwOTQwMDUiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvZGVuZ3FpbmdibyIsCiAgICAicG9ydCI6IDUxMzQwLAogICAgInBzIjogIvCfh7rwn4e4VVMtMTk4LjE0OC4xMjcuNjItOTgxOSIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICI4NS4xNy41LjE1MCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIjg1LjE3LjUuMTUwIiwKICAgICJpZCI6ICI0MDcwZmRkZS00M2Q1LTRiM2YtZGJjZi03NzUxYzc3ZTRiZjYiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvQWY1NjQ1dHIiLAogICAgInBvcnQiOiAzNjMwNiwKICAgICJwcyI6ICLwn4ez8J+HsU5MLTg1LjE3LjUuMTUwLTExNjE4IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICI4NS4xNy41LjE1MCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiNDA3MGZkZGUtNDNkNS00YjNmLWRiY2YtNzc1MWM3N2U0YmY2IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL0FmNTY0NXRyIiwKICAgICJwb3J0IjogMzYzMDYsCiAgICAicHMiOiAi8J+Hs/Cfh7FOTC04NS4xNy41LjE1MC0xMTYxMCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.161.118.38:801#%F0%9F%87%A8%F0%9F%87%A6CA-51.161.118.38-15782
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:807#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0966
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:811#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-2149
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@194.71.126.31:989#%F0%9F%87%B7%F0%9F%87%B8RS-194.71.126.31-0408
    vmess://ewogICAgImFkZCI6ICIxNDEuMTAxLjExNS4xMjAiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJsZzEuY2ZjZG4zLnh5eiIsCiAgICAiaWQiOiAiMzNhYTU3ZGYtMWM5My00MzE4LTlmY2UtZTg1MDQzN2VlNzgxIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2Rvbmd0YWl3YW5nLmNvbSIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4+BUkVMQVktMTQxLjEwMS4xMTUuMTIwLTEyMzQiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    trojan://8b6daf15-8342-482d-b894-1239fd98ce7f@149.56.141.11:443?allowInsecure=1#%F0%9F%87%A8%F0%9F%87%A6CA-149.56.141.11-0319
    ssr://NDUuMTU0LjIxNS4xMzU6MzE1ODA6YXV0aF9hZXMxMjhfc2hhMTphZXMtMjU2LWNmYjp0bHMxLjJfdGlja2V0X2F1dGg6ZW5oUGJXUkUvP29iZnNwYXJhbT1WbTB4TkdFd01VaFNXR2hVVjBkNFYxbHJaRk5XYkd4VlUycFNXRkp0ZUhwWGEyTTFZV3hLZEdWSWNGaGhNVlV4VmtkNFlXTXhXbkZXYkZaWFlsZG9VVmRXVm1GVGJWRjVWR3RXVW1KSGFGbFZha0YzJnJlbWFya3M9OEolMkJIdXZDZmg3aFZVeTAwTlM0eE5UUXVNakUxTGpFek5TMHlNemcxJnByb3RvcGFyYW09TWpJMk5qTTZVWEZNYjJGWg==
    vmess://ewogICAgImFkZCI6ICI1MS44OS40Mi4xNTQiLAogICAgImFpZCI6IDY0LAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICI0MTgwNDhhZi1hMjkzLTRiOTktOWIwYy05OGNhMzU4MGRkMjQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvcGF0aC8xMjAyMTEzMzE0MjIiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HrPCfh6dHQi01MS44OS40Mi4xNTQtMTY5ODkiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    trojan://8b6daf15-8342-482d-b894-1239fd98ce7f@cat1.sshocean.net:443?allowInsecure=1#%F0%9F%87%A8%F0%9F%87%A6CA-149.56.141.11-0241
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTo5N09uREVaWUdqYTQ=@178.18.244.2:443#%F0%9F%87%A9%F0%9F%87%AADE-178.18.244.2-0756
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpzaUY5OHhCTDJ2MWk=@135.181.114.242:8478#%F0%9F%87%AB%F0%9F%87%AEFI-135.181.114.242-0798
    ss://YWVzLTI1Ni1jZmI6R2VyZWdldFI4Y3ZRSHpZcg==@213.183.53.221:9030#%F0%9F%87%B7%F0%9F%87%BARU-213.183.53.221-15695
    ss://YWVzLTI1Ni1jZmI6ZjhucEtnTnpka3NzMnl0bg==@213.183.53.221:9088#%F0%9F%87%B7%F0%9F%87%BARU-213.183.53.221-15694
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTopMU4xRTZ2MFNVX3JHVHBn@38.64.138.53:1035#%F0%9F%87%BA%F0%9F%87%B8US-38.64.138.53-0573
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.47:805#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.47-0761
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.161.118.38:812#%F0%9F%87%A8%F0%9F%87%A6CA-51.161.118.38-15779
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpXYWN3ZXRDaWY=@217.12.223.190:444#%F0%9F%87%BA%F0%9F%87%A6UA-217.12.223.190-0790
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.154:808#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.154-13651
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@5.188.0.151:800#%F0%9F%87%BA%F0%9F%87%B8US-5.188.0.151-15704
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@ak1466.free.www.outline.network:811#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.156-7643
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:809#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0566
    ssr://anAtYW00OC02LmVxbm9kZS5uZXQ6ODA4MTpvcmlnaW46YWVzLTI1Ni1jZmI6dGxzMS4yX3RpY2tldF9hdXRoOlpVRnZhMkpoUkU0Mi8/b2Jmc3BhcmFtPSZyZW1hcmtzPThKJTJCSHIlMkZDZmg3VktVQzAxTkM0Mk5DNDFOeTR6TkMwd05UYzQmcHJvdG9wYXJhbT0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.154:805#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.154-15687
    vmess://ewogICAgImFkZCI6ICI1MS44OS40Mi4xNTQiLAogICAgImFpZCI6IDY0LAogICAgImhvc3QiOiAiNTEuODkuNDIuMTU0IiwKICAgICJpZCI6ICI0MTgwNDhhZi1hMjkzLTRiOTktOWIwYy05OGNhMzU4MGRkMjQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvcGF0aC8xMjAyMTEzMzE0MjIiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HrPCfh6dHQi01MS44OS40Mi4xNTQtMTEzNTciLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxNDEuMTAxLjExNS4yIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiZnIxLmNmY2RuMS54eXoiLAogICAgImlkIjogImZiNWJiYzhjLWY2ZWMtNDYyOS04YzllLTIzZjAyNzgxYTIwZCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9kb25ndGFpd2FuZy5jb20iLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTE0MS4xMDEuMTE1LjItMDI0NCIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxNTAuMjMwLjE5OS4xNzciLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjZiNzQ1Y2FmLWU3ZjYtNDlmMS05YjYzLWU1YzQxNjMwM2JhYyIsCiAgICAibmV0IjogInRjcCIsCiAgICAicGF0aCI6ICIiLAogICAgInBvcnQiOiAyMTY5NiwKICAgICJwcyI6ICLwn4ev8J+HtUpQLTE1MC4yMzAuMTk5LjE3Ny0wMjM3IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxNDQuMjQuODguMTAxIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJmNTQyNWNjZi0zOTQ2LTRmYjQtZWIyNC01MzkzZDc4YTM5MmYiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMTY4MzMsCiAgICAicHMiOiAi8J+HsPCfh7dLUi0xNDQuMjQuODguMTAxLTA0NzYiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@134.195.196.143:802#%F0%9F%87%A8%F0%9F%87%A6CA-134.195.196.143-15751
    vmess://ewogICAgImFkZCI6ICIxMzguMi4xNS4yMyIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiOTk4MTUxZTUtMGJjNS00Mzc3LWUzOTAtYzQxYmIyNmZkZDBjIiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDQ2MzcwLAogICAgInBzIjogIvCfh6/wn4e1SlAtMTM4LjIuMTUuMjMtMDI5MCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICJ2bTEyLmxlaWZlbmdrZWppLmxpdmUiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJ2bTEyLmxlaWZlbmdrZWppLmxpdmUiLAogICAgImlkIjogIjc1MmE5NDA0LWM3MjktNDg1ZS04ZWE1LWFjYjNmNGZjODE4MCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi8iLAogICAgInBvcnQiOiAxMTExMSwKICAgICJwcyI6ICLwn4ew8J+Ht0tSLTQzLjIwMS4zOC4xOTMtMTI5OSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICJ2bTUubGVpZmVuZ2tlamkubGl2ZSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInZtNS5sZWlmZW5na2VqaS5saXZlIiwKICAgICJpZCI6ICI3NTJhOTQwNC1jNzI5LTQ4NWUtOGVhNS1hY2IzZjRmYzgxODAiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvIiwKICAgICJwb3J0IjogMTExMTEsCiAgICAicHMiOiAi8J+HsPCfh7dLUi0xMy4yMDkuNC4yMTEtMDIyOCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    trojan://752a9404-c729-485e-8ea5-acb3f4fc8180@hg5.leifengkeji.live:48903?allowInsecure=1#%F0%9F%87%B0%F0%9F%87%B7KR-43.200.4.201-11721
    vmess://ewogICAgImFkZCI6ICIxNTIuNzAuMjQxLjE4IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJlY2QyNzRjMC0xNzVkLTQ1ZjctODI3Ni1hM2RhOTM3ODY2MzIiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMjY2NzYsCiAgICAicHMiOiAi8J+HsPCfh7dLUi0xNTIuNzAuMjQxLjE4LTAzMjgiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxOTIuNzQuMjQyLjE4MiIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjQxODA0OGFmLWEyOTMtNGI5OS05YjBjLTk4Y2EzNTgwZGQyNCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9wYXRoLzE3MDQxOTExMTAyMSIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4e68J+HuFVTLTE5Mi43NC4yNDIuMTgyLTE2NjgzIiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICJ3d3cuMzIzMzgwNzUueHl6Igp9
    vmess://ewogICAgImFkZCI6ICJ2bTgubGVpZmVuZ2tlamkubGl2ZSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInZtOC5sZWlmZW5na2VqaS5saXZlIiwKICAgICJpZCI6ICI3NTJhOTQwNC1jNzI5LTQ4NWUtOGVhNS1hY2IzZjRmYzgxODAiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvIiwKICAgICJwb3J0IjogMTExMTEsCiAgICAicHMiOiAi8J+HsPCfh7dLUi0xNS4xNjQuMTYzLjE0LTExODg0IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    trojan://752a9404-c729-485e-8ea5-acb3f4fc8180@hg17.leifengkeji.live:33387?allowInsecure=1&sni=hg17.leifengkeji.live#%F0%9F%87%B0%F0%9F%87%B7KR-15.164.103.48-0255
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:803#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0571
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@134.195.196.143:805#%F0%9F%87%A8%F0%9F%87%A6CA-134.195.196.143-15766
    vmess://ewogICAgImFkZCI6ICIxNDYuNTYuMTU1LjcwIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJmOTc3MWMxOS1jOTFjLTQxYjUtOTA2NC04NzY4YjUxY2VjNmQiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMTgwNTAsCiAgICAicHMiOiAi8J+HsPCfh7dLUi0xNDYuNTYuMTU1LjcwLTAzMjUiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.154:801#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.154-15760
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.154:803#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.154-15754
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:802#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0537
    trojan://0Y9gOHSdRt@150.230.249.42:443?allowInsecure=1#%F0%9F%87%B0%F0%9F%87%B7KR-150.230.249.42-0291
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.147.230:805#%F0%9F%87%BA%F0%9F%87%B8US-37.120.147.230-0771
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.154:800#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.154-15677
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:806#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0553
    vmess://ewogICAgImFkZCI6ICIxNTIuNjcuMjE4LjM4IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiWW91VHViZS1hd2Vpa2VqaSIsCiAgICAiaWQiOiAiYjVlOTQ4MGEtYjdhYS00MGE0LWY5YTctNTI5OWI1ZTM2M2I0IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiLyIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4ew8J+Ht0tSLTE1Mi42Ny4yMTguMzgtMTU1NDUiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:800#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0543
    vmess://ewogICAgImFkZCI6ICI4LjIwOS4yMTguMTk1IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAibGluZG8uY25hYmMuZXUub3JnIiwKICAgICJpZCI6ICJmNmQ3YjA3Mi1kZTAwLTQ1ZGMtOWUyNC00OWY4Y2Y0MzUzMGQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvbGlub2QiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+Hr/Cfh7VKUC04LjIwOS4yMTguMTk1LTAzMjYiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICJ2bTE1LmxlaWZlbmdrZWppLmxpdmUiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJ2bTE1LmxlaWZlbmdrZWppLmxpdmUiLAogICAgImlkIjogIjc1MmE5NDA0LWM3MjktNDg1ZS04ZWE1LWFjYjNmNGZjODE4MCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi8iLAogICAgInBvcnQiOiAxMTExMSwKICAgICJwcyI6ICLwn4ew8J+Ht0tSLTU0LjE4MC4xMDEuNi0wMjkzIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICJhZWFkanBhZXMwMS54bi0tejRxNDhsY3ZwLmNvbSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInNob3V0aW5ndG91dGlhbzMuMTAwMTAuY29tIiwKICAgICJpZCI6ICIzZTgyMGViMC0zZjA2LTQzMzctYTRmYy0wYzNjN2MwZDNiNGQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvaW1hZ2VzIiwKICAgICJwb3J0IjogODAsCiAgICAicHMiOiAi8J+Hr/Cfh7VKUC0xNzIuMTA0Ljc5Ljk2LTE2MTA3IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxNTIuNjcuMjE4LjM4IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiMTUyLjY3LjIxOC4zOCIsCiAgICAiaWQiOiAiYjVlOTQ4MGEtYjdhYS00MGE0LWY5YTctNTI5OWI1ZTM2M2I0IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiLyIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4ew8J+Ht0tSLTE1Mi42Ny4yMTguMzgtMDIyNCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxMjkuMTU0LjU3LjEzNCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiY2FiYmRmNWQtM2NjYS00NjA1LWJhMWMtYzg5YTdkNWI0YzA3IiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDI2MjgyLAogICAgInBzIjogIvCfh7Dwn4e3S1ItMTI5LjE1NC41Ny4xMzQtMDMyMyIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTp2QXBZaUFnaHplc0g=@217.70.188.60:855#%F0%9F%87%AB%F0%9F%87%B7FR-217.70.188.60-15709
    vmess://ewogICAgImFkZCI6ICI1MS44OS40Mi4xNTQiLAogICAgImFpZCI6IDY0LAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICI0MTgwNDhhZi1hMjkzLTRiOTktOWIwYy05OGNhMzU4MGRkMjQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvcGF0aC8xMjAyMTEzMzE0MjIiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HrPCfh6dHQi01MS44OS40Mi4xNTQtMjM3OSIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICJtNC40MDAxMDAxMC54eXoiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjU3NWU0ZDkyLTEwNTYtNDRjMi04Y2FjLTc1ZWYxYzg1OWFkNSIsCiAgICAibmV0IjogInRjcCIsCiAgICAicGF0aCI6ICIiLAogICAgInBvcnQiOiAzNzEyMSwKICAgICJwcyI6ICLwn4ew8J+Ht0tSLTE0Ni41Ni4xMzMuMTA5LTAyODUiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.147.230:800#%F0%9F%87%BA%F0%9F%87%B8US-37.120.147.230-10336
    vmess://ewogICAgImFkZCI6ICJ3d3cuYXB1bG5pb24uY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAid3d3LmFwdWxuaW9uLmNvbSIsCiAgICAiaWQiOiAiN2I4YzM3MGQtODYxMC00OTg4LWIwYTctY2RlNzRhYTA3MTNiIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiLzU4YTUzNDJmN2EvIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfh7Dwn4e3S1ItMTMyLjIyNi4xNzMuMTE4LTAzMzEiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxNTIuNzAuMjM1LjIwNyIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiNzBkOTUzMDgtMmE2MS00ZjkzLWYxMzktOTEwM2QwNTg3ZmQ5IiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDM1NDEyLAogICAgInBzIjogIvCfh7Dwn4e3S1ItMTUyLjcwLjIzNS4yMDctMDI3MSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxOC4xNDMuMTIzLjM1IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiZG0udG91dGlhby5jb20iLAogICAgImlkIjogIjY4ZGY0ODM4LTQ2ZDAtNGI1Yi1jM2YwLWE0MGVjNzA2MzI0NSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi8iLAogICAgInBvcnQiOiA4MCwKICAgICJwcyI6ICLwn4e48J+HrFNHLTE4LjE0My4xMjMuMzUtMTU3MzMiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:804#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0555
    vmess://ewogICAgImFkZCI6ICIxOC4xNDMuMTIzLjM1IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICI2OGRmNDgzOC00NmQwLTRiNWItYzNmMC1hNDBlYzcwNjMyNDUiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvIiwKICAgICJwb3J0IjogODAsCiAgICAicHMiOiAi8J+HuPCfh6xTRy0xOC4xNDMuMTIzLjM1LTAzMzciLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    trojan://bb5b1337-fa9e-4e00-b8c6-1110e626171d@159.223.89.239:443?allowInsecure=1#%F0%9F%87%B8%F0%9F%87%ACSG-159.223.89.239-0240
    vmess://ewogICAgImFkZCI6ICIxOC4xNDMuMTIzLjM1IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiMTguMTQzLjEyMy4zNSIsCiAgICAiaWQiOiAiNjhkZjQ4MzgtNDZkMC00YjViLWMzZjAtYTQwZWM3MDYzMjQ1IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiLyIsCiAgICAicG9ydCI6IDgwLAogICAgInBzIjogIvCfh7jwn4esU0ctMTguMTQzLjEyMy4zNS0xNTcyMCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    trojan://bb5b1337-fa9e-4e00-b8c6-1110e626171d@sg-01.tiktokcdn.top:443?allowInsecure=1#%F0%9F%87%B8%F0%9F%87%ACSG-159.223.89.239-0282
    vmess://ewogICAgImFkZCI6ICIxMzguMi40NC4yMTEiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjU5M2I4NTI1LTBjNDgtNGIwZi1kOWFmLTJkNzNhOTE0ODk3MyIsCiAgICAibmV0IjogInRjcCIsCiAgICAicGF0aCI6ICIiLAogICAgInBvcnQiOiAyMDA4MSwKICAgICJwcyI6ICLwn4ev8J+HtUpQLTEzOC4yLjQ0LjIxMS0wMjYzIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxNTIuNjkuMTk3LjYwIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJhYzhlMjZmZS04MTUwLTRiNjAtYWU2NC04MmZjNzdlYmEyY2YiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMTA2OSwKICAgICJwcyI6ICLwn4ev8J+HtUpQLTE1Mi42OS4xOTcuNjAtMTM5OSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxNjcuMTcyLjY0LjExIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICI3NmEyNzZhMi0wZmMzLTRiZmItY2IwMC02Y2QyYTQzMDk2NzciLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMTAwODYsCiAgICAicHMiOiAi8J+HuPCfh6xTRy0xNjcuMTcyLjY0LjExLTAyMzQiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxNTIuNjkuMTk3LjYwIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJhYzhlMjZmZS04MTUwLTRiNjAtYWU2NC04MmZjNzdlYmEyY2YiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMTA2OSwKICAgICJwcyI6ICLwn4ev8J+HtUpQLTE1Mi42OS4xOTcuNjAtMDMyMCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICJzZzIwMi5oa2FhMC50ayIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInNnMjAyLmhrYWEwLnRrIiwKICAgICJpZCI6ICJiZGY3OThmNC1hOTkwLTQ3NDMtZTliMi05Yzc4YmE1OGZiMDQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvaGthYTAiLAogICAgInBvcnQiOiAxMDE4LAogICAgInBzIjogIvCfh7jwn4esU0ctMTcyLjEwNC4xNjMuMjAyLTE3MDg3IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICJzZzIwMi5oa2FhMC50ayIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.219.218:809#%F0%9F%87%BA%F0%9F%87%B8US-37.120.219.218-15659
    ss://YWVzLTI1Ni1jZmI6dkRTOUcycA==@185.4.65.6:21247#%F0%9F%87%B7%F0%9F%87%BARU-185.4.65.6-15714
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.219.218:803#%F0%9F%87%BA%F0%9F%87%B8US-37.120.219.218-15657
    trojan://cb43b7c2-b744-41c5-bcc2-fd7467b332cf@jgwxn3.gaox.ml:443?allowInsecure=1#%F0%9F%87%A6%F0%9F%87%BAAU-140.238.205.173-14885
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:805#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0538
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.156:809#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.156-15778
    trojan://c19d1432-8b3e-4818-8837-3d160cf65908@138.2.45.243:443?allowInsecure=1#%F0%9F%87%AF%F0%9F%87%B5JP-138.2.45.243-19249
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.147.230:809#%F0%9F%87%BA%F0%9F%87%B8US-37.120.147.230-10334
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.219.218:804#%F0%9F%87%BA%F0%9F%87%B8US-37.120.219.218-15656
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.154:802#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.154-15689
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.91.107.225:805#%F0%9F%87%BA%F0%9F%87%B8US-38.91.107.225-15679
    vmess://ewogICAgImFkZCI6ICIxNzIuNjQuMTUzLjEwMiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNsYXNoMi50cnVtcDIwMjMudXMiLAogICAgImlkIjogImJlZDNkODc2LTJkMjYtNGQ0ZC1iNzg5LTMwNjM0MzhlZTc3NCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9kb25ndGFpd2FuZy5jb20iLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTE3Mi42NC4xNTMuMTAyLTEwNTQiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.91.107.225:809#%F0%9F%87%BA%F0%9F%87%B8US-38.91.107.225-15688
    vmess://ewogICAgImFkZCI6ICIxNi4xNjIuNTUuMTMwIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiMTYuMTYyLjU1LjEzMCIsCiAgICAiaWQiOiAiMTliOTVhMGUtZmZjZi0zMmVkLTg2NTYtNTJhZTEwMmE4YWQ4IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL255IiwKICAgICJwb3J0IjogNDQzMDAsCiAgICAicHMiOiAi8J+HrfCfh7BISy0xNi4xNjIuNTUuMTMwLTEyMzcxIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:812#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0545
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.156:811#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.156-15770
    vmess://ewogICAgImFkZCI6ICIxMzkuOTkuOTEuOTUiLAogICAgImFpZCI6IDMyLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJjMDE1NjQ1MS00ZWZiLTQ1ZTItODRmYy04ZDMxNWM0NjUwZGIiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfh7jwn4esU0ctMTM5Ljk5LjkxLjk1LTAyMzIiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.147.230:810#%F0%9F%87%BA%F0%9F%87%B8US-37.120.147.230-10335
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.91.107.225:812#%F0%9F%87%BA%F0%9F%87%B8US-38.91.107.225-15693
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.156:808#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.156-15691
    ss://YWVzLTI1Ni1jZmI6ZjYzZ2c4RXJ1RG5Vcm16NA==@213.183.59.214:9010#%F0%9F%87%B3%F0%9F%87%B1NL-213.183.59.214-17493
    vmess://ewogICAgImFkZCI6ICJzZy1vdmgxLnYyLXJheS5jb20iLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJzZy1vdmgxLnYyLXJheS5jb20iLAogICAgImlkIjogImE5NDgxNjAwLWVmMzYtNDAyYS1hMGU1LTU1NDdiZmQ3Yjg3YyIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9mYXN0c3NoL2ZnaGhoLzYzNDE5N2M0Y2RmODEvIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfh7jwn4esU0ctNTEuNzkuMTY0LjE0Ni0yNzc4IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    trojan://e05c749b-7c6b-41b8-9c71-9dcf685edf4a@152.67.162.166:443?allowInsecure=1&sni=content-provider22.cdn-delivery.akamaicd.com#%F0%9F%87%AE%F0%9F%87%B3IN-152.67.162.166-4645
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpxWUF0ODVTRkdWNTY=@185.77.217.217:443#%F0%9F%87%AB%F0%9F%87%AEFI-185.77.217.217-0797
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.114.114.139:811#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.139-10525
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.156:804#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.156-15768
    vmess://ewogICAgImFkZCI6ICJmdWxsYWNjZXNzdG9rb3JlYW5uZXRzdWJub2RlMS5henVyZXdlYnNpdGVzLm5ldCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImZ1bGxhY2Nlc3N0b2tvcmVhbm5ldHN1Ym5vZGUxLmF6dXJld2Vic2l0ZXMubmV0IiwKICAgICJpZCI6ICIyNzRmMTFjNi1mNjliLTQwYjktODk2Ni1mMzllMDZlOTdiZTciLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvd3MiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HsPCfh7dLUi01Mi4yMzEuMjAwLjE3OS01MDI5IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.114.114.139:809#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.139-10984
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.114.114.139:810#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.139-0772
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@172.245.218.162:804#%F0%9F%87%BA%F0%9F%87%B8US-172.245.218.162-15753
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.156:803#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.156-15777
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.47:800#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.47-15661
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@172.245.218.162:800#%F0%9F%87%BA%F0%9F%87%B8US-172.245.218.162-21268
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@172.245.218.162:805#%F0%9F%87%BA%F0%9F%87%B8US-172.245.218.162-15767
    vmess://ewogICAgImFkZCI6ICIxNjguMTM4LjIwNy42NiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiOTA1Zjk5YjEtZTdiYS00NWUwLWFlNGQtYjBmZmRmMGFkMjQ1IiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDIxMzY1LAogICAgInBzIjogIvCfh6/wn4e1SlAtMTY4LjEzOC4yMDcuNjYtMDI2NyIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTopMU4xRTZ2MFNVX3JHVHBn@79.133.109.56:1036#%F0%9F%87%BA%F0%9F%87%B8US-79.133.109.56-15762
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@172.245.218.162:809#%F0%9F%87%BA%F0%9F%87%B8US-172.245.218.162-15775
    vmess://ewogICAgImFkZCI6ICJ3d3cuZ292LmhrIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAidm4uY2xvdWRmbGFyZS5xdWVzdCIsCiAgICAiaWQiOiAiZGM4YjY0ZGItZWI2ZC00YmRmLTk4YjItMzE2MTUzMTliZWE4IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2FyaWVzIiwKICAgICJwb3J0IjogMjA4NiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjE2LjI0OS4xMzAtMTI5NSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxODUuMjI1LjY5LjEzNCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiM2MzYmZkNzUtZGMzMC00ZTc2LTg5NDAtNDdlMTEzN2UyMWY5IiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDQ1MDgxLAogICAgInBzIjogIvCfh63wn4e6SFUtMTg1LjIyNS42OS4xMzQtMDIyMyIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@172.245.218.162:810#%F0%9F%87%BA%F0%9F%87%B8US-172.245.218.162-15761
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@172.245.218.162:801#%F0%9F%87%BA%F0%9F%87%B8US-172.245.218.162-15719
    vmess://ewogICAgImFkZCI6ICJzZzExOC5oa2FhMC50ayIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInNnMTE4LmhrYWEwLnRrIiwKICAgICJpZCI6ICI2NTJmNDI2My1iZDg2LTRiZjYtOWY3ZS1kMjVlNzUxNmZiNzIiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvaGthYTAiLAogICAgInBvcnQiOiAxMzY5MSwKICAgICJwcyI6ICLwn4e48J+HrFNHLTE3Mi4xMDQuMTYzLjExOC0wMjQ4IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.147.230:804#%F0%9F%87%BA%F0%9F%87%B8US-37.120.147.230-10332
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.91.107.225:800#%F0%9F%87%BA%F0%9F%87%B8US-38.91.107.225-15681
    vmess://ewogICAgImFkZCI6ICJ2c2cxLjBiYWQuY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiJTdCJTIySG9zdCUyMjolMjJ2c2cxLjBiYWQuY29tJTIyJTdEIiwKICAgICJpZCI6ICI5MjcwOTRkMy1kNjc4LTQ3NjMtODU5MS1lMjQwZDBiY2FlODciLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvY2hhdCIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4e48J+HrFNHLTE3MC4xODcuMTk2LjEyOC0xNTk4MSIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICI4OS4yMDguMTA1LjYzIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICIyRjA5NDg0NS1FMkJELUVCRjctREVCNy05OTU5OTI0MzZGQUYiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMjM0NTMsCiAgICAicHMiOiAi8J+Hs/Cfh7FOTC04OS4yMDguMTA1LjYzLTAzMDYiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.91.107.225:802#%F0%9F%87%BA%F0%9F%87%B8US-38.91.107.225-15692
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:812#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-0765
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:807#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-20430
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.219.218:812#%F0%9F%87%BA%F0%9F%87%B8US-37.120.219.218-15660
    trojan://3f087c04-44e6-4c96-a917-ca974de1212b@kr1.api-aws.com:443?allowInsecure=1#%F0%9F%87%B0%F0%9F%87%B7KR-146.56.176.239-15564
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.147.230:803#%F0%9F%87%BA%F0%9F%87%B8US-37.120.147.230-10337
    vmess://ewogICAgImFkZCI6ICIxNzIuNjQuMTUzLjEwMiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNsYXNoMi50cnVtcDIwMjMudXMiLAogICAgImlkIjogImJlZDNkODc2LTJkMjYtNGQ0ZC1iNzg5LTMwNjM0MzhlZTc3NCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9kb25ndGFpd2FuZy5jb20iLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTE3Mi42NC4xNTMuMTAyLTAyNTIiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:805#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-20428
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:801#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-2879
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:810#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-20415
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:808#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-20437
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:802#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-20423
    vmess://ewogICAgImFkZCI6ICJ1bnVzMDEuYWpka2phbGpkai54eXoiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJ1bnVzMDEuYWpka2phbGpkai54eXoiLAogICAgImlkIjogIjk1ZTlmZGExLWRjNDgtM2JiZC04YTE1LWU2NTI4ODgyZWEzYiIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi82IiwKICAgICJwb3J0IjogMTA4MiwKICAgICJwcyI6ICLwn4e68J+HuFVTLTM4LjU0Ljk1LjE3OC01MjQxIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:800#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-20418
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:800#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-4617
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.159.30.61:808#%F0%9F%87%AB%F0%9F%87%B7FR-51.159.30.61-0082
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@193.176.86.190:806#%F0%9F%87%A9%F0%9F%87%AADE-193.176.86.190-0969
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:801#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-0967
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:806#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-0763
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.219.218:801#%F0%9F%87%BA%F0%9F%87%B8US-37.120.219.218-15655
    vmess://ewogICAgImFkZCI6ICIyMTMuMjI2LjcxLjEyNyIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiMkYwOTQ4NDUtRTJCRC1FQkY3LURFQjctOTk1OTkyNDM2RkFGIiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDIzNDUzLAogICAgInBzIjogIvCfh6nwn4eqREUtMjEzLjIyNi43MS4xMjctNzkyNCIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:807#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-7529
    vmess://ewogICAgImFkZCI6ICJzZy5wcnByLmxpbmsiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJzZy5wcnByLmxpbmsiLAogICAgImlkIjogImNlYTQyMTYxLWJkZGMtNDIzMC1hOWI5LWU0MzE4Nzk2N2ZmYSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9UZWxlZ3JhbS9TaGFyZUNlbnRyZVByby9ta25uaXgiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTEwNC4yMS4zNS4yMTEtMTI1OCIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:809#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-7524
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:810#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-2099
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:804#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-7527
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:808#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-7521
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.159.30.61:809#%F0%9F%87%AB%F0%9F%87%B7FR-51.159.30.61-1423
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:802#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-7526
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpVbHRyQHIwMHRfMjAxNw==@138.68.248.130:811#%F0%9F%87%BA%F0%9F%87%B8US-138.68.248.130-0556

</details>

- you can import these 200 tested nodes using their subscription link into different clients. refer to `Instructions & Usage` section

### all nodes
merge nodes w/o dup: `6347`
- [Node link Mixed (V2ray)](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/sub/sub_merge.txt)
- [Node link Yaml (Clash)](https://raw.githubusercontent.com/mahdibland/SSAggregator/master/sub/sub_merge_yaml.yml)

#### all nodes separated by protoctol
- [VMESS](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/sub/splitted/vmess.txt)
- [TROJAN](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/sub/splitted/trojan.txt)
- [SSR](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/sub/splitted/ssr.txt)
- [SHADOWSOCKS](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/sub/splitted/ss.txt)

#### provider config for clash 🐈‍⬛
> Configs with the "others" tag will proxy domestic services.

- [Clash Meta For Iran](https://cdn.jsdelivr.net/gh/mahdibland/V2RayAggregator@master/update/provider/provider-meta.yml) (Recommended)
- [Clash Meta For China](https://cdn.jsdelivr.net/gh/mahdibland/V2RayAggregator@master/update/provider/provider-meta-cn.yml) (Recommended)
- [Clash Meta For Others](https://cdn.jsdelivr.net/gh/mahdibland/V2RayAggregator@master/update/provider/provider-meta-others.yml) (Recommended)

- [Clash For Iran](https://cdn.jsdelivr.net/gh/mahdibland/V2RayAggregator@master/update/provider/provider.yml)
- [Clash For China](https://cdn.jsdelivr.net/gh/mahdibland/V2RayAggregator@master/update/provider/provider-cn.yml)
- [Clash For Others](https://cdn.jsdelivr.net/gh/mahdibland/V2RayAggregator@master/update/provider/provider-others.yml)


### node sources
- [pojiezhiyuanjun/freev2](https://github.com/pojiezhiyuanjun/freev2), number of nodes: `131`
- [Nodefree.org](https://github.com/Fukki-Z/nodefree), number of nodes: `28`
- [FiFier/v2rayShare](https://github.com/FiFier/v2rayShare), number of nodes: `18`
- [AlienVPN402](https://github.com/AlienVPN402), number of nodes: `659`
- [huwo1/proxy_nodes](https://bitbucket.org/huwo1/proxy_nodes/raw/b90856fe7cb9c666223f3ad41c87d0e60c711590/proxy.md), number of nodes: `21`
- [hamidimorteza680](https://freevpn878.hamidimorteza680.workers.dev/sub), number of nodes: `186`
- [irancpi](https://t.me/irancpi_vpn), number of nodes: `181`
- [muma16fx](https://muma16fx.netlify.app), number of nodes: `20`
- [AzadNet](https://t.me/AzadNet), number of nodes: `845`
- [Huibqr](https://github.com/Huibq), number of nodes: `35`
- [Kwinshadow](https://github.com/Kwinshadow), number of nodes: `8`
- [Leon406](https://github.com/Leon406), number of nodes: `1503`
- [Lewis-1217](https://github.com/Lewis-1217), number of nodes: `39`
- [Mohammadgb0078](https://github.com/Mohammadgb0078), number of nodes: `30`
- [Mr8AHAL](https://github.com/Mr8AHAL), number of nodes: `26`
- [surfboardv2ray](https://t.me/surfboardv2ray), number of nodes: `483`
- [ZywChannel](https://github.com/ZywChannel), number of nodes: `166`
- [aiboboxx/v2rayfree](https://github.com/aiboboxx), number of nodes: `135`
- [dingyu0321/linshi](https://github.com/dingyu0321), number of nodes: `115`
- [ermaozi/get_subscribe](https://github.com/ermaozi), number of nodes: `20`
- [ermaozi01/free_clash_vpn](https://github.com/ermaozi01), number of nodes: `18`
- [fanqiangfeee/freefq](https://github.com/fanqiangfeee), number of nodes: `55`
- [xiyaowong/freeFQ](https://github.com/xiyaowong), number of nodes: `156`
- [free18/v2ray](https://github.com/free18), number of nodes: `28`
- [hkaa0/permalink](https://github.com/hkaa0), number of nodes: `10`
- [jsnjsnwbtwbt/2D2F](https://github.com/jsnjsnwbtwbt), number of nodes: `9`
- [junwei380](https://github.com/junwei380), number of nodes: `15`
- [mahsanet/MahsaFreeConfig](https://github.com/mahsanet), number of nodes: `3`
- [mlabalabala/v2ray-node](https://github.com/mlabalabala), number of nodes: `58`
- [peasoft/NoMoreWalls](https://github.com/peasoft), number of nodes: `134`
- [resasanian/Mirza](https://github.com/resasanian), number of nodes: `71`
- [ripaojiedian/freenode](https://github.com/ripaojiedian), number of nodes: `26`
- [sun9426/v2ray](https://github.com/sun9426), number of nodes: `6`
- [ts-sf/fly](https://github.com/ts-sf), number of nodes: `201`
- [voken100g/AutoSSR](https://github.com/voken100g), number of nodes: `19`
- [w1770946466/Auto_proxy](https://github.com/w1770946466), number of nodes: `421`
- [sub.pmsub.me/base64](https://sub.pmsub.me/base64), number of nodes: `2`
- [yebekhe/TVC](https://github.com/yebekhe), number of nodes: `244`
- [yebekhe/TelegramV2rayCollector](https://github.com/yebekhe), number of nodes: `66`
- [sarinaesmailzadeh/V2Hub](https://github.com/sarinaesmailzadeh), number of nodes: `39`
- [soroushmirzaei/telegram-configs-collector](https://github.com/soroushmirzaei), number of nodes: `5889`
- [coldwater-10/V2Hub3](https://github.com/coldwater-10/V2Hub3), number of nodes: `268`
- [coldwater-10/V2Hub4](https://github.com/coldwater-10/V2Hub4), number of nodes: `255`
- [coldwater-10/V2Hub5](https://github.com/coldwater-10/V2Hub5), number of nodes: `332`
- [vpnhat](https://t.me/vpnhat), number of nodes: `11`
- [wangcai](https://t.me/wangcai_8), number of nodes: `5`

## Softwares

### Best Clients For Each OS

|    OS   |              Best Client               | Alternatives |
|:-------:|:--------------------------------------:|:------------:|
|   IOS   |        Quantumult - Shadowrocket       |  NapsternetV |
| Android |Surfboard - Clash For Android - Matsuri |    V2rayNg   |
| Windows |   Clash For Windows - V2rayN - Nekoray |    Qv2ray    |
|  Linux  |           Clash For Windows            |    Qv2ray    |
|  MacOS  |           Clash For Windows            |    Qv2ray    |

### Desktop Clients

|                              MacOS                               |                              Linux                               |                                       Windows                                       | Brief description                                                                                         |
| :--------------------------------------------------------------: | :--------------------------------------------------------------: | :---------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------- |
| [CFW](https://github.com/Fndroid/clash_for_windows_pkg/releases) | [CFW](https://github.com/Fndroid/clash_for_windows_pkg/releases) | [CFW(Clash For Windows)](https://github.com/Fndroid/clash_for_windows_pkg/releases) | SS, SSR, Trojan, Vmess, VLESS protocol support, strong policy offload capability.                                         |
|       [Qv2ray](https://github.com/Qv2ray/Qv2ray/releases)        |       [Qv2ray](https://github.com/Qv2ray/Qv2ray/releases)        |                 [Qv2ray](https://github.com/Qv2ray/Qv2ray/releases)                 | SS, SSR, Trojan, Vmess, VLESS, Trojan-Go protocol support (relevant plugins need to be installed).                            |
|                                ×                                 |                                ×                                 |                 [V2rayN](https://github.com/2dust/v2rayN/releases)                  | SS, Trojan, Vmess, VLESS protocol support, with speed measurement, delay measurement function, support subscription, QR code, clipboard import and manual configuration.  |
|                                ×                                 |                                ×                                 |               [WinXray](https://github.com/TheMRLL/winxray/releases)                | SS, SSR, Trojan, Vmess, VLESS protocol support, support automatic connection to the fastest node.                                   |
|                                ×                                 |                                ×                                 | [Shadowsocks-windows](https://github.com/shadowsocks/shadowsocks-windows/releases)  | SS protocol support, SS dedicated client.                                                                    |
|                                ×                                 |                                ×                                 |  [ShadowsocksR-windows](https://github.com/HMBSbige/ShadowsocksR-Windows/releases)  | SSR protocol support, SSR dedicated client.                                                                   |
|                  [Surge](https://nssurge.com/)                   |                                ×                                 |                                          ×                                          | SS, Trojan, Vmess protocol support, well-known network debugging tools, powerful strategy offloading ability, need to pay.                         |
|     [ClashX](https://github.com/yichengchen/clashX/releases)     |                                ×                                 |                                          ×                                          | SS, SSR, Trojan, Vmess protocol support, occupy less resources.                                                  |
|        [V2rayU](https://github.com/yanue/V2rayU/releases)        |                                ×                                 |                                          ×                                          | SS, Trojan, Vmess protocol support, support subscription, QR code, clipboard import, manual configuration, QR code sharing, similar to V2RayN. |
|       [V2rayA](https://github.com/v2rayA/v2rayA/releases/)       |       [V2rayA](https://github.com/v2rayA/v2rayA/releases/)       |                [V2rayA](https://github.com/v2rayA/v2rayA/releases/)                 | V2Ray, Xray, SS, SSR, Trojan support, subscription and manual config.  |

### Mobile Clients

|                               iOS/iPadOS                                |                                      Android                                       | Brief description                                                                                                                                                  |
| :---------------------------------------------------------------------: | :--------------------------------------------------------------------------------: | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Shadowrocket](https://apps.apple.com/us/app/shadowrocket/id932747118)  |  [Shadowrocket](https://play.google.com/store/apps/details?id=com.v2cross.proxy)   | SS, SSR, Trojan, Vmess, VLESS protocol support, the iOS side needs to be purchased in the non-country App Store, the US price is $2.99; the Android side is not the same author as the iOS side, does not support the SSR protocol, free and built-in free nodes. |
|                      [Surge](https://nssurge.com/)                      |                                         ×                                          | SS, Trojan, Vmess protocol support, well-known network debugging tools on the iOS side, chargeable.                                                                                              |
| [Quantumult X](https://apps.apple.com/us/app/quantumult-x/id1443988620) |                                         ×                                          |                                                                                 |
| [Potatso Lite](https://apps.apple.com/us/app/potatso-lite/id1239860606) |                                         ×                                          | SS, SSR protocol support, need to be purchased in the non-country AppStore, free.                                                                                                        |
|                                    ×                                    |    [Surfboard](https://play.google.com/store/apps/details?id=com.getsurfboard)     | SS, SSR, Vmess Protocol support, Android network debugging software, compatible with Surge 2 configuration.                                                                                          |
|                                    ×                                    |    [CFA(Clash For Android)](https://github.com/Kr328/ClashForAndroid/releases)     | SS, SSR, Trojan, Vmess Protocol support.                                                                                                                         |
|                                    ×                                    |             [SagerNet](https://github.com/SagerNet/SagerNet/releases)              | SS, SSR, Trojan, Vmess, VLESS Protocol support.                                                                                                                  |
|                                    ×                                    | [Shadowsocks-android](https://github.com/shadowsocks/shadowsocks-android/releases) | SS protocol support, Android-specific SS client.                                                                                                                         |
|                                    ×                                    | [ShadowsocksR-android](https://github.com/HMBSbige/ShadowsocksR-Android/releases)  | SSR protocol support, Android-specific SSR client.                                                                                                                       |
|                                    ×                                    |                [V2rayNG](https://github.com/2dust/v2rayNG/releases)                | SS, Trojan, Vmess, VLESS protocol support, v2ray kernel.                                                                                                           |

### Credit: 
- [alanbobs999](https://github.com/alanbobs999)
- [PersianBlocker](https://github.com/MasterKia/PersianBlocker)
- [iran-hosted-domains](https://github.com/bootmortis/iran-hosted-domains)
