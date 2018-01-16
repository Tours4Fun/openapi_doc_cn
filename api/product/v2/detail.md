# 产品详情

### 描述

根据产品ID批量获取产品详情信息。数据结构根据你产品所属产品线，结构有所不同，在做业务处理时，请遵守产品线数据类型处理。


### API地址

    /v2/product/detail

### 参数

| 参数           | 类型          | 是否必须 | 描述             |
| -------------- |:-------------:| ----:| :-----------------|
| product_ids    | array  |  是   | 产品ID号  |

注意：批量获取每次最多可以传入10个产品ID

### 参数示例

    {
        "product_ids":[101686926,101457615]
    }

### 返回示例

    多日游(product_lint为tour):
    {
        "code": 0,
        "msg": "success",
        "data": {
            "base": {
                "product_id": 101457621,
                //产品老id
                "product_id_old": "6678",
                //产品线
                "product_line": "tour",
                //产品名称
                "name": "十一日畅游墨西哥,旧金山,大峡谷,迪斯尼,环球影城之旅",
                //产品主图
                "image_url": "sg3da.jpg",
                //建议价格
                "advertised_price": 755,
                //价格货币类型
                "currency": "USD",
                //行程时间
                "duration": 11,
                //行程时间单位 day,hour,minute
                "duration_type": "day",
                //库存状态
                "stock_status": 1,
                //最大小孩年龄
                "max_child_age": 11,
                //提前预定天数
                "min_days_before_departure": 0,
                //最小出团人数
                "min_guest_number": 1,
                //是否显示自费项目
                "show_ownexpense": 0,
                "visa_passport": 0,
                //是否提供出发接送服务
                "is_pickup": 2,
                //是否提供到达接送服务
                "is_dropoff": 2,
                "hotel_pickup": 0,
                //出发城市(可以多个)
                "departure_city": [
                    {
                        "departure_city_id": 1,
                        "departure_city_name": "洛杉矶"
                    }
                ],
                //回团城市(可以多个)
                "return_city": [
                    {
                        "return_city_id": 1,
                        "return_city_name": "洛杉矶"
                    }
                ],
                //产品区域中文名
                "region_chinese_name": "美国",
                //产品子区域中文名
                "sub_region_chinese_name": "美西",
                "region": "us",
                "sub_region": "west"
            },
            "info": {
                //简要描述、推荐
                "brief_description": "您将超值游览到迪士尼乐园、加州著名的丹麦城、拥有价值连城的古董和艺术品的赫氏古堡、文化名城旧金山。而风景秀丽的优胜美地国家公园会让您恍若置身世外桃园。除此之外，享有“世界娱乐之都”美誉的拉斯维加斯、鬼斧神工的科罗拉多大峡谷和拥有工业世界七大奇观之一美誉的胡佛大坝更是您不容错过的特色景点。著名的好莱坞环球影城主题公园将会为您的旅程增光添彩。还有迷人的墨西哥恩森那达绽放光彩。",
                //详细描述
                "full_description": "<STYLE type=text/css>\r\n<!--\r\n.STYLE1 {color: #F7860F}\r\n-->\r\n</STYLE>\r\n\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第一天 </SPAN>原居地(Home)-洛杉矶(Los Angeles)<BR></H5></DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/los-angeles-skyline-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1>\r\n  <p class=\"main\">当您降落於洛杉矶机场的时候,我们热情的导游将在<span class=\"STYLE1\">行李认领处</span>等候您的到来。之后，导游会把您带往下榻的酒店，您可以自行安排余下的时间。（希望可以在当地时间下午3：00pm以后到达，办理酒店登记手续。）</p></DIV>\r\n<DIV class=p_p>\r\n<TABLE>\r\n<TBODY>\r\n<TR>\r\n<TD><img src=\"http://images.tours4fun.com/image/f.gif\" /></TD>\r\n<TD>+ </TD>\r\n<TD><IMG src=\"http://images.tours4fun.com/image/upgrad_hotel.gif\"></TD>\r\n<TD><B><SPAN class=hotel_title>酒店</SPAN>: Anaheim Park Hotel 或 Holidays Inn Hotel La Mirada 或者同等级的酒店</B></TD>\r\n</TR></TBODY></TABLE></DIV></DIV>\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第二天 </SPAN>洛杉矶(Los Angeles)-罗莎丽多(Rosarito)-恩塞那达(Ensenada)<BR>\r\n</H5>\r\n</DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/ensenada-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1>\r\n  <p class=\"main\">早上我们从洛杉矶出发，迎著和煦的阳光，沿著加州公路南下，穿越美墨边城蒂娃娜，进入了一号海滨公路。碧蓝的海水，洁白的沙滩，马上映入您的眼帘。中午时分来到著名的罗莎丽多海滨渡假城，您可坐在露天餐厅享受著阳光，或自费骑马奔驰在沙滩上。傍晚进入渔港之都－恩森那达。抵达酒店后，自由活动,您可以漫步於城中，购买精美价廉的墨西哥手工艺品：皮包，皮衣，然后饱尝新鲜海鱼，龙虾等海鲜大餐，迷人的拉丁音乐风情，伴您进入梦乡。</p></DIV>\r\n<DIV class=p_p>\r\n<TABLE>\r\n<TBODY>\r\n<TR>\r\n<TD><img src=\"http://images.tours4fun.com/image/f.gif\" /></TD>\r\n<TD><B><SPAN class=hotel_title>酒店:</SPAN><SPAN class=mainblue>Santo Tomasl 或 San Nicolas Resort  或者同等级酒店</SPAN></B></TD>\r\n</TR></TBODY></TABLE></DIV></DIV>\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第三天 </SPAN>恩塞那达(Ensenada)-拉普发多拉天然海水喷泉(La Bufadora)-科罗娜多岛(Coronado Island)<BR></H5>\r\n</DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/colorado-island-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1>\r\n  <p class=\"main\">上午前往拉普发多拉天然海水喷泉，沿著海岸可看见光怪陆离的岩穴，海水拍岸，浪花四溅，堪称海上奇景。午后沿著黄金海岸北上，回到美国西岸最大的军港城市圣地牙哥。穿越跨海大桥，来到哥罗娜多岛，美丽的海滩，绿草如茵的高尔夫球场，同时参观加州最古老的哥罗娜多酒店。此酒店已有百年历史，爱迪生曾亲自监督该旅馆照明设备之安装，英国皇室之温莎公爵也曾下榻於此。此外，曾有十二位美国总统莅临开会及渡假。经由跨海大桥，俯瞰军港及海湾美景并转赴古城游览。古城为加州之发源地，其高耸入云的旗杆，曾升上南加第一面国旗，思古幽情中，充满了南美拉丁色彩之艺术品及文物，然后踏著夕阳，带著美好的回忆，大约在傍晚7：00回到洛杉矶。</p></DIV>\r\n<DIV class=p_p>\r\n<TABLE>\r\n<TBODY>\r\n<TR>\r\n<TD><img src=\"http://images.tours4fun.com/image/f.gif\" /></TD>\r\n<TD>+ </TD>\r\n<TD><IMG src=\"http://images.tours4fun.com/image/upgrad_hotel.gif\"></TD>\r\n<TD><B><SPAN class=hotel_title>酒店：Anaheim Park Hotel 或 Holidays Inn Hotel La Mirada 或者同等级的酒店</SPAN> </B></TD></TR></TBODY></TABLE></DIV></DIV>\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第四天 </SPAN>迪斯尼乐园或者加州冒险乐园(Disney or Adventure Park)<BR></H5></DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/los-angeles-disneyland-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1>\r\n  <p class=\"main\">清晨大约7时左右，由洛杉矶出发沿5号州际高速公路向南到达橙县，去到座落在加州的全世界闻名迪斯尼乐园。在专业的导游一天的时间当中为您特别挑选出一些最为值得参加的游乐项目，让您感觉到目不转睛，惊险无比。傍晚之后，再由导游送回到酒店休息。</p></DIV>\r\n<DIV class=p_p>\r\n<TABLE>\r\n<TBODY>\r\n<TR>\r\n<TD><img src=\"http://images.tours4fun.com/image/f.gif\" /></TD>\r\n<TD>+ </TD>\r\n<TD><IMG src=\"http://images.tours4fun.com/image/upgrad_hotel.gif\"></TD>\r\n<TD><B><SPAN class=hotel_title>酒店：Anaheim Park Hotel 或 Holidays Inn Hotel La Mirada 或者同等级的酒店</SPAN> </B></TD></TR></TBODY></TABLE></DIV></DIV>\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第五天 </SPAN>好莱坞环球影城主题公园(Universal Studios)<BR></H5></DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/hollywood-universal-studio-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1><SPAN class=main>早上出发后，到达著名的好莱坞星光大道，参观著名的中国大剧院，柯达剧院，明星手印，之后进入环电影制片主题公园。这次旅程将带您游历城里的恐怖片的拍摄场景。在这里您可以充分的体验场面宏大的表演和动物秀，以及幽默滑稽的儿童节目。</span></DIV>\r\n<DIV class=p_p>\r\n<TABLE>\r\n<TBODY>\r\n<TR>\r\n<TD><img src=\"http://images.tours4fun.com/image/f.gif\" /></TD>\r\n<TD>+ </TD>\r\n<TD><IMG src=\"http://images.tours4fun.com/image/upgrad_hotel.gif\"></TD>\r\n<TD><STRONG><SPAN class=hotel_title>酒店</SPAN>: </STRONG><B>Anaheim Park Hotel 或 Holidays Inn Hotel La Mirada 或者同等级的酒店</B></TD>\r\n</TR></TBODY></TABLE></DIV></DIV>\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第六天 </SPAN><SPAN class=heading_text>洛杉矶(Los Angeles)-巴斯多(Basedow)-拉斯维加斯(Las Vegas) （约266英里）\r\n</SPAN><BR></H5>\r\n</DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/barstow-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1>\r\n  <p class=\"main\">清晨我们将从洛杉矶出发，开始精彩的三天之旅。驱车途经圣贝纳迪诺山和莫哈韦大沙漠。中午时分，团体特别为我们会在巴斯多－从洛杉矶到拉斯维加斯途中的一个工厂直销商场做一个短暂的购物休息，并且在这里享用午餐。之后前往拉斯维加斯，晚上您可以自由活动。</p></DIV>\r\n<DIV class=p_p>\r\n<TABLE>\r\n<TBODY>\r\n<TR>\r\n<TD><img src=\"http://images.tours4fun.com/image/f.gif\" /></TD>\r\n<TD><B><SPAN class=hotel_title>酒店</SPAN>: Stratosphere Hotel 或 <SPAN class=mainblue>Plaza Casino Hotel, Las Vegas  或者同等级酒店</SPAN></B></TD>\r\n</TR></TBODY></TABLE></DIV></DIV>\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第七天 </SPAN>拉斯维加斯(Las Vegas)-大峡谷国家公园(Grand Canyon)-胡佛水坝(Hoover Dam)-拉斯维加斯(Las Vegas) （约520英里） \r\n<BR></H5>\r\n</DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/grand_canyon-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1>\r\n  <p class=\"main\">清晨前往拥有世界七大奇景美誉的科罗拉多大峡谷国家公园。这是世界上最为鲜活的侵蚀范本，也使游客无不面对这造物主的鬼斧神工而感慨万千。之后前往参观美国历史上最为著名的水利工程之一-位于科罗拉多河上的胡佛水霸,并且可以遥望西海岸最大的米德人工湖。下午，再此满怀期待的回到这个世界娱乐之都-罪恶之城,拉斯维加斯。 您可在下榻的酒店一试手气，或者安排各种酒店表演。</p></DIV>\r\n<DIV class=p_p>\r\n<TABLE>\r\n<TBODY>\r\n<TR>\r\n<TD><img src=\"http://images.tours4fun.com/image/f.gif\" /></TD>\r\n<TD><B><SPAN class=hotel_title>酒店:</SPAN> Stratosphere Hotel 或 Plaza Casino Hotel, Las Vegas <SPAN class=mainblue>或者同等级酒店</SPAN></B></TD>\r\n</TR></TBODY></TABLE></DIV></DIV>\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第八天 </SPAN><SPAN class=heading_text>拉斯维加斯(Las Vegas)-巧克力工厂(Hershey Chocolate Factory)-工厂直销商场(Outlet Factory)-洛杉矶(Los Angeles) （约270英里）\r\n</SPAN><BR></H5>\r\n</DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/las-vegas-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1>\r\n  <p class=\"main\">清晨我们将前往参观巧克力工厂，让您亲眼目睹巧克力的生产过程。您还可以购买各种精致的巧克力。大约中午11:00左右，我们会向洛杉矶进发。中途会再次路径巴斯多用午餐和做简单购物。大约下午6：00会回到洛杉矶。</p></DIV>\r\n<DIV class=p_p>\r\n<TABLE>\r\n<TBODY>\r\n<TR>\r\n<TD><img src=\"http://images.tours4fun.com/image/f.gif\" /></TD>\r\n<TD>+ </TD>\r\n<TD><IMG src=\"http://images.tours4fun.com/image/upgrad_hotel.gif\"></TD>\r\n<TD><B><SPAN class=hotel_title>酒店:</SPAN> Anaheim Park Hotel 或 Holidays Inn Hotel La Mirada 或者同等级的酒店</B></TD>\r\n</TR></TBODY></TABLE></DIV></DIV>\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第九天 </SPAN><SPAN class=heading_text>洛杉矶(Los Angelea)-<strong>丹麦城(Solvang)</strong>-赫氏古堡(Hearst Castle)-</SPAN>旧金山(San Francisco) （约380英里）<BR></span></H5>\r\n</DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/solvang-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1>\r\n  <p class=\"main\">早上离开LA最大的华人社区--蒙特利公园城市，沿途欣赏太平洋海岸线公路的美景，抵达加州著名的丹麦城--享受加州阳光和丹麦咖啡的温情与浪漫. 接著继续北行游览赫斯特城堡，在<span class=\"heading_text\">赫氏古堡</span>里，你可以观赏价值连城的古董和艺术品，甚至是装饰华丽，镀金的小泳池，宏伟的主礼堂威严耸立，令人瞩目。晚上留宿旧金山。</p></DIV>\r\n<DIV class=p_p>\r\n<TABLE>\r\n<TBODY>\r\n<TR>\r\n<TD><img src=\"http://images.tours4fun.com/image/f.gif\" /></TD>\r\n<TD><B><SPAN class=hotel_title>酒店:</SPAN><SPAN class=mainblue> Courtyard Marriott Silicon Valley, Fremont 或Comfort Inn Cockatoo或者同等级酒店</span></B></TD>\r\n</TR></TBODY></TABLE></DIV></DIV>\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第十天 </SPAN>旧金山(San Francisco)<strong>市区游览</strong><BR></H5>\r\n</DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/san-francisco-skyline-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1>\r\n  <p class=\"main\">清晨大约40分钟驱车前往加州历史、文化名城--旧金山。「雾锁金门」是这的特有景观。华裔移民聚居在中国城，意大利后裔在北滩创建「小意大利区」，当今渔人码头已成观光胜地。你还可以选择自费乘船游览海湾。富豪岗立即展现了淘金热与铁路供给的金碧辉煌；俄罗斯山的陡峭，反而成就了伦巴街独特的九曲十八弯。艺术宫的古罗马建筑，使人们对巴拿马博览会的盛况浮想联翩。傍晚9时回到位于莫德斯托的酒店。</p></DIV>\r\n<DIV class=p_p>\r\n<TABLE>\r\n<TBODY>\r\n<TR>\r\n<TD><img src=\"http://images.tours4fun.com/image/f.gif\" /></TD>\r\n<TD><B><SPAN class=hotel_title>酒店:</SPAN><SPAN class=mainblue> Courtyard Marriott Silicon Valley, Fremont 或Comfort Inn Cockatoo或者同等级酒店</B></TD>\r\n</TR></TBODY></TABLE></DIV></DIV>\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第十一天 </SPAN>莫德斯托(Modesto)<SPAN class=heading_text>-优胜美地国家公园(Yosemite)</SPAN>-洛杉矶 （约312英里） \r\n(Los Angeles)<BR></H5>\r\n</DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/yosemite-national-park-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1>\r\n  <p class=\"main\">清晨继续前行游览加州最出名的国家公园之一--优胜美地国家公园（Yosemite National Park），它坐落于内华达州山脉的中，是一处自然奇观。高耸入云的花岗石山岩，气势磅礴的瀑布，以及空幽迷人的山谷…赋予这个国家公园「神地」的美名。中午十分到达佛雷斯诺(Fresno),午餐之后将沿著加州著名的农业高速公路,在傍晚回到洛杉矶,结束这次愉快的旅程。\r\n<BR><br>\r\n<SPAN class=STYLE1>如果您想在当天飞离LAX机场，请安排9：30PM以后的美国国内航班，10：30PM以后的国际航班。我们可以帮助您预订LA 国际机场附近的特假豪华酒店. 您隔天可以方便的乘坐免费往返大巴抵达LAX. 请在支付页面注明您的预订请求,我们为您报价。<br><br>如果您特别在意晚上方便使用中式餐, 可以自费将洛杉矶的酒店调整到 Best Western Executive Inn，Rowland Heights Comfort Suites Rosemead, 或者升级到LA 华人社区最好的酒店: Hilton San Gabriel 。 </SPAN></p>\r\n</DIV></DIV>",
                //接送讯息
                "airport_transfer_info": "",
                //通知
                "notice": "",
                //费用包含
                "includes": "<LI>豪华空调大巴或中巴接送, 每个预定单提供一次9：00AM-10：00PM的免费接机和送机服务 </LI>\r\n<LI>十晚酒店住宿, 所有酒店提供双人床, 标准间 </LI>\r\n<LI>行程中所提及的国家公园门票；环球影视城，迪斯尼乐园或加州冒险乐园门票 </LI>\r\n<LI>精心安排旅馆酒店及大型巴士, 让您的旅程舒适又安全 </LI>\r\n<LI>洛杉矶最具经验的专职双语导游和超过10年驾驶经验的车长</LI>",
                //费用不包含
                "excludes": "<LI>不提供您往返出发地和洛杉矶机场的机票和相关交通费用</LI>\r\n  <LI>所有个人费用和饮食, 行程中的自费项目 </LI>\r\n  <LI>自费旅游项目（价格随实际路线不同而变化)<BR></LI>\r\n    -拉斯维加斯夜晚深度游（成人$25.00 小孩$20）<BR>\r\n    -拉斯维加斯各种秀的表演 （每人$73)<BR>\r\n    -大峡谷立体电影（成人$12.00，小孩$9.00） <BR>\r\n    -赫氏古堡门票（成人$24.00，小孩$12.00）<BR>\r\n    -旧金山渔人码头游轮（成人$26 小孩 $22）<BR>\r\n    -旧金山深度市区游（每人$25，小孩$20）<BR>\r\n    -圣地亚哥巡游观光或旅游大巴观光（成人$15.00，小孩$12.00）\r\n  <LI>不包括提供给导游和司机的小费（每人每天$6.00）</LI>",
                "package_special_note": "<style type=\"text/css\">\r\n<!--\r\n.STYLE1 {color: #F7860f}\r\n-->\r\n</style>\r\n<LI>请注意协调您的航班和旅行团行程的时间。我们建议您在收到您的电子票的所有相关细节确认邮件后再预订您的机票。您的预订通常会在1-2个工作日内得到确认。 </LI>\r\n<LI>请您於第一天与您的导游在洛杉矶机场的行李认领处汇合。</LI>\r\n<LI><span class=\"STYLE1\">如果您选择前往冒险乐园，我们的导游会帮您安排好，但导游不会和您一同前往。</span></LI>\r\n <LI><span class=\"STYLE1\">如果您想在当天飞离LAX机场，请安排9：30PM以后的美国国内航班，10：30PM以后的国际航班。我们可以帮助您预订LAX附近的酒店。您可以第二天早上乘坐酒店的免费往返大巴抵达LAX。请在支付页面注明您的预订请求。</span></LI>\r\n<LI>如遇因天气或其他无法预料的情况而导致当天您乘坐的航班延误超过45分钟的，请您自行安排前往下榻酒店。您也可以联系当地的旅行团供应商，看是否能给予您一些帮助。</LI>\r\n<LI>我们强烈建议您在出发前联系航空公司和地方旅行团供应商以确认好您的航班抵达时间和接机安排事宜。 </LI>\r\n<LI><span class=\"STYLE1\">签证不是必需的。但是，请携带有您照片的身份证明和国籍证明 （美国出生证或者入籍证）以便出美国国境以后重新进入。强烈推荐使用护照。年龄在18岁及以下的儿童需要提供出生证明。如果您不是美国公民或者美国永久性居民（permanent resident），请携带您的护照，I-94卡或者侨民卡（resident alien card）。由於边境安全局势紧张，部分国家的游客需要提供附加文档。此条只适用於极少数国家。请留意您国家或者地区的状况或者和当地移民局联系以确定您能多次出入美国。这样将会避免不必要的拖延。如果任何一个游客因为再次进入美国的问题被扣留，附加文档申请期间我们将不做等待。交通运输可能会另外收取费用。需多次进出美国有效签证。</span></LI>\r\n<LI>英语和美元在美国与墨西哥边境是普遍使用和流通的。 </LI>\r\n<LI>请於班机起飞前二小时抵达机场，以免拥挤及延迟办理登机手续。 </LI>\r\n<LI>搭乘飞机时，请随时扣紧安全带，以免乱气流影响安全。 </LI>\r\n<LI>行程先后次序可能会因出发日期而作调整。 </LI>\r\n<LI>住宿饭店时请随时将房门扣上安全锁，以测安全；勿在灯上晾衣物；勿在床上吸烟，听到警报器响，请由紧急出口迅速离开。 </LI>\r\n<LI>每个酒店房间只安排两张床;三人/四人同房如需加床请自行向酒店服务台查询。 </LI>\r\n<LI>团体需一起活动，途中若要离队需征得导游同意以免发生意外。 </LI>\r\n<LI>夜间或自由活动时间若需自行外出，请告知导游或团友，并应特别注意安全。 </LI>\r\n<LI>新年、国庆日、劳动节或其他长周末假期, 团费会有适当的调整, 请在订团前先确认价钱。 </LI>\r\n<LI>如遇特别情形, (天气,修路,罢工,封山,旅游车特殊状况) 为保障旅客权益, 本公司保留调整取消行程的最终解释权。 </LI>\r\n<LI>春夏两季：请您注意穿著轻便的衣物和舒适的鞋子。<BR>秋冬两季：请您注意穿著厚实的衣物以保暖。</LI><LI>途风温馨提示：<BR>为保障您的个人财产安全，我们建议您在旅行期间随身携带个人贵重物品，不要将贵重物品遗留在大巴/酒店/景点/餐馆等地点；<BR>在任何情况及任何地点下失窃，造成个人财产损失，途风、地接社及司机、领队导游等均不负任何责任，请您悉知。</LI>",
                "price_special_note": "<style type=\"text/css\">\n<!--\n.STYLE4 {font-weight: bold; font-family: \"Times New Roman\", Times, serif; color: #F7860F;}\n.STYLE5 {color: #F7860F}\n-->\n</style>\n<p align=\"left\" class=\"STYLE5\">*此行程逢美国长周末或国定假日(如纪念日，独立日，劳工节等)，价格会有浮动。敬请见谅。</p><div class=\"pr_2\">\n<div class=\"p_p\">*单人间价格是指一人单独享有一个酒店标准间的价格。</div>\n<div class=\"p_p\">*双人/三人/四人间是指双人/三人/四人共同享用一个酒店标准间的价格。  </div>\n<div class=\"p_p\">*三人/四人间价格不包括在房间里另加床位的价格,另加床位要在登记时单独提出要求。 </div> \n<div class=\"p_p\">*2-9岁儿童的价格是指在一个酒店的标准间享用第三或第四个人床位的价格。 </div> \n<div class=\"p_p\">*一个房间最多只能容纳包括成人和小孩或婴儿在内共四人。</div>\n</div>",
                "eticket_special_note": "--如果是第一天自行入住酒店且不需要接机服务的贵宾, 请务必当日在工作时间联络当地巴士部门或者途风以确认第二天的出发时间。\n\n接送机时给司机的小费:每人$3.00\n\n\n签证不是必需的。但是，请携带有您照片的身份证明和国籍证明 （美国出生证或者入籍证）以便出美国国境以后重新进入。强烈推荐使用护照。年龄在18岁及以下的儿童需要提供出生证明。如果您不是美国公民或者美国永久性居民（permanent resident），请携带您的护照，I-94卡或者侨民卡（resident alien card）。由於边境安全局势紧张，部分国家的游客需要提供附加文档。此条只适用於极少数国家。请留意您国家或者地区的状况或者和当地移民局联系以确定您能多次出入美国。这样将会避免不必要的拖延。如果任何一个游客因为再次进入美国的问题被扣留，附加文档申请期间我们将不做等待。交通运输可能会另外收取费用。需多次进出美国有效签证。",
                //提示
                "tips": "",
                //seo
                "seo": {
                    "title": "",
                    "description": "",
                    "keywords": ""
                },
                //促销须知
                "additional_promotion": "",
                //证件须知
                "credential": "",
                //取消/更改须知
                "change_notice": "",
                //自动确认收货须知
                "auto_confirm": "",
                //行程须知
                "travel_notice": "",
                //产品提示
                "product_tips": ""
            },
            //服务语言
            "language": [
                {
                    "language_type": "live",
                    "name": "Chinese Live",
                    "icon": "chinese_live.jpg"
                },
                {
                    "language_type": "live",
                    "name": "English Live",
                    "icon": "english_live.jpg"
                }
            ],
            //行程信息 (多日游(product_line为tour)部分产品有多条行程可供选择)
            "itinerary": [
                {
                    //行程名称
                    "itinerary_title": "线路1",
                    //行程编号
                    "itinerary_no": 1,
                    "itinerary_days_info": [
                        {
                            "itinerary_id": 234,
                            //第几天
                            "day_no": 1,
                            //行程里程数
                            "mileage": 0,
                            //提示
                            "tips": "<b><font color=\"#f7860f\"><font size=\"2\">奥特莱斯倾情推荐，尽享美妙购物之旅：</b></font></font><br>\r\n<b>城堡奥特莱斯——加州风格，物美价廉</b><br>\r\n城堡奥特莱斯是洛杉矶地区唯一一家折扣店，汇集了130个世界级品牌，店内设有高档休息间、货币兑换中心、重新打包区、国际快递等服务区，为顾客提供极致购物体验。当然这里拥有纯正的加州风格，有数不清的景点和各种著名的娱乐场所、主题公园，同时毗邻美丽的加州海岸。赶快来城堡奥特莱斯，体验正宗的加州风情！<br>\r\n营业时间：10:00-21:00(周一至周日)<br>\r\n地址：100 Citadel Drive, Suite 480 Los Angele<br><br>\r\n获取城堡奥特莱斯优惠券，请戳这里：</span><a href=\"http://cn.toursforfun.com/citadel-\r\noutlets-discount-coupon.html\" target=\"_blank\">城堡奥特莱斯购物折扣券</a></font>，享途风独家优惠(数量有限，先到先得)：<br>\r\n* 途风客人到达Citadel Outlets客服中心可获赠折扣券、购物袋、瓶装水礼包一份<br>\r\n* 途风客人到达Citadel Outlets客服中心可获得VIP贵宾休息室礼遇<br><br>\r\n",
                            //描述
                            "summary": "fwefwef<br />\r\nfwqfwef<br />\r\n方法违反<br />\r\n我符文<br />\r\nfwefewfwef",
                            //行程标题
                            "title": "<img src=\"http://cdn.tff.bz/f2/windtour/9d/de/20171221072922022725321.png\" style=\"width: 883px; height: 436px;\" />原居地(Home) - 洛杉矶(Los Angeles)",
                            //景点
                            "attractions": [
                                {
                                    "attraction_id": 284346,
                                    //时间单位
                                    "duration_type": "day",
                                    //时间
                                    "duration": "0.0",
                                    //是否为可选
                                    "is_optional": 0,
                                    "city_description": {
                                        "name": "洛杉矶国际机场",
                                        "pinyin": "L",
                                        "alias": "",
                                        "description": "洛杉矶国际机场是美国加州大洛杉矶地区的主要机场，当地人一般皆以洛杉矶国际机场的代号“LAX”来称呼该机场，洛杉矶国际机场1948 年投入商用航班营运，一直是洛杉矶地区的主要机场。洛杉矶国际机场是最有名民航飞机迷观赏飞机的机场之一。其中，Imperial Hill 地区为著名观机的地点，整个机场的南面由此处可一览无遗。此外，位在24左跑道与24右跑道端靠近 In-N-Out汉堡速食店旁的草地，更是飞机迷经常造访之处。在此处观赏民航班机，最大的好处，是有机会可以看到各种不同机型，飞越头顶上空而降落的壮观景像。",
                                        "transportation": "",
                                        "languages": "",
                                        "feature_foods": "",
                                        "religious_culture": "",
                                        "tips": "",
                                        "operate_tips": "",
                                        "tour_city_id": 466,
                                        "language_id": 3,
                                        "image": "TourCity201405271401213175_5384d0f7b4a7c.jpg"
                                    }
                                }
                            ],
                            //酒店
                            "hotels": [
                                {
                                    "hotel_id": 150399,
                                    //名称
                                    "name": "Howard Johnson Fullerton",
                                    //描述
                                    "description": "",
                                    //图片
                                    "image_url": ""
                                }
                            ],
                            //城市
                            "citys": [
                                {
                                    "city_id": 176614,
                                    "city_description": {
                                        "name": "洛杉矶",
                                        "pinyin": "L",
                                        "alias": "",
                                        "description": "洛杉矶位于美国加州西南部，是美国的第二大城，仅次于纽约，美国最大的海港。全世界的文化、科学、技术、国际贸易和高等教育中心之一，还拥有世界知名的各种专业与文化领域的机构。该市及紧邻的区域，洛杉矶已为美国石油化工、海洋、航天工业和电子业的最大基地，它是美国科技的主要中心之一，拥有美国西部最大的海港，享有“科技之城”的称号。洛杉矶成为在美国仅次于纽约的金融中心。洛杉矶是全球文化、科技、媒体、经济、国际贸易中心城市之一。"
                                    }
                                }
                            ],
                            //餐食信息
                            "meals": [
                                {
                                    "meal_id": 9363,
                                    "name": "早餐：自理",
                                    "description": "",
                                    "image_url": ""
                                },
                                {
                                    "meal_id": 9364,
                                    "name": "午餐：自理",
                                    "description": "",
                                    "image_url": ""
                                }
                            ],
                            //自费
                            "ownexpenses": [
                                {
                                    "ownexpense_id": 97950,
                                    //价格
                                    "price": "",
                                    //提示
                                    "tips": "test",
                                    "ownexpense_description": {
                                        "name": "宾汉峡谷lyc铜矿",
                                        "description": ""
                                    }
                                },
                            ]
                        }
                    ]
                },
                {
                    "itinerary_title": "线路2",
                    "itinerary_no": 2,
                    "itinerary_days_info": [
                        {
                            "itinerary_id": 148384,
                            "day_no": 1,
                            "mileage": 0,
                            "tips": "D",
                            "summary": "!",
                            "title": "<",
                            "attractions": [],
                            "hotels": [],
                            "citys": [],
                            "meals": [],
                            "ownexpenses": [
                                {
                                    "ownexpense_id": 97950,
                                    "price": "",
                                    "tips": "test",
                                    "ownexpense_description": {
                                        "name": "宾汉峡谷lyc铜矿",
                                        "description": ""
                                    }
                                },
                                {
                                    "ownexpense_id": 97951,
                                    "price": "成人$45.00/人、小孩$40人,老人$40人",
                                    "tips": "夜游根据天气有变111",
                                    "ownexpense_description": {
                                        "name": "拉斯维加斯夜游+拉斯维加斯",
                                        "description": ""
                                    }
                                },
                                {
                                    "ownexpense_id": 97952,
                                    "price": "成人$49.00/人; 小孩$15.00/人(3-11)",
                                    "tips": "",
                                    "ownexpense_description": {
                                        "name": "太浩湖游船",
                                        "description": ""
                                    }
                                },
                                {
                                    "ownexpense_id": 97953,
                                    "price": "$60.00/成人；$40.00/小孩(5-10)",
                                    "tips": "为了拍摄美景，强烈建议您参加此自费项目，如果您不参加则只能看到小部分的鲍威尔湖。",
                                    "ownexpense_description": {
                                        "name": "鲍威尔湖游船",
                                        "description": ""
                                    }
                                }
                            ]
                        }
                    ]
                }
            ],
            "media": {
                //产品主图
                "image_url": "sg3da.jpg",
                //产品图片
                "extra": [
                    "201403181395127991_5327f6b7d89d5_watermark_800_800.jpg",
                    "201403181395132288_5328078031b42_watermark_800_800.jpg",
                    "201403181395131355_532803db6a228_watermark_800_800.jpg",
                    "201403181395131190_532803366ce5c_watermark_800_800.jpg",
                    "201403181395130954_5328024a31c89_watermark_800_800.jpg",
                    "201403181395130527_5328009f5b816_watermark_800_800.jpg",
                    "201403181395130451_53280053b0998_watermark_800_800.jpg",
                    "201403181395130294_5327ffb6584f6_watermark_800_800.jpg",
                    "201403181395129883_5327fe1be5e03_watermark_800_800.jpg",
                    "201403181395129533_5327fcbd08383_watermark_800_800.jpg",
                    "201403181395129448_5327fc68725c3_watermark_800_800.jpg",
                    "201403181395128893_5327fa3dc717b_watermark_800_800.jpg",
                    "201403181395128657_5327f9517575e_watermark_800_800.jpg",
                    "201403181395128287_5327f7dfc74d0_watermark_800_800.jpg",
                    "http://images.tours4fun.com/images/db/products/Los-Angeles%202.jpg",
                    "2587_APHTP-HV5-tours-1.jpg",
                    "http://images.tours4fun.com/images/db/products/Disneyland.jpg",
                    "http://images.tours4fun.com/images/db/products/0414_Las-Vegas_2.jpg",
                    "http://images.tours4fun.com/images/db/products/Solvang_3.jpg",
                    "http://images.tours4fun.com/images/db/products/0415_San-Francisco_.jpg"
                ]
            },
            //旅客预定需填信息
            "passengerForm": {
                "lastname_en": {
                    "name": "lastname_en",
                    "label": "姓氏",
                    "type": "text",
                    "min": "",
                    "max": "",
                    "options": [
                        ""
                    ],
                    "placeholder": ""
                },
                "firstname_en": {
                    "name": "firstname_en",
                    "label": "名字",
                    "type": "text",
                    "min": "",
                    "max": "",
                    "options": [
                        ""
                    ],
                    "placeholder": ""
                },
                "passport": {
                    "name": "passport",
                    "label": "护照",
                    "type": "text",
                    "min": "",
                    "max": "",
                    "options": [],
                    "placeholder": ""
                },
                "passport_expire": {
                    "name": "passport_expire",
                    "label": "护照过期日期",
                    "type": "date",
                    "min": "",
                    "max": "",
                    "options": [],
                    "placeholder": ""
                },
                "mobile": {
                    "name": "mobile",
                    "label": "电话",
                    "type": "phone",
                    "min": "",
                    "max": "",
                    "options": [],
                    "placeholder": ""
                },
                "email": {
                    "name": "email",
                    "label": "邮箱",
                    "type": "text",
                    "min": "",
                    "max": "",
                    "options": [],
                    "placeholder": ""
                },
                "gender": {
                    "name": "gender",
                    "label": "性别",
                    "type": "radio",
                    "options": [
                        "未知",
                        "男",
                        "女"
                    ],
                    "min": "",
                    "max": "",
                    "placeholder": ""
                },
                "dob": {
                    "name": "dob",
                    "label": "出生日期",
                    "type": "date",
                    "min": "",
                    "max": "",
                    "options": [],
                    "placeholder": ""
                },
                "nation": {
                    "name": "nation",
                    "label": "国籍",
                    "type": "text",
                    "min": "",
                    "max": "",
                    "options": [],
                    "placeholder": ""
                },
                "weight": {
                    "name": "weight",
                    "label": "体重",
                    "type": "number",
                    "min": "",
                    "max": "",
                    "options": [],
                    "placeholder": ""
                },
                "weight_unit": {
                    "name": "weight_unit",
                    "label": "体重单位",
                    "type": "select",
                    "options": [
                        "kg",
                        "pound"
                    ],
                    "min": "",
                    "max": "",
                    "placeholder": ""
                }
            }
        }
    }
    
    一日游(product_line为activity):
    {
            "code": 0,
            "msg": "success",
            "data": {
                "base": {
                    "product_id": 13374,
                    //产品老id
                    "product_id_old": "1568",
                    //产品线
                    "product_line": "activity",
                    //产品名称
                    "name": "洛杉矶迪斯尼乐园超值欢乐一日游",
                    //产品主图
                    "image_url": "sg3da.jpg",
                    //建议价格
                    "advertised_price": 755,
                    //价格货币类型
                    "currency": "USD",
                    //行程时间
                    "duration": 1,
                    //行程时间单位 day,hour,minute
                    "duration_type": "day",
                    //库存状态
                    "stock_status": 1,
                    //最大小孩年龄
                    "max_child_age": 11,
                    //提前预定天数
                    "min_days_before_departure": 0,
                    //最小出团人数
                    "min_guest_number": 1,
                    //是否显示自费项目
                    "show_ownexpense": 0,
                    "visa_passport": 0,
                    //是否提供出发接送服务
                    "is_pickup": 2,
                    //是否提供到达接送服务
                    "is_dropoff": 2,
                    "hotel_pickup": 0,
                    //出发城市(可以多个)
                    "departure_city": [
                        {
                            "departure_city_id": 1,
                            "departure_city_name": "洛杉矶"
                        }
                    ],
                    //回团城市(可以多个)
                    "return_city": [
                        {
                            "return_city_id": 1,
                            "return_city_name": "洛杉矶"
                        }
                    ],
                    //产品区域中文名
                    "region_chinese_name": "美国",
                    //产品子区域中文名
                    "sub_region_chinese_name": "美西",
                    "region": "us",
                    "sub_region": "west"
                },
                "info": {
                    //简要描述、推荐
                    "brief_description": "您将超值游览到迪士尼乐园、加州著名的丹麦城、拥有价值连城的古董和艺术品的赫氏古堡、文化名城旧金山。而风景秀丽的优胜美地国家公园会让您恍若置身世外桃园。除此之外，享有“世界娱乐之都”美誉的拉斯维加斯、鬼斧神工的科罗拉多大峡谷和拥有工业世界七大奇观之一美誉的胡佛大坝更是您不容错过的特色景点。著名的好莱坞环球影城主题公园将会为您的旅程增光添彩。还有迷人的墨西哥恩森那达绽放光彩。",
                    //详细描述
                    "full_description": "<STYLE type=text/css>\r\n<!--\r\n.STYLE1 {color: #F7860F}\r\n-->\r\n</STYLE>\r\n\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第一天 </SPAN>原居地(Home)-洛杉矶(Los Angeles)<BR></H5></DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/los-angeles-skyline-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1>\r\n  <p class=\"main\">当您降落於洛杉矶机场的时候,我们热情的导游将在<span class=\"STYLE1\">行李认领处</span>等候您的到来。之后，导游会把您带往下榻的酒店，您可以自行安排余下的时间。（希望可以在当地时间下午3：00pm以后到达，办理酒店登记手续。）</p></DIV>\r\n<DIV class=p_p>\r\n<TABLE>\r\n<TBODY>\r\n<TR>\r\n<TD><img src=\"http://images.tours4fun.com/image/f.gif\" /></TD>\r\n<TD>+ </TD>\r\n<TD><IMG src=\"http://images.tours4fun.com/image/upgrad_hotel.gif\"></TD>\r\n<TD><B><SPAN class=hotel_title>酒店</SPAN>: Anaheim Park Hotel 或 Holidays Inn Hotel La Mirada 或者同等级的酒店</B></TD>\r\n</TR></TBODY></TABLE></DIV></DIV>\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第二天 </SPAN>洛杉矶(Los Angeles)-罗莎丽多(Rosarito)-恩塞那达(Ensenada)<BR>\r\n</H5>\r\n</DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/ensenada-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1>\r\n  <p class=\"main\">早上我们从洛杉矶出发，迎著和煦的阳光，沿著加州公路南下，穿越美墨边城蒂娃娜，进入了一号海滨公路。碧蓝的海水，洁白的沙滩，马上映入您的眼帘。中午时分来到著名的罗莎丽多海滨渡假城，您可坐在露天餐厅享受著阳光，或自费骑马奔驰在沙滩上。傍晚进入渔港之都－恩森那达。抵达酒店后，自由活动,您可以漫步於城中，购买精美价廉的墨西哥手工艺品：皮包，皮衣，然后饱尝新鲜海鱼，龙虾等海鲜大餐，迷人的拉丁音乐风情，伴您进入梦乡。</p></DIV>\r\n<DIV class=p_p>\r\n<TABLE>\r\n<TBODY>\r\n<TR>\r\n<TD><img src=\"http://images.tours4fun.com/image/f.gif\" /></TD>\r\n<TD><B><SPAN class=hotel_title>酒店:</SPAN><SPAN class=mainblue>Santo Tomasl 或 San Nicolas Resort  或者同等级酒店</SPAN></B></TD>\r\n</TR></TBODY></TABLE></DIV></DIV>\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第三天 </SPAN>恩塞那达(Ensenada)-拉普发多拉天然海水喷泉(La Bufadora)-科罗娜多岛(Coronado Island)<BR></H5>\r\n</DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/colorado-island-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1>\r\n  <p class=\"main\">上午前往拉普发多拉天然海水喷泉，沿著海岸可看见光怪陆离的岩穴，海水拍岸，浪花四溅，堪称海上奇景。午后沿著黄金海岸北上，回到美国西岸最大的军港城市圣地牙哥。穿越跨海大桥，来到哥罗娜多岛，美丽的海滩，绿草如茵的高尔夫球场，同时参观加州最古老的哥罗娜多酒店。此酒店已有百年历史，爱迪生曾亲自监督该旅馆照明设备之安装，英国皇室之温莎公爵也曾下榻於此。此外，曾有十二位美国总统莅临开会及渡假。经由跨海大桥，俯瞰军港及海湾美景并转赴古城游览。古城为加州之发源地，其高耸入云的旗杆，曾升上南加第一面国旗，思古幽情中，充满了南美拉丁色彩之艺术品及文物，然后踏著夕阳，带著美好的回忆，大约在傍晚7：00回到洛杉矶。</p></DIV>\r\n<DIV class=p_p>\r\n<TABLE>\r\n<TBODY>\r\n<TR>\r\n<TD><img src=\"http://images.tours4fun.com/image/f.gif\" /></TD>\r\n<TD>+ </TD>\r\n<TD><IMG src=\"http://images.tours4fun.com/image/upgrad_hotel.gif\"></TD>\r\n<TD><B><SPAN class=hotel_title>酒店：Anaheim Park Hotel 或 Holidays Inn Hotel La Mirada 或者同等级的酒店</SPAN> </B></TD></TR></TBODY></TABLE></DIV></DIV>\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第四天 </SPAN>迪斯尼乐园或者加州冒险乐园(Disney or Adventure Park)<BR></H5></DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/los-angeles-disneyland-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1>\r\n  <p class=\"main\">清晨大约7时左右，由洛杉矶出发沿5号州际高速公路向南到达橙县，去到座落在加州的全世界闻名迪斯尼乐园。在专业的导游一天的时间当中为您特别挑选出一些最为值得参加的游乐项目，让您感觉到目不转睛，惊险无比。傍晚之后，再由导游送回到酒店休息。</p></DIV>\r\n<DIV class=p_p>\r\n<TABLE>\r\n<TBODY>\r\n<TR>\r\n<TD><img src=\"http://images.tours4fun.com/image/f.gif\" /></TD>\r\n<TD>+ </TD>\r\n<TD><IMG src=\"http://images.tours4fun.com/image/upgrad_hotel.gif\"></TD>\r\n<TD><B><SPAN class=hotel_title>酒店：Anaheim Park Hotel 或 Holidays Inn Hotel La Mirada 或者同等级的酒店</SPAN> </B></TD></TR></TBODY></TABLE></DIV></DIV>\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第五天 </SPAN>好莱坞环球影城主题公园(Universal Studios)<BR></H5></DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/hollywood-universal-studio-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1><SPAN class=main>早上出发后，到达著名的好莱坞星光大道，参观著名的中国大剧院，柯达剧院，明星手印，之后进入环电影制片主题公园。这次旅程将带您游历城里的恐怖片的拍摄场景。在这里您可以充分的体验场面宏大的表演和动物秀，以及幽默滑稽的儿童节目。</span></DIV>\r\n<DIV class=p_p>\r\n<TABLE>\r\n<TBODY>\r\n<TR>\r\n<TD><img src=\"http://images.tours4fun.com/image/f.gif\" /></TD>\r\n<TD>+ </TD>\r\n<TD><IMG src=\"http://images.tours4fun.com/image/upgrad_hotel.gif\"></TD>\r\n<TD><STRONG><SPAN class=hotel_title>酒店</SPAN>: </STRONG><B>Anaheim Park Hotel 或 Holidays Inn Hotel La Mirada 或者同等级的酒店</B></TD>\r\n</TR></TBODY></TABLE></DIV></DIV>\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第六天 </SPAN><SPAN class=heading_text>洛杉矶(Los Angeles)-巴斯多(Basedow)-拉斯维加斯(Las Vegas) （约266英里）\r\n</SPAN><BR></H5>\r\n</DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/barstow-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1>\r\n  <p class=\"main\">清晨我们将从洛杉矶出发，开始精彩的三天之旅。驱车途经圣贝纳迪诺山和莫哈韦大沙漠。中午时分，团体特别为我们会在巴斯多－从洛杉矶到拉斯维加斯途中的一个工厂直销商场做一个短暂的购物休息，并且在这里享用午餐。之后前往拉斯维加斯，晚上您可以自由活动。</p></DIV>\r\n<DIV class=p_p>\r\n<TABLE>\r\n<TBODY>\r\n<TR>\r\n<TD><img src=\"http://images.tours4fun.com/image/f.gif\" /></TD>\r\n<TD><B><SPAN class=hotel_title>酒店</SPAN>: Stratosphere Hotel 或 <SPAN class=mainblue>Plaza Casino Hotel, Las Vegas  或者同等级酒店</SPAN></B></TD>\r\n</TR></TBODY></TABLE></DIV></DIV>\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第七天 </SPAN>拉斯维加斯(Las Vegas)-大峡谷国家公园(Grand Canyon)-胡佛水坝(Hoover Dam)-拉斯维加斯(Las Vegas) （约520英里） \r\n<BR></H5>\r\n</DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/grand_canyon-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1>\r\n  <p class=\"main\">清晨前往拥有世界七大奇景美誉的科罗拉多大峡谷国家公园。这是世界上最为鲜活的侵蚀范本，也使游客无不面对这造物主的鬼斧神工而感慨万千。之后前往参观美国历史上最为著名的水利工程之一-位于科罗拉多河上的胡佛水霸,并且可以遥望西海岸最大的米德人工湖。下午，再此满怀期待的回到这个世界娱乐之都-罪恶之城,拉斯维加斯。 您可在下榻的酒店一试手气，或者安排各种酒店表演。</p></DIV>\r\n<DIV class=p_p>\r\n<TABLE>\r\n<TBODY>\r\n<TR>\r\n<TD><img src=\"http://images.tours4fun.com/image/f.gif\" /></TD>\r\n<TD><B><SPAN class=hotel_title>酒店:</SPAN> Stratosphere Hotel 或 Plaza Casino Hotel, Las Vegas <SPAN class=mainblue>或者同等级酒店</SPAN></B></TD>\r\n</TR></TBODY></TABLE></DIV></DIV>\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第八天 </SPAN><SPAN class=heading_text>拉斯维加斯(Las Vegas)-巧克力工厂(Hershey Chocolate Factory)-工厂直销商场(Outlet Factory)-洛杉矶(Los Angeles) （约270英里）\r\n</SPAN><BR></H5>\r\n</DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/las-vegas-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1>\r\n  <p class=\"main\">清晨我们将前往参观巧克力工厂，让您亲眼目睹巧克力的生产过程。您还可以购买各种精致的巧克力。大约中午11:00左右，我们会向洛杉矶进发。中途会再次路径巴斯多用午餐和做简单购物。大约下午6：00会回到洛杉矶。</p></DIV>\r\n<DIV class=p_p>\r\n<TABLE>\r\n<TBODY>\r\n<TR>\r\n<TD><img src=\"http://images.tours4fun.com/image/f.gif\" /></TD>\r\n<TD>+ </TD>\r\n<TD><IMG src=\"http://images.tours4fun.com/image/upgrad_hotel.gif\"></TD>\r\n<TD><B><SPAN class=hotel_title>酒店:</SPAN> Anaheim Park Hotel 或 Holidays Inn Hotel La Mirada 或者同等级的酒店</B></TD>\r\n</TR></TBODY></TABLE></DIV></DIV>\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第九天 </SPAN><SPAN class=heading_text>洛杉矶(Los Angelea)-<strong>丹麦城(Solvang)</strong>-赫氏古堡(Hearst Castle)-</SPAN>旧金山(San Francisco) （约380英里）<BR></span></H5>\r\n</DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/solvang-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1>\r\n  <p class=\"main\">早上离开LA最大的华人社区--蒙特利公园城市，沿途欣赏太平洋海岸线公路的美景，抵达加州著名的丹麦城--享受加州阳光和丹麦咖啡的温情与浪漫. 接著继续北行游览赫斯特城堡，在<span class=\"heading_text\">赫氏古堡</span>里，你可以观赏价值连城的古董和艺术品，甚至是装饰华丽，镀金的小泳池，宏伟的主礼堂威严耸立，令人瞩目。晚上留宿旧金山。</p></DIV>\r\n<DIV class=p_p>\r\n<TABLE>\r\n<TBODY>\r\n<TR>\r\n<TD><img src=\"http://images.tours4fun.com/image/f.gif\" /></TD>\r\n<TD><B><SPAN class=hotel_title>酒店:</SPAN><SPAN class=mainblue> Courtyard Marriott Silicon Valley, Fremont 或Comfort Inn Cockatoo或者同等级酒店</span></B></TD>\r\n</TR></TBODY></TABLE></DIV></DIV>\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第十天 </SPAN>旧金山(San Francisco)<strong>市区游览</strong><BR></H5>\r\n</DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/san-francisco-skyline-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1>\r\n  <p class=\"main\">清晨大约40分钟驱车前往加州历史、文化名城--旧金山。「雾锁金门」是这的特有景观。华裔移民聚居在中国城，意大利后裔在北滩创建「小意大利区」，当今渔人码头已成观光胜地。你还可以选择自费乘船游览海湾。富豪岗立即展现了淘金热与铁路供给的金碧辉煌；俄罗斯山的陡峭，反而成就了伦巴街独特的九曲十八弯。艺术宫的古罗马建筑，使人们对巴拿马博览会的盛况浮想联翩。傍晚9时回到位于莫德斯托的酒店。</p></DIV>\r\n<DIV class=p_p>\r\n<TABLE>\r\n<TBODY>\r\n<TR>\r\n<TD><img src=\"http://images.tours4fun.com/image/f.gif\" /></TD>\r\n<TD><B><SPAN class=hotel_title>酒店:</SPAN><SPAN class=mainblue> Courtyard Marriott Silicon Valley, Fremont 或Comfort Inn Cockatoo或者同等级酒店</B></TD>\r\n</TR></TBODY></TABLE></DIV></DIV>\r\n<DIV class=pl_1>\r\n<DIV class=p_p>\r\n<H5 class=sp4><SPAN class=sp2>第十一天 </SPAN>莫德斯托(Modesto)<SPAN class=heading_text>-优胜美地国家公园(Yosemite)</SPAN>-洛杉矶 （约312英里） \r\n(Los Angeles)<BR></H5>\r\n</DIV>\r\n<div class=\"p_p_img\"><img src=\"http://images.tours4fun.com/images/db/products/yosemite-national-park-pic.jpg\" class=\"img_border\" /></div> \r\n<DIV class=p_p_1>\r\n  <p class=\"main\">清晨继续前行游览加州最出名的国家公园之一--优胜美地国家公园（Yosemite National Park），它坐落于内华达州山脉的中，是一处自然奇观。高耸入云的花岗石山岩，气势磅礴的瀑布，以及空幽迷人的山谷…赋予这个国家公园「神地」的美名。中午十分到达佛雷斯诺(Fresno),午餐之后将沿著加州著名的农业高速公路,在傍晚回到洛杉矶,结束这次愉快的旅程。\r\n<BR><br>\r\n<SPAN class=STYLE1>如果您想在当天飞离LAX机场，请安排9：30PM以后的美国国内航班，10：30PM以后的国际航班。我们可以帮助您预订LA 国际机场附近的特假豪华酒店. 您隔天可以方便的乘坐免费往返大巴抵达LAX. 请在支付页面注明您的预订请求,我们为您报价。<br><br>如果您特别在意晚上方便使用中式餐, 可以自费将洛杉矶的酒店调整到 Best Western Executive Inn，Rowland Heights Comfort Suites Rosemead, 或者升级到LA 华人社区最好的酒店: Hilton San Gabriel 。 </SPAN></p>\r\n</DIV></DIV>",
                    //接送讯息
                    "airport_transfer_info": "",
                    //通知
                    "notice": "",
                    //费用包含
                    "includes": "<LI>豪华空调大巴或中巴接送, 每个预定单提供一次9：00AM-10：00PM的免费接机和送机服务 </LI>\r\n<LI>十晚酒店住宿, 所有酒店提供双人床, 标准间 </LI>\r\n<LI>行程中所提及的国家公园门票；环球影视城，迪斯尼乐园或加州冒险乐园门票 </LI>\r\n<LI>精心安排旅馆酒店及大型巴士, 让您的旅程舒适又安全 </LI>\r\n<LI>洛杉矶最具经验的专职双语导游和超过10年驾驶经验的车长</LI>",
                    //费用不包含
                    "excludes": "<LI>不提供您往返出发地和洛杉矶机场的机票和相关交通费用</LI>\r\n  <LI>所有个人费用和饮食, 行程中的自费项目 </LI>\r\n  <LI>自费旅游项目（价格随实际路线不同而变化)<BR></LI>\r\n    -拉斯维加斯夜晚深度游（成人$25.00 小孩$20）<BR>\r\n    -拉斯维加斯各种秀的表演 （每人$73)<BR>\r\n    -大峡谷立体电影（成人$12.00，小孩$9.00） <BR>\r\n    -赫氏古堡门票（成人$24.00，小孩$12.00）<BR>\r\n    -旧金山渔人码头游轮（成人$26 小孩 $22）<BR>\r\n    -旧金山深度市区游（每人$25，小孩$20）<BR>\r\n    -圣地亚哥巡游观光或旅游大巴观光（成人$15.00，小孩$12.00）\r\n  <LI>不包括提供给导游和司机的小费（每人每天$6.00）</LI>",
                    "package_special_note": "<style type=\"text/css\">\r\n<!--\r\n.STYLE1 {color: #F7860f}\r\n-->\r\n</style>\r\n<LI>请注意协调您的航班和旅行团行程的时间。我们建议您在收到您的电子票的所有相关细节确认邮件后再预订您的机票。您的预订通常会在1-2个工作日内得到确认。 </LI>\r\n<LI>请您於第一天与您的导游在洛杉矶机场的行李认领处汇合。</LI>\r\n<LI><span class=\"STYLE1\">如果您选择前往冒险乐园，我们的导游会帮您安排好，但导游不会和您一同前往。</span></LI>\r\n <LI><span class=\"STYLE1\">如果您想在当天飞离LAX机场，请安排9：30PM以后的美国国内航班，10：30PM以后的国际航班。我们可以帮助您预订LAX附近的酒店。您可以第二天早上乘坐酒店的免费往返大巴抵达LAX。请在支付页面注明您的预订请求。</span></LI>\r\n<LI>如遇因天气或其他无法预料的情况而导致当天您乘坐的航班延误超过45分钟的，请您自行安排前往下榻酒店。您也可以联系当地的旅行团供应商，看是否能给予您一些帮助。</LI>\r\n<LI>我们强烈建议您在出发前联系航空公司和地方旅行团供应商以确认好您的航班抵达时间和接机安排事宜。 </LI>\r\n<LI><span class=\"STYLE1\">签证不是必需的。但是，请携带有您照片的身份证明和国籍证明 （美国出生证或者入籍证）以便出美国国境以后重新进入。强烈推荐使用护照。年龄在18岁及以下的儿童需要提供出生证明。如果您不是美国公民或者美国永久性居民（permanent resident），请携带您的护照，I-94卡或者侨民卡（resident alien card）。由於边境安全局势紧张，部分国家的游客需要提供附加文档。此条只适用於极少数国家。请留意您国家或者地区的状况或者和当地移民局联系以确定您能多次出入美国。这样将会避免不必要的拖延。如果任何一个游客因为再次进入美国的问题被扣留，附加文档申请期间我们将不做等待。交通运输可能会另外收取费用。需多次进出美国有效签证。</span></LI>\r\n<LI>英语和美元在美国与墨西哥边境是普遍使用和流通的。 </LI>\r\n<LI>请於班机起飞前二小时抵达机场，以免拥挤及延迟办理登机手续。 </LI>\r\n<LI>搭乘飞机时，请随时扣紧安全带，以免乱气流影响安全。 </LI>\r\n<LI>行程先后次序可能会因出发日期而作调整。 </LI>\r\n<LI>住宿饭店时请随时将房门扣上安全锁，以测安全；勿在灯上晾衣物；勿在床上吸烟，听到警报器响，请由紧急出口迅速离开。 </LI>\r\n<LI>每个酒店房间只安排两张床;三人/四人同房如需加床请自行向酒店服务台查询。 </LI>\r\n<LI>团体需一起活动，途中若要离队需征得导游同意以免发生意外。 </LI>\r\n<LI>夜间或自由活动时间若需自行外出，请告知导游或团友，并应特别注意安全。 </LI>\r\n<LI>新年、国庆日、劳动节或其他长周末假期, 团费会有适当的调整, 请在订团前先确认价钱。 </LI>\r\n<LI>如遇特别情形, (天气,修路,罢工,封山,旅游车特殊状况) 为保障旅客权益, 本公司保留调整取消行程的最终解释权。 </LI>\r\n<LI>春夏两季：请您注意穿著轻便的衣物和舒适的鞋子。<BR>秋冬两季：请您注意穿著厚实的衣物以保暖。</LI><LI>途风温馨提示：<BR>为保障您的个人财产安全，我们建议您在旅行期间随身携带个人贵重物品，不要将贵重物品遗留在大巴/酒店/景点/餐馆等地点；<BR>在任何情况及任何地点下失窃，造成个人财产损失，途风、地接社及司机、领队导游等均不负任何责任，请您悉知。</LI>",
                    "price_special_note": "<style type=\"text/css\">\n<!--\n.STYLE4 {font-weight: bold; font-family: \"Times New Roman\", Times, serif; color: #F7860F;}\n.STYLE5 {color: #F7860F}\n-->\n</style>\n<p align=\"left\" class=\"STYLE5\">*此行程逢美国长周末或国定假日(如纪念日，独立日，劳工节等)，价格会有浮动。敬请见谅。</p><div class=\"pr_2\">\n<div class=\"p_p\">*单人间价格是指一人单独享有一个酒店标准间的价格。</div>\n<div class=\"p_p\">*双人/三人/四人间是指双人/三人/四人共同享用一个酒店标准间的价格。  </div>\n<div class=\"p_p\">*三人/四人间价格不包括在房间里另加床位的价格,另加床位要在登记时单独提出要求。 </div> \n<div class=\"p_p\">*2-9岁儿童的价格是指在一个酒店的标准间享用第三或第四个人床位的价格。 </div> \n<div class=\"p_p\">*一个房间最多只能容纳包括成人和小孩或婴儿在内共四人。</div>\n</div>",
                    "eticket_special_note": "--如果是第一天自行入住酒店且不需要接机服务的贵宾, 请务必当日在工作时间联络当地巴士部门或者途风以确认第二天的出发时间。\n\n接送机时给司机的小费:每人$3.00\n\n\n签证不是必需的。但是，请携带有您照片的身份证明和国籍证明 （美国出生证或者入籍证）以便出美国国境以后重新进入。强烈推荐使用护照。年龄在18岁及以下的儿童需要提供出生证明。如果您不是美国公民或者美国永久性居民（permanent resident），请携带您的护照，I-94卡或者侨民卡（resident alien card）。由於边境安全局势紧张，部分国家的游客需要提供附加文档。此条只适用於极少数国家。请留意您国家或者地区的状况或者和当地移民局联系以确定您能多次出入美国。这样将会避免不必要的拖延。如果任何一个游客因为再次进入美国的问题被扣留，附加文档申请期间我们将不做等待。交通运输可能会另外收取费用。需多次进出美国有效签证。",
                    //提示
                    "tips": "",
                    //seo
                    "seo": {
                        "title": "",
                        "description": "",
                        "keywords": ""
                    },
                    //促销须知
                    "additional_promotion": "",
                    //证件须知
                    "credential": "",
                    //取消/更改须知
                    "change_notice": "",
                    //自动确认收货须知
                    "auto_confirm": "",
                    //行程须知
                    "travel_notice": "",
                    //产品提示
                    "product_tips": ""
                },
                //服务语言
                "language": [
                    {
                        "language_type": "live",
                        "name": "Chinese Live",
                        "icon": "chinese_live.jpg"
                    },
                    {
                        "language_type": "live",
                        "name": "English Live",
                        "icon": "english_live.jpg"
                    }
                ],
                //行程信息
                "itinerary": {
                    //景点
                    "attractions": [
                        {
                            "attraction_id": 5,
                            //时间
                            "duration": 0,、
                            //时间单位
                            "duration_type": "hour",
                            //是否可选
                            "is_optional": 0,
                            //名字
                            "name": "迪斯尼乐园",
                            //描述
                            "description": "加州迪斯尼乐园位于美国加利福尼亚州阿纳海姆市迪斯尼乐园度假区，自1955年7月17日开幕以来，加州迪斯尼乐园就成为世界最受欢迎的主题乐园之一，被人们誉为地球上最快乐的地方。以米老鼠为首的迪斯尼家族，每年都有新成员加入，加上迪斯尼乐园的软硬件不断推陈出新，使得这儿成为观光客前往洛杉矶，绝对不会错过的重要景点。迄今游览过加州迪斯尼乐园的游客已经超过5.5亿，这其中包括国家总统、皇室、世界顶级明星等。挑一个假期，全家大小好好玩乐一番，一定会有跟世界其他迪斯尼乐园不一样的感觉！"
                        },
                        {
                            "attraction_id": 20853,
                            "duration": 0,
                            "duration_type": "hour",
                            "is_optional": 0,
                            "name": "加州冒险乐园",
                            "description": "加州冒险乐园是华特迪士尼公司于美国安纳海姆市所建立的一个主题公园，如同其命名一般，加州冒险乐园是以「加州」作为整个乐园的主题，园内除了设置项加州知名地标的缩比复制品之外，也有不少以该州文化与历史作为主轴的设定。与隔邻的迪士尼乐园主要是以温馨梦幻的儿童客户为对象之风格不同，加州冒险乐园是以年龄层较大的成人客户作为锁定对象，因此园内虽然不乏各项适合阖家老小同乐的游戏项目，但相比之下也拥有较多刺激度较高的游乐设施，是此乐园与其他大部分迪士尼体系的主题乐园较为不相同之处。"
                        }
                    ],
                    //城市
                    "citys": [
                        {
                            "city_id": 1,
                            "name": "洛杉矶",
                            "description": "洛杉矶位于美国加州西南部，是美国的第二大城，仅次于纽约，美国最大的海港。全世界的文化、科学、技术、国际贸易和高等教育中心之一，还拥有世界知名的各种专业与文化领域的机构。该市及紧邻的区域，洛杉矶已为美国石油化工、海洋、航天工业和电子业的最大基地，它是美国科技的主要中心之一，拥有美国西部最大的海港，享有“科技之城”的称号。洛杉矶成为在美国仅次于纽约的金融中心。洛杉矶是全球文化、科技、媒体、经济、国际贸易中心城市之一。"
                        }
                    ],
                    //自费项目
                    "ownexpenses": [
                        {
                            "ownexpense_id": 379,
                            //名字
                            "name": "迪士尼乐园",
                            //描述
                            "description": "",
                            //价格
                            "price": "成人$95.00-$119.00/人；小孩(3-9)$89.00-$113.00/人，价格请以实际确认为准",
                            //时长
                            "duration": "",
                            //提示
                            "tips": "<font color=#f7860f>这是您在团上必付的费用，请直接将费用支付给导游。</font>"
                        }
                    ]
                },
                "media": {
                    //产品主图
                    "image_url": "sg3da.jpg",
                    //产品图片
                    "extra": [
                        "201403181395127991_5327f6b7d89d5_watermark_800_800.jpg",
                        "201403181395132288_5328078031b42_watermark_800_800.jpg",
                        "201403181395131355_532803db6a228_watermark_800_800.jpg",
                        "201403181395131190_532803366ce5c_watermark_800_800.jpg",
                        "201403181395130954_5328024a31c89_watermark_800_800.jpg",
                        "201403181395130527_5328009f5b816_watermark_800_800.jpg",
                        "201403181395130451_53280053b0998_watermark_800_800.jpg",
                        "201403181395130294_5327ffb6584f6_watermark_800_800.jpg",
                        "201403181395129883_5327fe1be5e03_watermark_800_800.jpg",
                        "201403181395129533_5327fcbd08383_watermark_800_800.jpg",
                        "201403181395129448_5327fc68725c3_watermark_800_800.jpg",
                        "201403181395128893_5327fa3dc717b_watermark_800_800.jpg",
                        "201403181395128657_5327f9517575e_watermark_800_800.jpg",
                        "201403181395128287_5327f7dfc74d0_watermark_800_800.jpg",
                        "http://images.tours4fun.com/images/db/products/Los-Angeles%202.jpg",
                        "2587_APHTP-HV5-tours-1.jpg",
                        "http://images.tours4fun.com/images/db/products/Disneyland.jpg",
                        "http://images.tours4fun.com/images/db/products/0414_Las-Vegas_2.jpg",
                        "http://images.tours4fun.com/images/db/products/Solvang_3.jpg",
                        "http://images.tours4fun.com/images/db/products/0415_San-Francisco_.jpg"
                    ]
                },
                //旅客预定需填信息
                "passengerForm": {
                    "lastname_en": {
                        "name": "lastname_en",
                        "label": "姓氏",
                        "type": "text",
                        "min": "",
                        "max": "",
                        "options": [
                            ""
                        ],
                        "placeholder": ""
                    },
                    "firstname_en": {
                        "name": "firstname_en",
                        "label": "名字",
                        "type": "text",
                        "min": "",
                        "max": "",
                        "options": [
                            ""
                        ],
                        "placeholder": ""
                    },
                    "passport": {
                        "name": "passport",
                        "label": "护照",
                        "type": "text",
                        "min": "",
                        "max": "",
                        "options": [],
                        "placeholder": ""
                    },
                    "passport_expire": {
                        "name": "passport_expire",
                        "label": "护照过期日期",
                        "type": "date",
                        "min": "",
                        "max": "",
                        "options": [],
                        "placeholder": ""
                    },
                    "mobile": {
                        "name": "mobile",
                        "label": "电话",
                        "type": "phone",
                        "min": "",
                        "max": "",
                        "options": [],
                        "placeholder": ""
                    },
                    "email": {
                        "name": "email",
                        "label": "邮箱",
                        "type": "text",
                        "min": "",
                        "max": "",
                        "options": [],
                        "placeholder": ""
                    },
                    "gender": {
                        "name": "gender",
                        "label": "性别",
                        "type": "radio",
                        "options": [
                            "未知",
                            "男",
                            "女"
                        ],
                        "min": "",
                        "max": "",
                        "placeholder": ""
                    },
                    "dob": {
                        "name": "dob",
                        "label": "出生日期",
                        "type": "date",
                        "min": "",
                        "max": "",
                        "options": [],
                        "placeholder": ""
                    },
                    "nation": {
                        "name": "nation",
                        "label": "国籍",
                        "type": "text",
                        "min": "",
                        "max": "",
                        "options": [],
                        "placeholder": ""
                    },
                    "weight": {
                        "name": "weight",
                        "label": "体重",
                        "type": "number",
                        "min": "",
                        "max": "",
                        "options": [],
                        "placeholder": ""
                    },
                    "weight_unit": {
                        "name": "weight_unit",
                        "label": "体重单位",
                        "type": "select",
                        "options": [
                            "kg",
                            "pound"
                        ],
                        "min": "",
                        "max": "",
                        "placeholder": ""
                    }
                }
            }
        }