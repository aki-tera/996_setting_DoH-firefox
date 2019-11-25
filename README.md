# 996_setting_DoH-firefox


How to use DoH(DNS over HTTPS) by Firefox.  

***

## setting
1. [address bar]about:config
0. [resarch:]network.trr
0. [network.trr.bootstrapAddress:string]"" -> "8.8.8.8"
0. [network.trr.excluded-domains]"localhost,local" -> "8.8.8.8"  ***Warning: If you do this, you will not be able to access the private network.***
0. [network.trr.mode]"0(Invalid)" ->  "3(Use only DNS Over HTTPS)"  
   *"1(Prioritize DNS and use DNS Over HTTPS)" or "2(Prioritize DNS Over HTTPS and use DNS)"*
0. [network.trr.uri]"" -> "https://dns.google/dns-query"
0. [address bar]about:networking#dns ---If TRR is True, DoH is enabled
