<div align="center">

# 나만의 아두이노 날씨 표시장치 만들기

## 개요

[![upir video](https://img.youtube.com/vi/xI6dXTA02UQ/0.jpg)](https://youtu.be/xI6dXTA02UQ?si=fvz78xu_96NryqND)

영상을 누르면 재생됩니다.

</div>

[Upir](https://www.youtube.com/@upir_upir)에서 만든 아두이노로 게이지를 만드는 튜토리얼은 나를 매료시키기 충분했다. 마침 방학이라 무엇이라도 하고 싶었던 나는 이 게이지를 활용해 나만의 시계 + 온습도계를 제작해보고자 했다. 

<div align="center">

## 필요한 재료

| 재료명 | 구매 링크 |
| --- | --- |
| WeMos D1 Mini v4.0.0, ESP8266, 4MB | [알리익스프레스1](https://ko.aliexpress.com/item/1005004544650251.html?spm=a2g0o.order_list.order_list_main.65.21ef140fxGS2uW&gatewayAdapt=glo2kor) / [알리익스프레스2](https://ko.aliexpress.com/item/1005005584902097.html?spm=a2g0o.productlist.main.3.70aa15e8h8a4nT&algo_pvid=089011f1-da66-4518-866c-d5920875552e&algo_exp_id=089011f1-da66-4518-866c-d5920875552e-1&pdp_npi=4%40dis%21KRW%213605%212130.0%21%21%212.64%21%21%40210321ea16928843661383219e4b11%2112000033646550763%21sea%21KR%21864354990%21&curPageLogUid=FHxuQpNmLnBb) / [쿠팡](https://www.coupang.com/vp/products/1910662584?itemId=3244018335&vendorItemId=71231195068&q=WeMos+D1&itemsCount=36&searchId=91aeca789abb46679920c07d43422790&rank=1&isAddedCart=) |
| DHT22 | [알리익스프레스1](https://ko.aliexpress.com/item/1005005203616199.html?spm=a2g0o.productlist.main.21.381d3a4cMHFMRx&algo_pvid=c73eea22-e571-4c99-8b0c-2a8655175be5&algo_exp_id=c73eea22-e571-4c99-8b0c-2a8655175be5-10&pdp_npi=4%40dis%21KRW%212567%211407.0%21%21%211.88%21%21%40210321ea16928844214784191e4b11%2112000032140438048%21sea%21KR%21864354990%21&curPageLogUid=kOoKVvWlkk0n) / [알리익스프레스2](https://ko.aliexpress.com/item/1005005616752351.html?spm=a2g0o.productlist.main.7.976d3a4c09933E&algo_pvid=54f5abd0-6ba6-49ec-8731-34189c60e1da&algo_exp_id=54f5abd0-6ba6-49ec-8731-34189c60e1da-3&pdp_npi=4%40dis%21KRW%211898%211803.0%21%21%211.39%21%21%40210321ea16928844660814633e4b11%2112000033761388071%21sea%21KR%21864354990%21&curPageLogUid=8Jd3rNxGB83Z) / [메카솔루션](https://mechasolution.com/shop/goods/goods_view.php?goodsno=540038&category=129003) |
| 1.5인치 128*128 STM32 OLED | [알리익스프레스](https://ko.aliexpress.com/item/4000080365758.html?spm=a2g0o.order_list.order_list_main.76.21ef140fxGS2uW&gatewayAdapt=glo2kor) |
| 500mAh 배터리 | [메카솔루션](https://mechasolution.com/shop/goods/goods_view.php?&goodsno=583877) |
| DS1307 RTC 모듈 | [메카솔루션](https://mechasolution.com/shop/goods/goods_view.php?&goodsno=590) |

</div>

기타 제작하는 데 필요한 스위치, 전선 등은 오프라인에서 구매하였다.
