# Product Detail

### Description

Get product details information in batches according to product ID. The data structure is different depending on the product line your product belongs to. When doing code logic processing, please follow the data type processing of the product line.


### API URL

    /v2/product/detail

### Parameter

| parameter           | type          | required | description             |
| -------------- |:-------------:| ----:| :-----------------|
| product_ids    | array  |  yes   | product id array  |

Note：A maximum of 10 product_ids can be passed at a time to obtain ten product information

### Request parameter example

    {
        "product_ids":[101686926,101457615]
    }

### Response

    Tour package(product_lint is tour):
    {
        "code": 0,
        "msg": "success",
        "data": {
            "base": {
                "product_id": 101457615,
                "product_id_old": "130",
                "product_line": "tour",
                "name": "7-Day Grand Canyon, Antelope Canyon, Las Vegas, Los Angeles, San Francisco Small Group Tour**Super Value****6-10 Pax**<br />\n** Mercedes Benz Sprinter**",
                //product image url
                "image_url": "https://tffimg.tff.bz/5a/40/b35/35a/215d5809cbddb4af44bd47.jpg",
                "advertised_price": 755,
                "currency": "USD",
                "duration": 7,
                //dutation type: day,hour,minute
                "duration_type": "day",
                //stock status: 0 soldout, 1 normal.
                "stock_status": 1,
                "max_child_age": 11,
                //advance booking days limit
                "min_days_before_departure": 0,
                //order minimum number of guests
                "min_guest_number": 1,
                "show_ownexpense": 0,
                "visa_passport": 0,
                //whether to provide departure pick-up service
                "is_pickup": 2,
                //whether to provide arrival pick-up service
                "is_dropoff": 2,
                "hotel_pickup": 0,
                "departure_city": [
                    {
                        "departure_city_id": 1,
                        "departure_city_name": "Los Angeles"
                    }
                ],
                "return_city": [
                    {
                        "return_city_id": 1,
                        "return_city_name": "Los Angeles"
                    }
                ],
                "region_chinese_name": "美国",
                "sub_region_chinese_name": "美西",
                "region": "us",
                "sub_region": "west"
            },
            "info": {
                "brief_description": "• See the neon lights of Las Vegas's world-famous resorts&nbsp;<br />\n• Experience the Grand Canyon from 720 feet in the air on the Skywalk&nbsp;<br />\n• Discover breathtaking sandstone formations in Antelope Canyon<br />\n• Enjoy the picture-perfect 17 Mile Drive along the coast of Monterey <br />\n• Take photos of the Golden Gate Bridge, Chinatown and more in San Francisco<br />\n• Visit Yosemite National Park and see waterfalls, lakes and giant redwoods<br />\n&nbsp;",
                "full_description": "• See the neon lights of Las Vegas's world-famous resorts&nbsp;<br />\n• Experience the Grand Canyon from 720 feet in the air on the Skywalk&nbsp;<br />\n• Discover breathtaking sandstone formations in Antelope Canyon<br />\n• Enjoy the picture-perfect 17 Mile Drive along the coast of Monterey <br />\n• Take photos of the Golden Gate Bridge, Chinatown and more in San Francisco<br />\n• Visit Yosemite National Park and see waterfalls, lakes and giant redwoods<br />\n&nbsp;",
                "airport_transfer_info": "<strong>LAX pick-up: </strong><br />\n*LAX Terminal Meeting Spots<br />\nTom Bradley Int'l Terminal(Terminal B)&nbsp;- The Coffee Bean &amp; Tea Leaf)<br />\nTerminal 1 - Baggage Claim#1 Hudson News<br />\nTerminal 2 - Baggage Claim#2<br />\nTerminal 3 - Baggage Claim#A<br />\nTerminal 4 - Starbucks<br />\nTerminal 5 - Baggage Claim#3<br />\nTerminal 6 - Information and ATM<br />\nTerminal 7/8 - Baggage Claim#1<br />\n<br />\n*LAX Pick-up Time and Schedule<br />\n- We offer one complimentary airport transfer from LAX to your hotel for each reservation. We offer complimentary transfers for:<br />\n- Free airport transfers operate between 9:00 AM -11:00 PM (Bus leaving time)<br />\nBus schedule: Every 2 hour we have the transfer bus pick passengers up at airport (9:00am, 11:10am, 1:00pm, 3:00pm, 5:00pm, 7:00pm, 9:00pm, 11:00pm).<br />\n- If you arrive early, please meet your guides and wait at the meeting point for the next bus. The guide will be wearing a yellow uniform, holding a small yellow flag or an iPad with the local provider's icon.<br />\n- If your flight should become delayed or change for any reason, we will not be held responsible for your airport transfers. If you should arrive after the complimentary airport transfer times indicated, you may also be subject to a late arrival transfer fee or be required to self-transfer to the hotel. If you are delayed and arrive after our normal hours, please contact the emergency number listed on your e-ticket for assistance.<br />\n<br />\n<strong>Airport drop-off: </strong><br />\n*Drop-off in Los Angeles:<br />\n- The tour normally returns to Los Angeles between 6:30 PM - 7:00 PM, but there may be a 30-60 minute delay caused by some special circumstances, such as bad weather condition, traffic jam, etc.<br />\n- We offer the complimentary airport drop-off service, guests who wish to fly out of LAX on the same day must please book a U.S. domestic flight after 9:30 PM and international flight after 10:30 PM&nbsp;before 2/15/2020, please book your departure flight after 9:00pm for U.S domestic flights or after 10:00pm for International flights from 2/15/2020.&nbsp;<br />\n<br />\n*Drop-off in Las Vegas: <strong>(</strong><b>Please call us or make a comment to confirm the order of itinerary if you want to leave tour from Las Vegas. We will check whether it is OK. We can't guarantee that any departure date will end in Las Vegas, please refer to the final confirmation.</b><strong>)</strong><br />\n- For customers departing from Las Vegas, you will forego the tour to the Outlets without any refund, however you will visit the Ethel M Chocolate Factory and Botanical Cactus Garden in the morning. Then we will transfer you to MGM hotel, and you can take taxi or bus to Mccarran International Airport at your own expense (Taxis: about $10.00; Time: about 10 minutes). Please book your departure flight after 2:00pm from McCarran International Airport.&nbsp;(Booking from 1/21/2020 and departure dates from 2/15/2020: we will offer complimentary McCarran International Airport and MGM hotel drop-off service)<br />\n<br />\n<strong>*Please provide your flight info at least 3 days prior to your departure date.</strong>",
                "notice": "",
                "includes": "<LI>Airport Transfers</LI>\r\n<LI>6-Night Hotel Accommodations</LI>\r\n<LI>Transportation in air-conditioned deluxe tour coach</LI>\r\n<LI>Professional tour guide</LI>",
                "excludes": "<LI>All personal expenses</LI>                          \r\n<LI>Service Fee for tour guide (min. $10.00/day per person)</LI>\r\n<li>Airport Pick-up Service Fee for Driver (min. $10.00/person/way)</li>\r\n<LI>Service Fee for Los Angeles Night Tour ($5.00/person)</LI>\r\n<LI>Admissions and optional tours</li>",
                "package_special_note": "<ul>\n\t<li><strong>Cancellation Policy:</strong><br />\n\tAs US west tours are likely to be sold out, we will reserve bus seats once you make reservation. If you would like to cancel your order after confirmation, please check refund policy as following:<br />\n\t* Cancellation made within:<br />\n\t* 16 and More Days Prior to Departure Date: 100% of total purchase amount can be refunded<br />\n\t* 11 - 15 Days Prior to Departure Date: 80% of total purchase amount can be refunded<br />\n\t* 7 - 10 Days Prior to Departure Date: 50% of total purchase amount can be refunded<br />\n\t* 0 - 6 Days Prior to Departure Date: Non-refundable<br />\n\t* Apply to the following situations:<br />\n\t- Cancel the order<br />\n\t- Decrease the number of guests<br />\n\t- Change to other tours<br />\n\t- Change the departure date</li>\n\t<li><strong>Amendment Policy:</strong><br />\n\tAs US west tours are very popular, we will reserve bus seats once you make reservation. If you would like to make any change for your reservation, please check amendment policy as following:<br />\n\tAmendment made within:<br />\n\t* 7 and More Days Prior to Departure Date: $30.00 service fee per change;<br />\n\t* 0 - 6 Days Prior to Departure Date: No Amendment will be accepted;<br />\n\t* Apply to the following situations:<br />\n\t- Change identity information: name, age, etc.<br />\n\t- Change optional tour or available package hotel</li>\n\t<li><strong>Please note that order of day-to-day itinerary is adjustable depending on tour start day.</strong></li>\n\t<li>Prices may vary due to the season and are subject to the final confirmation made by tour guide when on tour.</li>\n\t<li><strong>Gift Pack for Tours4Fun guests</strong><br />\n\tAll passengers in this tour lodging in Circus Circus Hotel will receive a $100-value Super Gift Pack each!<br />\n\t★2 Hot Entertainments at World’s Largest Indoor Theme Park in Circus Circus Hotel, $30 value!<br />\n\t★2 Normal Entertainments at World’s Largest Indoor Theme Park in Circus Circus Hotel, $20 value!<br />\n\t★Famous show by World’s Largest Permanent Circus in Circus Circus Hotel, $10 value!<br />\n\t★Discounts for a variety of restaurants and shops within the hotel, $20 + value!<br />\n\t★Free WIFI and Kettle using in Circus Circus Hotel, $20 value!<br />\n\t(The special offers listed above are subject to the final confirmation made by the tour guide.)<br />\n\tOptional Buffet lunch is only for the Las Vegas visit. The restaurant address is 4300 E. Sunset Rd., C-1, Henderson, NV 89014.</li>\n\t<li>To make your travel more convenient, we suggest you book your tour one month prior to the departure date during the holiday season (New Year/Christmas).</li>\n\t<li>Due to the popularity of these tours during our busy season, the overnight hotels may be fully booked. We will choose the hotels which offer similar standards of service as an alternative.</li>\n\t<li>On the day you visit Grand Canyon or Antelope Canyon, if you choose not to visit these two attractions, you will need to pay $30.00/person for free explore fee.</li>\n\t<li>Las Vegas Tours do not permit travelers under 18, unaccompanied by a co-traveler 21 or older, to join. Travelers aged 18-21 who are unaccompanied by a co-traveler 21 or older can join the tour, however, they cannot gamble in Las Vegas.</li>\n\t<li>Due to the Department of Homeland Security's regulations of Hoover Dam, all bus tours are limited to carry-on luggage such as backpacks and duffle bags. All carry-on items must fit in the over head compartment. Luggage cannot be stored in the compartments under the bus. Any other travel luggage needs to be left at your hotel.</li>\n\t<li>During the busy season (especially in July and August), the listed advanced hotels may be sold out due to the large number of guests and limited rooms. We strongly recommend you book your tour as early as you can. In case there are no more rooms available for these advanced hotels, you can upgrade your Los Angeles hotel to a better quality hotel, with additional fees.</li>\n\t<li>We strongly recommend that you contact the airline and our local tour provider to confirm your flight arrival timing, and request to arrange for a pick-up before your departure.</li>\n\t<li>According to the legal requirements of the destination, smoking is prohibited on the bus during the tour. This also applies to hotel rooms. Violations are fined $300.00 or more (please refer to the hotel rules). Customers are responsible for paying fines and penalties.</li>\n\t<li>Flight information must be provided in order for the airport transfer services to be arranged. At our discretion, if flight information is not provided or provided last minute, your reservation will be noted as a self-transfer and no airport transfer services will be arranged. If you decide to self-transfer to the tour's first night's hotel, please inform us at your earliest convenience. If you opt out of a transfer service, you may reinstate the airport transfer service if notification to reinstate the service is given well in advance of the tour's departure. Urgent requests to reinstate airport transfer services will not be guaranteed. If a flight is delayed, Tours4Fun/ local provider will attempt to arrange a later airport transfer service, however; this later service is not guaranteed. If an airport transfer service is not available and cannot be provided, all guests are responsible for self-transferring to the tour's first night's hotel.</li>\n\t<li>Guests are welcome to opt of the 17 Miles tour and ending their tour in San Francisco, if they wish to do so.</li>\n\t<li>San Francisco Public Transportation: If the hotels used on this tour are near the Fremont/Union City region, clients may ask the hotel for a taxi service to the nearest Bart/train station (around USD 15). Clients may then use the Bart/train system's transfer services to arrive at downtown San Francisco.</li>\n\t<li>San Francisco Taxi Service: Transportation from the Fremont/Union City region to downtown San Francisco takes about 40 minutes - 1 hour. Taxi fares may vary.</li>\n</ul>\n",
                "price_special_note": "*Price for Single Occupancy applies when one person stays in one standard hotel room.<br />\n*Price for Double/Triple/Quadruple Occupancy applies when two/three/four people stay in one standard hotel room respectively.<br />\n*Triple/Quadruple price does not guarantee a third/fourth bed in the room since each room is equipped with 2 beds. Please check the availability at the time of check-in.<br />\n*Maximum room capacity: 4 people including adult and child/infant.",
                "eticket_special_note": "Airport pick-up and drop-off tips for driver will be excluded from the tour price from each guest. Please pay this amount directly to the driver at completion of each transfer. \r\n\r\n**If your flight should be delayed or changed for any reason, we will not be held responsible for your airport transfers. If you should arrive after the complimentary airport transfer times indicated, you may also be subject to a late arrival transfer fee or be required to self-transfer to the hotel. If you are delayed and arrive after our normal office hours, please contact the emergency number listed on your e-ticket for assistance.**\r\n \r\nPlease e-mail or call us for a price quote if you:\r\n\r\n    * Arrive outside of the complimentary airport transfer time frames.\r\n    * Have flight delays, requiring last minute additional late night/delayed airport transfers.\r\n    * Request more than one airport transfer per order. \r\n\r\nWe strongly recommend that you book your flight arrivals within the time frames which are noted and departure flight times after the times indicated.\r\n\r\nAll optional tours that include a service fee must be paid for ( in cash only), before joining the tour.\r\n\r\nYou can call Tours4Fun to acquire the tour guide's contact number and reconfirm your tour the day before tour departure date.\r\n\r\nAccording to the legal requirements of the destination, smoking is prohibited on the bus during the tour. This also applies to hotel rooms. Violations are fined $300.00 or more (please refer to the hotel rules). Customers are responsible for paying fines and penalties. \r\n\r\nTour arrangements/order of itinerary is subject to amendment if deemed necessary by your Local Provider. Any failure to perform, delay, liability or damage shall be excused and Tours4Fun/local provider shall not be held responsible for the consequences of acts of god, labor disputes, civil commotions, fire, traffic conditions, weather conditions, theft, unavoidable accidents, war, acts of state or agencies thereof or any other circumstance/emergency beyond the control of Tours4Fun/local provider. Tours4Fun/local provider shall not be liable should it be required to change an itinerary, a departure date, hotel accommodation or other services necessary for the safety and continuation of any tour or passenger or due to unforeseen circumstances beyond the control of Tours4Fun/local provider. The tour guide/local provider will do their best to provide and maintain their standard of service if the above circumstances/emergencies were to occur. Tours4Fun will do their best to accommodate your needs and address your concerns by speaking with the tour guide/local provider but the tour guide/local provider will make the final decision on any and all requests.\r\n\r\nDuring your trip, please respect your fellow travelers as well as the tour guide and bus driver. At the discretion of the tour guide/driver, travelers who inhibit the tour from going forward and/or are deemed disruptive/destructive will be asked to leave the tour group.\r\n\r\nTours4Fun/local provider reserves the right to modify or change any published rate where changes or modifications have been made and are required by any entities beyond Tours4Fun's/local provider's ownership or control.\r\n\r\nFlight information must be provided in order for the airport transfer services to be arranged. At our discretion, if flight information is not provided or provided last minute, your reservation will be noted as a self-transfer and no airport transfer services will be arranged. If you decide to self transfer to the tour's first night's hotel, please inform us at your earliest convenience. If you opt out of a transfer service, you may reinstate the airport transfer service if notification to reinstate the service is given well in advance of the tour's departure. Urgent requests to reinstate airport transfer services will not be guaranteed. If a flight is delayed, Tours4Fun/local provider will attempt to arrange a later airport transfer service, however; this later service is not guaranteed. If an airport transfer service is not available and cannot be provided, all guests are responsible for self-transferring to the tour's first night's hotel.\r\n\r\nIn order to protect your own property, please bring any valuable items with you at any time. Please do not leave any valuable items on the bus/hotel/attraction/restaurant etc. Tours4Fun, local operators, drivers and tour guides will not take any responsibility for any theft or loss at any location.",
                "tips": "",
                "seo": {
                    "title": "",
                    "description": "",
                    "keywords": ""
                },
                "additional_promotion": "",
                "credential": "",
                "change_notice": "",
                "auto_confirm": "",
                "travel_notice": "",
                "product_tips": ""
            },
            //service language
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
            //itinerary info
            "itinerary": [
                {
                    "itinerary_no": 1,
                    "itinerary_title": "",
                    "itinerary_days_info": [
                        {
                            "itinerary_id": 234,
                            "day_no": 1,
                            "mileage": 0,
                            "tips": "<LI>We strongly recommend that you book your flight arrivals within the time frames suggested and departure flight times after the times indicated.</LI>",
                            "excess_value_recommendation": "",
                            "summary": "Your fun-filled tour through the best sites and cities on the West Coast begins when your airplane lands at Los Angeles airport (LAX). You will be greeted by your friendly tour guide at the airport. They will guide you to your hotel and assist you with the check-in if needed. The hotel check-in time is 3:00 PM. \n\n<strong> Los Angeles Night Tour (Free light meal + 1 bottle of water per person)</strong>\nFor customers whose international flights arriving before 2:00pm or domestic flights arriving before 3:00pm, we recommend you to join the Los Angeles Night Tour!\nDuring this 3 hours tour, you will visit the centre of Los Angeles city. We will stop in Walt Disney Concert Hall and The Broad. Then visit the Los Angeles Lakers home \"Staples Center\" (exterior). At last head to financial district, visit Los Angeles Public Library(exterior) and climb to the famous OUE Skyspace (additional admission), experience the unique Skyslide. \n\nWe will pass by: Los Angeles City Hall, Grand Park, Dorothy Chandler Pavilion, The Museum of Contemporary Art.\n\n*The Night Tour is not available on all Sundays.\n\nDeparture Time and Location of Los Angeles Night Tour:\n17:30pm: La Quinta Inn & Suites Pomona, 3200 W Temple Ave, Pomona, CA 91768\n17:45pm: Best Western Plus Executive Inn, Rowland Heights, 18880 Gale Ave, Rowland Heights, CA 91748\n18:15pm: Quality Inn Rosemead, 9488 Valley Blvd, Rosemead, CA 91770\n18:30pm: Holiday Inn El Monte, 9920 Valley Blvd, El Monte, CA 91731\n\n**If your flight should be delayed or change for any reason, we will not be held responsible for your airport transfers. If you should arrive after the complimentary airport transfer times indicated, you may also be subject to a late arrival transfer fee or be required to self-transfer to the hotel. If you are delayed and arrive after our normal hours, please contact the emergency number listed on your e-ticket for assistance.**\n \n Please e-mail or call us for a transportation price quote for customers that:\n* Arrive outside of the complimentary airport transfer time frames.\n* Have flight delays requiring last minute additional late night/delayed airport transfers.\n* Request more than one airport transfer per order. \nWe strongly recommend that you book your flight arrivals within the time frames suggested and departure flight times after the times indicated.",
                            "title": "Los Angeles",
                            "attraction": [
                                {
                                    "attraction_id": 682509,
                                    "parent_id": 466,
                                    "duration": "0.0",
                                    "duration_type": "day",
                                    "is_optional": 0,
                                    "city_description": {
                                        "name": "LAX Airport",
                                        "pinyin": null,
                                        "alias": null,
                                        "seo_url": "lax-airport",
                                        "description": "Los Angeles International Airport, often shorted to LAX, is the third busiest airport in the United States and the sixth in the world accommodating an average of 63.7 million passengers per year. It has been an air field since 1928 when it was called Mines Field. LAX offered commercial airline service in 1946 and the current terminal structure was built in 1961. It provides 680 daily flights to 96 American cities and 910 weekly nonstop flights to 59 cities in 30 countries on 60 commercial airlines.",
                                        "transportation": null,
                                        "languages": null,
                                        "feature_foods": null,
                                        "religious_culture": null,
                                        "tips": null,
                                        "operate_tips": null,
                                        "tour_city_id": 466,
                                        "language_id": 1,
                                        "parent_tour_city_id": 1,
                                        "image": "TourCity201405271401213175_5384d0f7b4a7c.jpg",
                                        "latitude": 33.9425,
                                        "longitude": -118.4080556
                                    }
                                },
                                {
                                    "attraction_id": 682512,
                                    "parent_id": 58119,
                                    "duration": "0.0",
                                    "duration_type": "day",
                                    "is_optional": 0,
                                    "city_description": {
                                        "name": "Oue Skyspace",
                                        "pinyin": "O",
                                        "alias": "",
                                        "seo_url": "oue-skyspace",
                                        "description": "",
                                        "transportation": null,
                                        "languages": null,
                                        "feature_foods": null,
                                        "religious_culture": null,
                                        "tips": null,
                                        "operate_tips": null,
                                        "tour_city_id": 58119,
                                        "language_id": 1,
                                        "parent_tour_city_id": 1,
                                        "image": "https://cdn.tff.bz/f2/windtour/1c/4d/losspace.jpg",
                                        "latitude": 34.0511007,
                                        "longitude": -118.2565766
                                    }
                                }
                            ],
                            "hotel": [
                                {
                                    "hotel_id": 506233,
                                    "name": "La Quinta Pomona",
                                    "description": null,
                                    "image_url": "",
                                    "parent_id": null,
                                    "is_deleted": 0,
                                    "language_id": 1,
                                    "hotel_info": []
                                },
                                {
                                    "hotel_id": 561304,
                                    "name": "Vanllee Hotel & Suites LVGEM",
                                    "description": null,
                                    "image_url": "",
                                    "parent_id": null,
                                    "is_deleted": 0,
                                    "language_id": 1,
                                    "hotel_info": []
                                }
                            ],
                            "city": [
                                {
                                    "city_id": 422646,
                                    "parent_id": 1,
                                    "city_description": {
                                        "name": "Los Angeles",
                                        "pinyin": "L",
                                        "alias": "LA;LAX",
                                        "seo_url": "los-angeles",
                                        "description": "This Southern California city is known for sunshine, beaches and the film industry, Los Angeles, often called \"The City of Angels\" is the second most populated city in the United States behind New York City and is known for the diversity of its residents. It was founded in 1781, obtained by Mexico from 1821-1848 and was incorporated in 1850. Some of the city's most popular tourist attractions are The Hollywood Sign, Capitol Records Building, TCL Chinese Theatre, Hollywood Walk of Fame, Griffith Observatory, The Getty Center, Dolby Theatre, Los Angeles Memorial Coliseum, Hollywood Bowl and Staples Center. <br>Explore the world by joining a <a href=\"http://www.tours4fun.com/tours/las-vegas/\">Las Vegas Tour</a>, <a href=\"http://www.tours4fun.com/tours/chicago/\">Chicago Tour</a>, <a href=\"http://www.tours4fun.com/tours/yosemite-national-park/\">Yosemite Tour</a>, <a href=\"http://www.tours4fun.com/tours/yellowstone-national-park/\">Yellowstone Tour</a>, and much, much more.",
                                        "transportation": null,
                                        "languages": null,
                                        "feature_foods": null,
                                        "religious_culture": null,
                                        "tips": null,
                                        "operate_tips": null,
                                        "tour_city_id": 1,
                                        "language_id": 1,
                                        "image": "TourCity201703081489012276_58c086341f10d.jpg",
                                        "latitude": 34.0521019,
                                        "longitude": -118.2436196
                                    }
                                }
                            ],
                            "transport": [],
                            "meal": [],
                            "ownexpense": [
                                {
                                    "ownexpense_id": 316842,
                                    "parent_id": 131022,
                                    "tour_city_ownexpense_id": 12792,
                                    "price": " $33.00",
                                    "tips": "Optional tour, available if you join Los Angeles Night Tour",
                                    "ownexpense_description": {
                                        "name": "OUE Skyspace+Skyslide",
                                        "description": "",
                                        "tour_city_ownexpense_id": 12792,
                                        "language_id": 1,
                                        "tour_city_id": 1
                                    }
                                }
                            ]
                        },
                        {
                            "itinerary_id": 237,
                            "day_no": 2,
                            "mileage": 0,
                            "tips": "",
                            "excess_value_recommendation": "",
                            "summary": "The tour group will depart Los Angeles driving through the scenic Mojave Desert to arrive in Las Vegas - The Pearl in the Desert. You'll have the night to yourself. You may join our Las Vegas Night Tour or see one of the many award-winning shows the city has to offer!",
                            "title": "Los Angeles - Las Vegas ",
                            "attraction": [
                                {
                                    "attraction_id": 471012,
                                    "parent_id": 10121,
                                    "duration": "0.0",
                                    "duration_type": "day",
                                    "is_optional": 0,
                                    "city_description": {
                                        "name": "Las Vegas Strip",
                                        "pinyin": "L",
                                        "alias": "Sin City;vegas",
                                        "seo_url": "las-vegas-strip",
                                        "description": "Thousands visit Vegas every year just to spend time at the Strip. In just four miles, the Strip contains over 30 casinos, numerous hotels and a 24-hour party scene. You can enjoy a drink at Caesar's Palace while you take a gamble, eat your heart out at Mirage's Cravings buffet, shop until you drop at the Grand Canal Shoppes at Venetian Resort & Casino or sit back to a Broadway show or musical. Plenty of magicians and comedians perform daily to impress and entertain you. Come join the fun at the Strip!",
                                        "transportation": null,
                                        "languages": null,
                                        "feature_foods": null,
                                        "religious_culture": null,
                                        "tips": null,
                                        "operate_tips": null,
                                        "tour_city_id": 10121,
                                        "language_id": 1,
                                        "parent_tour_city_id": 3,
                                        "image": "TourCity201706181497806361_5946b619224b5.jpg",
                                        "latitude": 36.115131,
                                        "longitude": -115.1727314
                                    }
                                }
                            ],
                            "hotel": [
                                {
                                    "hotel_id": 485851,
                                    "name": "Circus Circus Hotel",
                                    "description": null,
                                    "image_url": "",
                                    "parent_id": null,
                                    "is_deleted": 0,
                                    "language_id": 1,
                                    "hotel_info": []
                                }
                            ],
                            "city": [
                                {
                                    "city_id": 296151,
                                    "parent_id": 1,
                                    "city_description": {
                                        "name": "Los Angeles",
                                        "pinyin": "L",
                                        "alias": "LA;LAX",
                                        "seo_url": "los-angeles",
                                        "description": "This Southern California city is known for sunshine, beaches and the film industry, Los Angeles, often called \"The City of Angels\" is the second most populated city in the United States behind New York City and is known for the diversity of its residents. It was founded in 1781, obtained by Mexico from 1821-1848 and was incorporated in 1850. Some of the city's most popular tourist attractions are The Hollywood Sign, Capitol Records Building, TCL Chinese Theatre, Hollywood Walk of Fame, Griffith Observatory, The Getty Center, Dolby Theatre, Los Angeles Memorial Coliseum, Hollywood Bowl and Staples Center. <br>Explore the world by joining a <a href=\"http://www.tours4fun.com/tours/las-vegas/\">Las Vegas Tour</a>, <a href=\"http://www.tours4fun.com/tours/chicago/\">Chicago Tour</a>, <a href=\"http://www.tours4fun.com/tours/yosemite-national-park/\">Yosemite Tour</a>, <a href=\"http://www.tours4fun.com/tours/yellowstone-national-park/\">Yellowstone Tour</a>, and much, much more.",
                                        "transportation": null,
                                        "languages": null,
                                        "feature_foods": null,
                                        "religious_culture": null,
                                        "tips": null,
                                        "operate_tips": null,
                                        "tour_city_id": 1,
                                        "language_id": 1,
                                        "image": "TourCity201703081489012276_58c086341f10d.jpg",
                                        "latitude": 34.0521019,
                                        "longitude": -118.2436196
                                    }
                                },
                                {
                                    "city_id": 296154,
                                    "parent_id": 3,
                                    "city_description": {
                                        "name": "Las Vegas",
                                        "pinyin": "L",
                                        "alias": "Vegas;sin city",
                                        "seo_url": "las-vegas",
                                        "description": "Las Vegas' nickname is \"Sin City\" and you'll find out why when you visit; the Strip is full of casinos, night clubs, indulgent pools and replicas of some of the world's most popular tourist attractions. Looking for <a href=\"http://www.tours4fun.com/tours/las-vegas/things-to-do/\">Things to Do & Activities in Las Vegas</a>? The city is located in the heart of the Mojave Desert. During the day you can bask by the pool, take a <a href=\"http://www.tours4fun.com/tours/las-vegas/helicopter/\">helicopter tour</a>, enjoy an all-you-can-eat buffet or view magnificent <a href=\"http://www.tours4fun.com/tours/las-vegas/shows-and-events/\">shows in Las Vegas</a> such as Cirque du Soleil, David Copperfield, or the classic Jersey Boys show! Dine at many five-star restaurants with world-renowned chefs and then check out the nightlife at Mirage or any of the hotels on the Strip. Don't forget to watch the spectacular water show at the Bellagio or visit the aquarium at Mandalay Bay. Throughout your stay, remember \"what happens in Vegas, stays in Vegas,\" so no worries!  <br> You may also interested in <a href=\"http://www.tours4fun.com/tours/grand-canyon/\">Grand Canyon Tours</a>, <a href=\"http://www.tours4fun.com/tours/hoover-dam/\">Hoover Dam Tours</a> , <a href=\"http://www.tours4fun.com/tours/los-angeles/\">Los Angeles Tours</a>.",
                                        "transportation": null,
                                        "languages": null,
                                        "feature_foods": null,
                                        "religious_culture": null,
                                        "tips": null,
                                        "operate_tips": null,
                                        "tour_city_id": 3,
                                        "language_id": 1,
                                        "image": "TourCity201706181497805071_5946b10f4ddc8.jpg",
                                        "latitude": 36.1146003,
                                        "longitude": -115.1728458
                                    }
                                }
                            ],
                            "transport": [],
                            "meal": [],
                            "ownexpense": [
                                {
                                    "ownexpense_id": 301353,
                                    "parent_id": 132732,
                                    "tour_city_ownexpense_id": 5079,
                                    "price": "$40.00/Person",
                                    "tips": "",
                                    "ownexpense_description": {
                                        "name": "Las Vegas High Roller",
                                        "description": "",
                                        "tour_city_ownexpense_id": 5079,
                                        "language_id": 1,
                                        "tour_city_id": 3
                                    }
                                },
                                {
                                    "ownexpense_id": 301356,
                                    "parent_id": 132735,
                                    "tour_city_ownexpense_id": 14253,
                                    "price": "$45.00/Person",
                                    "tips": "",
                                    "ownexpense_description": {
                                        "name": "Las Vegas In-depth Tour(3 hours)",
                                        "description": "",
                                        "tour_city_ownexpense_id": 14253,
                                        "language_id": 1,
                                        "tour_city_id": 3
                                    }
                                }
                            ]
                        }
                    ]
                }
            ],
            "media": {
                "image_url": "https://tffimg.tff.bz/5a/40/b35/35a/215d5809cbddb4af44bd47.jpg",
                "thumbnail_url": "https://tffimg.tff.bz/5a/40/b35/35a/215d5809cbddb4af44bd47.jpg",
                "map_image_url": "",
                "video_url": "",
                "extra": [
                    "https://tffimg.tff.bz/ea/38/7a1/153/d106667d5263d1269b813a.jpg",
                    "https://tffimg.tff.bz/d3/1d/767/656/002423d116b284e40e8bae.jpg",
                    "https://tffimg.tff.bz/17/46/74f/389/92515d26e247253dad2cd1.jpg",
                    "https://tffimg.tff.bz/f9/6c/9c8/cc3/9a9e86240df4d6dccbfca6.jpg",
                    "https://tffimg.tff.bz/7c/a6/8be/58e/bd24a4aa7a13132c5c99f0.jpg"
                ]
            },
            //guest required information
            "passengerForm": {
                "lastname_en": {
                    "name": "lastname_en",
                    "label": "Last Name",
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
                    "label": "First Name",
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
                    "label": "Passport Number",
                    "type": "text",
                    "min": "",
                    "max": "",
                    "options": [],
                    "placeholder": ""
                },
                "passport_expire": {
                    "name": "passport_expire",
                    "label": "Passport Expire Date",
                    "type": "date",
                    "min": "",
                    "max": "",
                    "options": [],
                    "placeholder": ""
                },
                "mobile": {
                    "name": "mobile",
                    "label": "Mobile",
                    "type": "phone",
                    "min": "",
                    "max": "",
                    "options": [],
                    "placeholder": ""
                },
                "email": {
                    "name": "email",
                    "label": "Email",
                    "type": "text",
                    "min": "",
                    "max": "",
                    "options": [],
                    "placeholder": ""
                },
                "gender": {
                    "name": "gender",
                    "label": "Gender",
                    "type": "radio",
                    "options": [
                        "unknown",
                        "male",
                        "female"
                    ],
                    "min": "",
                    "max": "",
                    "placeholder": ""
                },
                "dob": {
                    "name": "dob",
                    "label": "Birthday",
                    "type": "date",
                    "min": "",
                    "max": "",
                    "options": [],
                    "placeholder": ""
                },
                "nation": {
                    "name": "nation",
                    "label": "Country",
                    "type": "text",
                    "min": "",
                    "max": "",
                    "options": [],
                    "placeholder": ""
                },
                "weight": {
                    "name": "weight",
                    "label": "Body Weight",
                    "type": "number",
                    "min": "",
                    "max": "",
                    "options": [],
                    "placeholder": ""
                },
                "weight_unit": {
                    "name": "weight_unit",
                    "label": "Weight Unit",
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


