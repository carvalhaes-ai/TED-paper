## story_PMUL3171
* I m looking for a _hotel_type_ to stay in that s _pricerange_ and on the _area_ side.
    - slot{"hotel_status": "available"}
    - inform_hotel: _hotel_name_ is on the _area_ side and _pricerange_ .   <!-- predicted: inform_restaurant_request_restaurant: I have found _number_ _food_type_ restaurants on the _area_ side. There are _number_ _pricerange_ and _number_ _pricerange_ . Did you have a price range in mind? -->
* That sounds good, but can you tell me if it includes free wifi?
    - slot{"hotel_status": "unique"}
    - Yes it does would you like me to book that for you?
* Yes for _number_ person, staring _weekday_ starting _number_ days.
    - slot{"hotel_status": "booked"}
    - Okay, you re all set! Your reference number is _reference_ .
* No, that is all. Cheer.
    - bye_general: Thank you for contacting us. Have a wonderful visit.   <!-- predicted: bye_general_greet_general_welcome_general: Thank you for using our service. Call us anytime. Take care. Goodbye. -->


## story_PMUL3731
* Please find a _pricerange_ price range _food_type_ restaurant.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_recommend_restaurant: Sure, there are _number_ in the centre of town. I prefer _hotel_name_ , located at _number_ Bridge Street, City Centre.   <!-- predicted: inform_restaurant_request_restaurant_select_restaurant: there are _number_ in town. did you have a certain part of town you want to dine in? i have some in the centre and _area_ . -->
* I want to book a table for _number_ people at _time_ on _weekday_ will you do that ?
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant: Booking was successful. The table will be reserved for _number_ minutes.Reference number is _reference_ .   <!-- predicted: book_booking_restaurant_reqmore_general: No problem! I ve booked you a reservation at _restaurant_name_ for _weekday_ at _time_ for _number_ people. The reference number is _reference_ . Is there anything else? -->
* Thanks for the booking. I would like to sightsee a bit. Do you have any _attraction_type_ attractions in town?
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: I have _number_ _attraction_type_ attractions. _number_ are in the centre, with _number_ in the _area_ and _area_ . Are you interested in information about _number_ of them in a certain area?   <!-- predicted: nooffer_restaurant_request_restaurant: I am sorry I can find no place that serves that in the centre area. Would you like to try another area or food type? -->
* Please pick the _number_ that you think is the best out of them, and then provide me the phone number and address for it
    - inform_attraction: _attraction_name_ is located at _hotel_name_ passenger cruisers, jubilee house and the phone number is _number_ .   <!-- predicted: recommend_attraction: _attraction_name_ _attraction_type_ centre	_number_ cb58bs	jesus lane	free_attraction_name_ _attraction_type_ centre	_number_ cb23pq	market square	_number_ pounds_attraction_name_ _attraction_type_ centre	_number_ cb23nz	market street	free_attraction_name_ _attraction_type_ centre	_number_ cb21qy	little saint mary s lane	free_attraction_name_ _attraction_type_ centre	_number_ cb21tt	trinity lane	free -->
* Great, can you help me book a taxi?
    - Where are you leaving from and going to and what time are you wanting to go?
* Anything that arrives by _time_ . I want to commute from the Riverboat to the restaurant.
    - slot{"taxi_status": "booked"}
    - inform_taxi_reqmore_general: You are booked for a _color_ _cartype_ with the contact number _number_ . Is there anything else?   <!-- predicted: inform_taxi: Ok, your taxi is booked. The car will be a _color_ _cartype_ and the contact number is _number_ . -->
* That is everything that I need.
    - greet_general: Enjoy your stay and if you need anything in the future feel free to contact us.   <!-- predicted: bye_general_welcome_general: Glad I could be of service. Goodbye. -->
* I sure will, thanks. Goodbye
    - greet_general: thanks again have a great day   <!-- predicted: bye_general_reqmore_general_welcome_general: Okay, great. I m glad I could help. Don t hesitate to contact us again if you need additional assistance. Goodbye. -->


## story_PMUL2933
* I m looking for a _hotel_type_ to stay at that has free wifi and a _number_ star rating. Do you have any suggestions?
    - slot{"hotel_status": "available"}
    - inform_hotel: _hotel_name_ is in the _area_ with wifi and a _number_ star rating.   <!-- predicted: inform_hotel_request_hotel: There are _number_ matching your request. Do you have any preferences such as area, price, parking, or internet? -->
* That sounds great but I was hoping to stay in the _area_ . Do you have anything else?
    - slot{"hotel_status": "available"}
    - inform_hotel_select_hotel: Yes I have _number_ guesthouses in the _area_ . _number_ in the _pricerange_ price range and another in the _pricerange_ price range. Do you have a preference?   <!-- predicted: inform_hotel_reqmore_general: There are _number_ moderately priced hotels and guest houses in _hotel_name_ . Do you have any more requirements to help narrow it down? -->
* No, I ll take your recommendation. Can you give me a phone number and postcode? Oh, and how _pricerange_ is it?
    - slot{"hotel_status": "unique"}
    - _hotel_name_ is cheaply priced and is absolutely gorgeous. The phone number is _number_ and the postcode is cb22ha. Would you like me to book a room?
* Not now. But can you tell me something about concert halls in the _area_ ?
    - slot{"attraction_status": "NA"}
    - nooffer_attraction: Sure thing, there are none.   <!-- predicted: inform_attraction_nooffer_attraction: I am sorry, there actually are not any _attraction_type_ attractions in the centre. There is _number_ located in the _area_ , though. -->
* How about a _attraction_name_ in the same area?
    - slot{"attraction_status": "available"}
    - inform_attraction_select_attraction: My favorite paid _attraction_name_ to visit is _hotel_name_ _attraction_name_ and my favorite free _attraction_name_ to visit _hotel_name_ Hall. Do either of those peek your interest?   <!-- predicted: inform_attraction_reqmore_general: There are _number_ colleges in town centre. _hotel_name_ and Caius _attraction_name_ is on trinity street with free entrance. Do you want more information on any others? -->
* I love free. Can you give me the address of _hotel_name_ Hall?
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: Sure, the address is herschel road. Is there something else I can help you with?   <!-- predicted: inform_attraction: Yes, I can. The address is university of _hotel_name_ , _location_ , postcode cb23dz. -->
* No, that will be all. Thank you!
    - You re welcome, have a great day.


## story_MUL1855
* Yes I am looking for a train leaving _hotel_name_ on _weekday_ .
    - slot{"train_status": "available"}
    - greet_general_inform_train: I can help you with that. The first _number_ departs at _time_ and the last trains runs at _time_ . How many tickets would you like?   <!-- predicted: inform_train_request_train: There are _number_ trains traveling on _weekday_ . Where will you be departing from and where is your destination? -->
* Also the destination is _location_ and leaves after _time_ .
    - slot{"train_status": "unique"}
    - There is a train leaving at _time_ that fits your criteria. Would you like me to book it for you?
* Yes, please, just _number_ ticket.
    - slot{"train_status": "booked"}
    - greet_general_offerbooked_train_reqmore_general: Great! Your booking was successful. The fee will be _number_ _reference_ payable at the station. Would you like the reference number?   <!-- predicted: offerbooked_train_reqmore_general: Booking was successful for _reference_ , the total fee is _number_ _reference_ payable at the station. Your reference number is _reference_ . Do you need further assistance? -->
* Yes, please. I am also looking for attractions in the _area_ part of town.
    - slot{"attraction_status": "available"}
    - inform_attraction_inform_train_recommend_attraction: Your reference number is _reference_ . There are several attractions in the _area_ . May I suggest the _restaurant_name_ _attraction_type_ ?   <!-- predicted: greet_general_inform_attraction_select_attraction: I am happy to help. There are several types of places to go in the _area_ . Parks, theatre, _attraction_type_ , _attraction_name_ , _attraction_type_ . What sounds good to you? -->
* Sure. Could I get their phone number please?
    - Sure! The phone number is _number_
* That s all I needed today. Thank you for your help.
    - bye_general_greet_general_welcome_general: You re quite welcome. Just let us know if you find yourself needing more information. Have a great day!   <!-- predicted: bye_general_welcome_general: My pleasure. Please call again if you need more help. I am happy to be of service. -->


## story_SNG0007
* I want to book a taxi going to _attraction_name_ departing from _restaurant_name_ please.
    - slot{"taxi_status": "available"}
    - When would you like to arrive by?
* Doesn t matter, but I need to leave after _time_
    - slot{"taxi_status": "booked"}
    - I was able to book you a _color_ _cartype_ for _time_ , the contact number is _number_ .
* Thank you very much.
    - Will there be anything else today, or have I answered all your questions?
* That s all I needed, thanks so much for your help.
    - bye_general: It was my pleasure. Have a great night.   <!-- predicted: greet_general: My pleasure. Thank you for contacting _hotel_name_ TownInfo centre. Have a nice visit. -->


## story_PMUL4343
* Can you get me information on a restaurant called mahal of _hotel_name_ ?
    - slot{"restaurant_status": "available"}
    - inform_restaurant_recommend_restaurant: Sure it is a _pricerange_ _food_type_ restaurant in the town centre. I hear it has great food.   <!-- predicted: inform_restaurant_reqmore_general: _restaurant_name_ in the _area_ is at _hotel_name_ Leisure _attraction_type_ Clifton Way. _restaurant_name_ is at _number_ Saint Andrews Street. Do you need additional information? -->
* Do you think they would be able to make reservations for a party of _number_ ?
    - slot{"restaurant_status": "available"}
    - greet_general_request_booking_restaurant: I can help you with that. When would you like to make the reservation for?   <!-- predicted: inform_booking_restaurant_inform_restaurant_reqmore_general: They serve _food_type_ food. Do you need any other information, or help making a booking? -->
* _time_ for a table of _number_ for the restaurant stated above. Thank you!
    - slot{"restaurant_status": "available"}
    - request_booking_restaurant: What day would you like that reservation for?   <!-- predicted: select_restaurant: The restaurants are _restaurant_name_ , _restaurant_name_ and _restaurant_name_ . -->
* Oh, _weekday_ please. And if you could give me a reference number, that d be great.
    - slot{"restaurant_status": "booked"}
    - I have successfully booked your table! Your reference number is _reference_ . Anything else I can help you with today?
* I would also like the address of a _attraction_name_ in the centre of town
    - slot{"attraction_status": "available"}
    - Primavera is a _attraction_name_ in the center of town. Their address is _number_ king s parade. What else can I help with?
* Oh, I made a mistake. I really need that table for _time_ , not _time_ . Can you change it, do you thing?
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_greet_general: Yes, I already changed it for you. Your new reference number is _reference_ .   <!-- predicted: reqmore_general: Yes nice place. Did you need any info on it ? -->
* Thank you for making that change. Can you recommend a _attraction_name_ in the centre?
    - We have _number_ museums in the Centre, my personal favorite is the _attraction_name_ at Unit su43, Grande arcade, Saint Andrews street. There is no entrance fee there.
* That sounds great. I will plan to stop at that _attraction_name_ .
    - slot{"attraction_status": "available"}
    - greet_general_reqmore_general: Great! Have a great time. Is there anything else you need?   <!-- predicted: inform_attraction_reqmore_general: _attraction_name_ is in the centre area on jesus lane. It is free to visit. Would you like more information? -->
* No that is it. Thank you.
    - You are welcome. Enjoy your time in _hotel_name_ . Goodbye.


## story_PMUL2205
* Can you help me find a moderately priced _food_type_ restaurant?
    - slot{"restaurant_status": "available"}
    - inform_restaurant_select_restaurant: _restaurant_name_ is available, would you like to try that?   <!-- predicted: inform_hotel_reqmore_general: There are _number_ moderately priced hotels and guest houses in _hotel_name_ . Do you have any more requirements to help narrow it down? -->
* That sounds good. Where is it located? I was looking for somewhere in the _area_ .
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_booking_restaurant: _restaurant_name_ is located in the _area_ section of town! What day and time can I make your reservations for?   <!-- predicted: inform_restaurant_reqmore_general: _restaurant_name_ in the _area_ is at _hotel_name_ Leisure _attraction_type_ Clifton Way. _restaurant_name_ is at _number_ Saint Andrews Street. Do you need additional information? -->
* I think I would just like to get the postcode, address and phone number to contact them myself.
    - greet_general_inform_restaurant: Sure! The postcode is cb58jj, address is _number_ Newmarket Road Fen Ditton and the phone is _number_ . Enjoy your dining experience!   <!-- predicted: inform_restaurant_reqmore_general: Of course. _restaurant_name_ is located at Thompsons Lane Fen Ditton. The post code is cb58aq. The phone number is _number_ . Do you need any further assistance? -->
* Thanks you, Im think of doing something after I eat, are there any good _attraction_type_ places in the _area_ area?
    - slot{"attraction_status": "available"}
    - inform_attraction_request_attraction: Yes, there are quite a few good places. Was there a certain type of _attraction_type_ you were interested in?   <!-- predicted: greet_general_inform_attraction_select_attraction: I am happy to help. There are several types of places to go in the _area_ . Parks, theatre, _attraction_type_ , _attraction_name_ , _attraction_type_ . What sounds good to you? -->
* The attraction type is _attraction_type_ , in the _area_ area, please.
    - inform_attraction: I found _number_ attractions that match your request _attraction_name_ and _attraction_name_ .   <!-- predicted: nooffer_attraction_reqmore_general: I m sorry, there are no _attraction_type_ attractions listed in the centre of _hotel_name_ . Would you like to search for something different? -->
* Cherry Hinton Hall sounds good can I get the phone number, address, and postcode.
    - slot{"attraction_status": "available"}
    - inform_attraction: The _attraction_name_ is on Cherry Hinton Road. Their phone number is _number_ and the postcode is cb18dw.   <!-- predicted: inform_attraction_inform_train_reqmore_general: The _attraction_name_ s address is Market Street, postcode cb23nz. There are many trains arriving in Stansted Airport by _time_ . Would you like to narrow your search further? -->
* Thank you. I will also need a taxi between the _number_ places that leaves the restaurant by _time_ .
    - slot{"taxi_status": "booked"}
    - inform_taxi_reqmore_general: Booking completed!Booked car type _color_ _cartype_ Contact number _number_ Can I help you with anything else?   <!-- predicted: inform_taxi: Okay! Your taxi is a _color_ _color_ _cartype_ . Contact number _number_ -->
* Nope, that s it. Thank you. Bye now
    - bye_general: Good bye, enjoy your stay in _hotel_name_ .   <!-- predicted: bye_general_welcome_general: You are quite welcome. Thank you for using our services! -->


## story_SNG1126
* Hello, I am trying to find an attraction in the _area_ part of town. Can you help me?
    - slot{"attraction_status": "available"}
    - inform_attraction_select_attraction: Sure, there are many colleges and museums in the _area_ , there is also some _attraction_type_ . Do you have a preference on any of these?   <!-- predicted: inform_attraction_reqmore_general: I have _number_ _attraction_type_ attractions. _number_ are in the centre, with _number_ in the _area_ and _area_ . Are you interested in information about _number_ of them in a certain area? -->
* Not really. Could you give me the postcode for _number_ of the museums?
    - slot{"attraction_status": "available"}
    - recommend_attraction_reqmore_general: The _number_ I recommend is the People s Portraits Exhibition at Girton _attraction_name_ . It s free to get in. Their postcode is cb3ojg. Is there any other information I can provide?   <!-- predicted: inform_attraction: The _attraction_name_ is a _attraction_name_ . Entry is free, and their postcode is cb15dh. -->
* Thank you. That s all I need today. Goodbye.
    - bye_general_greet_general: Thank you for calling. Goodbye.   <!-- predicted: bye_general_welcome_general: You re welcome. Thanks for contacting the _hotel_name_ TownInfo Centre and have a great day! -->


## story_MUL1811
* I m looking for something to do in town. Are there any interesting attraction in the _area_ part of town?
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: Yes, there are several places I see a _attraction_type_ , a _attraction_type_ , and _number_ swimming pools. Would _number_ of these work for you?   <!-- predicted: inform_attraction_recommend_attraction: _attraction_name_ is my favorite place on the _area_ side! I don t have any information on the entrance fee, but their phone is _number_ . -->
* Ooh, a pool would be fun. Can you give me their contact info?
    - slot{"attraction_status": "available"}
    - Great! _attraction_name_ is located at jedburgh court, kings hedges Postcode is cb42xh and their phone is _number_ . Is there anything else I can help you with?
* I need a train from bishops shortford.
    - slot{"train_status": "available"}
    - request_train: I can help you with that. Can you confirm the destination you are traveling to?   <!-- predicted: inform_train_request_train: There are _number_ trains leaving _hotel_name_ after that time. What is your destination and day of travel? -->
* I need a train to arrive by _time_ on _weekday_ going to _hotel_name_ .
    - slot{"train_status": "available"}
    - You ve got _number_ choices from very early morning to somewhat late evening. What would you prefer?
* Pick the closest _number_ to the arrival time. I need it for _number_ people and I need the reference number.
    - slot{"train_status": "booked"}
    - Great. Your reference number is _reference_ and you are fully booked.
* Thanks for all your help. That s all for me. Bye!
    - Glad to help. Have a wonderful day!


## story_PMUL2503
* I m places to go, can you point me in the right direction?
    - request_attraction: what type of attraction do you want?   <!-- predicted: request_restaurant: Yes, could you tell me what type of food you would like and the part of town you prefer? -->
* I want to go to a _attraction_name_ .
    - slot{"attraction_status": "available"}
    - inform_attraction_request_attraction: There are several what area are you wanting to go to?   <!-- predicted: inform_hotel_request_hotel: There are _number_ available that match what you re looking for, do you have any preference for what area you want to stay in? -->
* Any place in town is fine for me. Do you have any recommendations?
    - slot{"attraction_status": "available"}
    - recommend_attraction: I suggest the byard art _attraction_name_ located in the _area_ .   <!-- predicted: inform_hotel_request_hotel: There are _number_ hotels which are _number_ stars, _number_ in the _area_ and _number_ in the centre. Is there an area which you prefer? -->
* That sounds great. What is the entrance fee?
    - Their admission is free. Is there anything else you need to know?
* Yes please. I need an _pricerange_ guesthouse that has free parking please.
    - slot{"hotel_status": "NA"}
    - nooffer_hotel_reqmore_general: I m sorry I don t have anything in that category. Can we check something else?   <!-- predicted: inform_hotel_nooffer_hotel: There s nothing fitting those criteria. I do have _number_ moderately priced guesthouses with free parking. Or would you like to change something else? -->
* Do you have a guesthouse in the _pricerange_ price range with free parking?
    - slot{"hotel_status": "available"}
    - inform_hotel_select_hotel: I have several in the _area_ closer to the _attraction_name_ , and some in the _area_ . Do you have a preference?   <!-- predicted: inform_hotel: Actually, _hotel_name_ doesn t meet your requirements. But I do have other options that are moderately priced, such as _hotel_name_ , Arbury Lodge Guesthouse, and _hotel_name_ . -->
* No I don t. Can you pick the best _number_ please. I need a room for _number_ and _number_ nights starting from _weekday_ .
    - slot{"hotel_status": "booked"}
    - book_booking_hotel_inform_hotel_reqmore_general: You are booked at the _hotel_name_ at _number_ Chesterton Road. Reference number is _reference_ . Can I help with anything else today?   <!-- predicted: book_booking_hotel_reqmore_general: Your rooms at the _hotel_name_ have been booked. Your reference number is _reference_ . Is there anything further I can assist you with today? -->
* That ll be all thanks so much!
    - You re welcome, hope you have a great time! Goodbye.


## story_MUL2423
* Yes, I am looking for a place to dine. I would prefer the city centre and am looking for _food_type_ food.
    - slot{"restaurant_status": "NA"}
    - I am sorry I can find no place that serves that in the centre area. Would you like to try another area or food type?
* Ok. Is there an _food_type_ restaurant in the centre area.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_restaurant: There are _number_ _food_type_ restaurants in that area, what is your price-range?   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* I don t have a price range. Can you just recommend _number_ of the _number_ restaurants and tell me the postcode and the price range
    - inform_restaurant_recommend_restaurant_reqmore_general: I apologize. There were _number_ differrent _food_type_ restaurants in the centre of town. My recommendation would be _restaurant_name_ . They are _pricerange_ . Their postcode is cb12lf. Anything else I can help with?   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* What is the post code for the _pricerange_ restaurant _restaurant_name_ ?
    - slot{"restaurant_status": "available"}
    - inform_restaurant_reqmore_general: The postcode is cb12lf. Is there anything else I can do for you?   <!-- predicted: inform_restaurant: There is _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _restaurant_name_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _area_ _food_type_ , _food_type_ , _food_type_ , and _food_type_ food available in the centre. -->
* I d like some information on theatre s in town.
    - slot{"attraction_status": "available"}
    - inform_attraction_request_attraction: There are _number_ theatres in town, are you looking for something in the center of town as well?   <!-- predicted: greet_general_inform_attraction_select_attraction: I am happy to help. There are several types of places to go in the _area_ . Parks, theatre, _attraction_type_ , _attraction_name_ , _attraction_type_ . What sounds good to you? -->
* Yes, and i would also need a taxi to leave by _time_ .
    - slot{"attraction_status": "available"}
    - slot{"taxi_status": "available"}
    - request_taxi: I would love to help! Where would you be coming from or going?   <!-- predicted: inform_train_request_train: You ve got _number_ choices from very early morning to somewhat late evening. What would you prefer? -->
* I need the taxi to pick me up at the theatre. But I suppose we should figure out exactly which theatre that is. You mentioned _number_ in the centre?
    - inform_attraction: Actually there are _number_ theatres in the centre. _reference_ , _hotel_name_ Arts, Mumford, and the _hotel_name_ corn exchange.   <!-- predicted: request_taxi: Ok, so you d like a taxi from the restaurant to the _attraction_type_ ? Could you please let me know your desired departure and arrival times? -->
* How about _hotel_name_ Arts?
    - slot{"attraction_status": "available"}
    - slot{"taxi_status": "available"}
    - request_taxi: Ok. And what is your destination?   <!-- predicted: inform_attraction: _attraction_name_ is an architectural attraction in the center of town. They are located on Trinity Lane, in postcode cb21tt. -->
* I would be going from _hotel_name_ Arts to _restaurant_name_ , leaving by _time_ . Can you please provide the postcode and phone number of _hotel_name_ Arts as well?
    - slot{"taxi_status": "available"}
    - inform_attraction: The postcode is cb23pj and the phone is _number_ .   <!-- predicted: inform_attraction_reqmore_general: sheep s green and lammas land _attraction_type_ fen causeway number is _number_ and postcode is cb22ad. wandlebury country _attraction_type_ number is _number_ postcode is cb223ae. Do you need anything else? -->
* Great, I just need the taxi and I will be all set.
    - slot{"taxi_status": "booked"}
    - Sure. I have booked a _color_ _cartype_ to pick you up. The contact number is _number_ .
* OK, thank you for your help.
    - reqmore_general: Don t hesitate to contact the help desk again if you require assistance.   <!-- predicted: bye_general_welcome_general: Glad I could be of help, thank you. -->
* Thanks, that s all I need, goodbye!
    - It was a pleasure to serve you. Have a nice day. Goodbye.


## story_MUL1478
* I m looking for an _pricerange_ place to eat in the centre.
    - slot{"restaurant_status": "available"}
    - There are a lot of great, _pricerange_ restaurant in the centre. What type of food would you prefer?
* It doesn t matter to me which type of food they serve. What would you recommend for a person eating alone?
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_inform_restaurant: How about _restaurant_name_ , serving _food_type_ ? It s at Midsummer Common. Would you like to book a table?   <!-- predicted: inform_booking_restaurant_recommend_restaurant: I would recommend _restaurant_name_ . It is an _pricerange_ restaurant in the center. Would you like to book a reservation? -->
* Yes please, can you book a table for _number_ on _weekday_ at _time_ ?
    - slot{"restaurant_status": "booked"}
    - You are booked! Your table will be reserved for fifteen minutes and your reference number is _reference_ .
* Thanks! I also need a train to peterborough and I need it to arrive by 10am and arrive on _weekday_ to _hotel_name_
    - slot{"train_status": "available"}
    - request_train: I am sorry, would you like to go to or from _hotel_name_ ?   <!-- predicted: inform_train_request_train: I have _number_ trains available. Is there a certain time you would like to travel? -->
* I will be departing from _hotel_name_ and traveling to Peterborough.
    - slot{"train_status": "unique"}
    - offerbook_train_request_train: Sure, I can book you on _reference_ arriving by _time_ . Will this be a reservation for _number_ also?   <!-- predicted: inform_train_offerbook_train: Ah, it appears that the earliest train, _reference_ , leaves at _time_ , but it does arrive by _time_ . If that is okay, I could book that for you. -->
* Yes, this will be for _number_ person only. Thank you very much
    - slot{"train_status": "booked"}
    - offerbooked_train: Yes your booking was successful and your reference number is _reference_ .   <!-- predicted: book_booking_hotel_reqmore_general: Great, your Booking was successful, your reference number is _reference_ . for _weekday_ _number_ nights for _number_ . Anything else I can help you with today? -->
* Okay thank you very much.
    - welcome_general: Okay Glad I could help you.   <!-- predicted: reqmore_general_welcome_general: No problem at all! Is there anything more I can help you with today? -->


## story_PMUL3127
* Are there any trains leaving out of _hotel_name_ on _weekday_ ?
    - slot{"train_status": "available"}
    - Yes. Where would you be going to?
* Stevenage. I need to arrive by _time_
    - slot{"train_status": "unique"}
    - _reference_ will arrive at _time_ . Would you like to book?
* Yes please, I need tickets for _number_ please.
    - slot{"train_status": "booked"}
    - Your booking was successful. The total fee is _number_ _reference_ payable at the station. Your reference number is _reference_ . Can I help you with anything else?
* Yes I need information on _attraction_name_ .
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: The _attraction_name_ is in the centre. Admission is free, and the phone number is _number_ . Can I provide you with any other information?   <!-- predicted: inform_attraction: _hotel_name_ _attraction_name_ of Technology is located on the _area_ side at The Old Pumping Station, Cheddars Lane. Their phone number is _number_ and they charge an entrance fee of _number_ pounds. -->
* Can you tell me the address as well?
    - inform_attraction: The address is Free _attraction_name_ Lane and phone is _number_   <!-- predicted: recommend_attraction: _attraction_name_ _attraction_type_ centre	_number_ cb58bs	jesus lane	free_attraction_name_ _attraction_type_ centre	_number_ cb23pq	market square	_number_ pounds_attraction_name_ _attraction_type_ centre	_number_ cb23nz	market street	free_attraction_name_ _attraction_type_ centre	_number_ cb21qy	little saint mary s lane	free_attraction_name_ _attraction_type_ centre	_number_ cb21tt	trinity lane	free -->


## story_SNG01683
* I am looking for a restaurant. The restaurant should serve _food_type_ food and should be in the _pricerange_ price range
    - slot{"restaurant_status": "available"}
    - _restaurant_name_ is a great restaurant that fulfills your wishes. It is located at _number_ Regent Street City Centre.
* Awesome. Can I also get the area, post code, and phone number?
    - slot{"restaurant_status": "available"}
    - inform_restaurant: Yes, _restaurant_name_ is located in the centre and the postcode is cb21dp.   <!-- predicted: inform_restaurant_reqmore_general: Certainly, the phone number for the _restaurant_name_ restaurant is _number_ and the address is _number_ Regent Street City Centre. May I help you with anything else today? -->
* Thanks, I just need the phone number so I can call them.
    - inform_restaurant: The phone number is _number_ . Is there anything else I can help you with?   <!-- predicted: inform_hotel_reqmore_general: Absolutely! _hotel_name_ is a _number_ star _hotel_type_ and their phone number is _number_ _number_ . Is there anything else I can help you with? -->
* Thanks, that s all. Good bye.
    - bye_general: Enjoy yourself, and let me know if you need anything else.   <!-- predicted: greet_general: My pleasure. Thank you for contacting _hotel_name_ TownInfo centre. Have a nice visit. -->


## story_PMUL3275
* I am coming to visit and will be in the centre area. I would like an attraction to visit.
    - slot{"attraction_status": "available"}
    - inform_attraction: sure, how about _hotel_name_ contemporary art?   <!-- predicted: inform_attraction_request_attraction: I have _number_ results for colleges. To help narrow it down, are you looking for _number_ in a particular area? Some are free and some have entrance fees. -->
* Sounds interesting! What is the address?
    - slot{"attraction_status": "available"}
    - Located at _number_ trinity street	.
* now I need a place to eat in the centre
    - slot{"restaurant_status": "available"}
    - We have many restaurants available. What type of food are you interested in?
* I am really craving _food_type_ if you have something in that area.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_restaurant: Yes, _number_ _food_type_ places are in that area. Any preference on price range?   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* Yeah, I want an _pricerange_ place.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_recommend_restaurant: There are _number_ . Could I recommend Tang _food_type_ .   <!-- predicted: inform_hotel_request_hotel: I have about _number_ different places. Do you have a preference on the area of town? -->
* I will need a reservation for _number_ at _time_ on _weekday_ .
    - slot{"restaurant_status": "booked"}
    - Your table for _number_ is reserved for _weekday_ at _time_ . Your reference number is _reference_ .
* That is all I need. Bye, thanks.
    - bye_general: Ok. Take care. Goodbye   <!-- predicted: bye_general_greet_general_welcome_general: Thank you so much for calling! Enjoy your trip! Goodbye! -->


## story_PMUL3264
* i need a place to stay
    - request_hotel: Let s find you a great place in the city. Do you have a preference on what area in town?   <!-- predicted: inform_hotel_request_hotel: Most of the hotels in town offer free parking. Is there a certain area you d like to stay in, or do you have a price range in mind? -->
* I don t. I will need a guesthouse with at least _number_ star. It should also have free wifi.
    - slot{"hotel_status": "available"}
    - inform_hotel_request_hotel: There are _number_ entries that match your request. To help narrow results down, do you have a pricerange?   <!-- predicted: inform_train_request_train: There are lots to choose from under that criteria. What day would you like to travel on? -->
* No, just choose _number_ please. I ll need to book it for _weekday_ , _number_ nights, and _number_ people.
    - slot{"hotel_status": "booked"}
    - book_booking_hotel_reqmore_general: I have booked you at the _hotel_name_ Guesthouse. Reference number _reference_ . Can I be of any further help?   <!-- predicted: book_booking_hotel: Okay, your booking was successful! We have you booked at the _hotel_name_ . Your reference number is _reference_ . -->
* Thank you. The next thing I need is a train from _hotel_name_ to stevenage.
    - slot{"train_status": "available"}
    - What day will you be traveling?
* I will be traveling on and need to leave after _time_ .
    - slot{"train_status": "available"}
    - request_train: Okay, can you please tell me the day?   <!-- predicted: inform_train_reqmore_general: I apologize! There are _number_ trains leaving near your requested time. _number_ at _time_ and _number_ at _time_ . Will _number_ of those work? -->
* _weekday_ please ?
    - slot{"train_status": "unique"}
    - inform_train_offerbook_train: Train _reference_ meets your criteria. Would you like me to book it for you?   <!-- predicted: nobook_booking_restaurant_request_booking_restaurant: Unfortunately, I am unable to book for that day time. Would you like to book your table for another day or time? -->
* Yes, please. There are _number_ of us who need on it.
    - slot{"train_status": "booked"}
    - You are booked as requested, the total fee is _number_ _reference_ payable at the station, your Reference number is _reference_ . Anything Else today?
* That is all. Thank you
    - bye_general: Thank you for contacting us, enjoy your trip!   <!-- predicted: bye_general_welcome_general: You re welcome! Thank you for contacting us, have a great day! -->


## story_MUL2368
* Hello! I am looking to book reservations at _restaurant_name_ .
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_booking_restaurant: Ah yes, I have that right here. It s an _pricerange_ _food_type_ restaurant in the _area_ end. How many people would you like to reserve a table for, and what day time?   <!-- predicted: inform_restaurant_request_restaurant: There are a total of _number_ _pricerange_ restaurants located in town. Is there a specific area you are going to be in? -->
* That s all the info I needed. Thanks.
    - reqmore_general: Are you sure you don t need help with anything else?   <!-- predicted: bye_general_welcome_general: You are quite welcome. Thank you for using our services! -->
* I d also like to know if there s a swimmingpool in the _area_ .
    - slot{"attraction_status": "available"}
    - inform_attraction: Abbey pool and astroturf pitch is in the _area_ . Would you like the address and postal code?   <!-- predicted: inform_restaurant: The top _number_ places serving _food_type_ cuisine are _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Would you like more options? -->
* Just the address would be fine. Thanks.
    - Sure thing. The address is pool way, whitehill road, off newmarket road. Can I help with anything else?
* Yes, I need a taxi from the pool to the restaurant, I would like to leave the pool place at _time_
    - slot{"taxi_status": "booked"}
    - inform_taxi_reqmore_general: Booking complete! A _color_ _cartype_ will collect you at Abbey Pool and Astroturf Pitch at _time_ , heading to _restaurant_name_ . The driver s contact number is _number_ . Will that be all today?   <!-- predicted: inform_taxi: Okay! Your taxi is a _color_ _color_ _cartype_ . Contact number _number_ -->
* Yes, you have helped tremendously. Thank you.
    - bye_general_welcome_general: Thank you, have a nice day. Bye.   <!-- predicted: reqmore_general: Not a problem! Do you need anything else? -->


## story_PMUL4958
* I need a _hotel_type_ that is in the _pricerange_ price range. That has a _number_ star rating.
    - slot{"hotel_status": "unique"}
    - _hotel_name_ is a nice _hotel_type_ that I can book for you.
* Can I check if it has free wifi?
    - slot{"hotel_status": "unique"}
    - greet_general_inform_booking_hotel: It sure does! WOuld you like to book a room?   <!-- predicted: inform_booking_hotel_inform_hotel: yes it includes internet. would you like for me to book that for you? -->
* Yes, for _number_ people. _number_ nights, starting from _weekday_
    - slot{"hotel_status": "booked"}
    - Booking was successful. Reference number is _reference_ .
* Thank you. That is all for today. Goodbye
    - bye_general_welcome_general: My pleasure, enjoy your stay.   <!-- predicted: bye_general: Good bye, enjoy your stay in _hotel_name_ . -->


## story_MUL2415
* I want something to entertain me in town. What do you have?
    - slot{"attraction_status": "available"}
    - inform_attraction_request_attraction: I have _number_ venues that meet what you asked. Did you have a certain area you wanted?   <!-- predicted: inform_attraction_reqmore_general: I have _number_ _attraction_type_ attractions. _number_ are in the centre, with _number_ in the _area_ and _area_ . Are you interested in information about _number_ of them in a certain area? -->
* Nothing in particular. Something with high reviews. Can you send me the address of the top choice?
    - slot{"attraction_status": "available"}
    - inform_attraction_recommend_attraction: The _attraction_name_ it is. They re located at _number_ mercers row, mercers row industrial estate.   <!-- predicted: inform_attraction_reqmore_general: Sure thing. The address is pool way, whitehill road, off newmarket road. Can I help with anything else? -->
* Thanks - I am also looking for a _food_type_ restaurant in the city centre.
    - slot{"attraction_status": "available"}
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_restaurant: I ve got _number_ _food_type_ restaurants in that area, is there a price range you want to narrow it down to?   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* I prefer the _pricerange_ price range.
    - slot{"restaurant_status": "unique"}
    - _restaurant_name_ is a very popular restaurant in the _pricerange_ range. Would you like me to book a reservation for you?
* That sounds awesome. Can I get a reservation for _number_ people on _weekday_ at _time_ please?
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_reqmore_general: You are all set! Reference number _reference_ . Anything else I can help you with?   <!-- predicted: book_booking_restaurant: I have successfully booked a table for _number_ on _weekday_ at _time_ for you. The table will be reserved for _number_ minutes and your reference number is _reference_ . -->
* Yes, I need a taxi to get from the fun house to the restaurant by the reservation time, please.
    - slot{"taxi_status": "available"}
    - request_taxi: What time would you like to arrive and leave?   <!-- predicted: inform_taxi: Your taxi is booked. Be expecting a _color_ _cartype_ . Please call _number_ should you need to reach them. -->
* I need to arrive by _time_ at the restaurant.
    - slot{"taxi_status": "booked"}
    - inform_taxi_reqmore_general: Your booking is set, look for a _color_ _cartype_ , the driver can be reached at _number_ , anything else that I can assist with?   <!-- predicted: inform_taxi: Okay! Your taxi is a _color_ _color_ _cartype_ . Contact number _number_ -->
* Um... that should be everything.
    - bye_general_greet_general_welcome_general: Thank you for using our service. Have a great evening. Goodbye.   <!-- predicted: bye_general: Enjoy your time in _hotel_name_ . Goodbye. -->


## story_MUL0306
* I am looking for a train departing from _hotel_name_ leaving on _weekday_ .
    - slot{"train_status": "unique"}
    - inform_train_offerbook_train: I have trains departing long kings cross to _hotel_name_ on _weekday_ every _number_ hours starting at _time_ , would you like to make a reservation?   <!-- predicted: request_taxi: I d be happy to help you with a taxi, what is your destination departure and what time would you like to arrive leave? -->
* I need _number_ that leaves after _time_ for Bishops Stortford
    - slot{"train_status": "available"}
    - inform_train_select_train: How about the _reference_ ? It leaves at _time_ and arrives at _time_ in Bishops Stortford.   <!-- predicted: inform_train: I would recommend _reference_ which leaves Bishops Stortford at _time_ and arrives in _hotel_name_ by _number_ . -->
* And this train leaves from _hotel_name_ ? If so could you please book it for _number_ people and give me the reference number?
    - slot{"train_status": "booked"}
    - inform_train_offerbooked_train: Yes, it leaves from _hotel_name_ . I have booked this for you, and your reference number is _reference_ .   <!-- predicted: offerbooked_train_reqmore_general: Sure, the train is actually number _reference_ and your reference number is _reference_ . The price will be _number_ _reference_ payable at the station. Is there anything else today? -->
* I am also looking for a place to eat around the centre area that serves _restaurant_name_ style food.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_recommend_restaurant: I found _number_ places, would you like to try The Cow _attraction_name_ _restaurant_name_ ?   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* Yes, please book a reservation for _number_ people.
    - reqmore_general: Is there anything else I can do for you?   <!-- predicted: book_booking_restaurant_reqmore_general: I ve made the reservation and the reference number is _reference_ . What else can I help you with? -->
* Can I get the reference number for that.
    - request_booking_restaurant: What day and time would you like the reservation for?   <!-- predicted: reqmore_general: Yes nice place. Did you need any info on it ? -->
* Also _weekday_ at _time_ .
    - slot{"restaurant_status": "NA"}
    - I could not book the restaurant for _number_ people at _time_ . Would you like to try a different time?
* Can you get a table for _number_ at _time_ ?
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant: I was able to book that for you. Your reference number is _reference_ . Your table will be reserved for _number_ minutes.   <!-- predicted: book_booking_hotel_reqmore_general: That did the trick, your booking was successful and your reference number is _reference_ . Is there anything else you need help with today? -->
* Ok great thank you for all of your help!
    - greet_general_welcome_general: You re very welcome, I hope you enjoy your meal!   <!-- predicted: inform_attraction_reqmore_general: No problem. They can be reached at _number_ . Is there anything else I can help with? -->


## story_PMUL0506
* I need a train leaving after _time_ and heading the _location_ .
    - slot{"train_status": "available"}
    - OK, and what day would you like to leave?
* I d like to leave on _weekday_ .
    - slot{"train_status": "NA"}
    - nooffer_train: There are no trains leaving at that time.   <!-- predicted: nooffer_train_reqmore_general: I just checked again. Unfortunately there are no trains available. Any other arrangements I can make for you? -->
* I am going to have to ask you to check again, after _time_ please.
    - request_train: Where are you leaving from?   <!-- predicted: inform_train: Train _reference_ departing from _hotel_name_ at _time_ and arriving at stansted airport at _time_ will be the best option for you. -->
* i m leaving from _hotel_name_
    - slot{"train_status": "unique"}
    - I have _number_ leaving at _time_ . Would you like me to make a booking for you?
* Yes. Please book for _number_ people.
    - slot{"train_status": "booked"}
    - inform_train: I was able to book you on trainTR1765. The Reference number is _reference_ .   <!-- predicted: offerbooked_train_reqmore_general: Booking was successful for _reference_ , the total fee is _number_ _reference_ payable at the station. Your reference number is _reference_ . Do you need further assistance? -->
* Thanks. I am also looking to find a restaurant in the _area_ .
    - slot{"restaurant_status": "available"}
    - request_restaurant: Any type of food you would like?   <!-- predicted: inform_restaurant: The top _number_ places serving _food_type_ cuisine are _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Would you like more options? -->
* I am open to suggestions. I just would prefer it to be in the _pricerange_ range.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_select_restaurant: I have the _restaurant_name_ which serves _food_type_ . I also have _restaurant_name_ that serves _food_type_ food. Which would you prefer?   <!-- predicted: inform_restaurant_recommend_restaurant: We have _number_ _pricerange_ _food_type_ restaurants in the centre. May I suggest the _restaurant_name_ ? -->
* I think _restaurant_name_ sounds good. Can you book a table for the same group of people at _time_ on the same day?
    - slot{"restaurant_status": "booked"}
    - Your table is booked, ref _reference_ . Can I help you with anything else?
* Nope, that s all I needed today. Thanks!
    - welcome_general: You re welcome, have a great day!   <!-- predicted: bye_general_greet_general_welcome_general: Thank you so much for calling! Enjoy your trip! Goodbye! -->


## story_PMUL1772
* I m looking for a train to _hotel_name_ .
    - slot{"train_status": "available"}
    - request_train: What day will you be traveling?   <!-- predicted: inform_train_request_train: There are _number_ trains departing for Stevenage, where would you be departing from? -->
* I would like to leave on _weekday_ .
    - slot{"train_status": "available"}
    - inform_train_request_train: Okay I have several. What time are you leaving, and how many tickets would you like?   <!-- predicted: inform_train: _reference_ will arrive in _hotel_name_ _weekday_ by _time_ , it will depart peterborough at _time_ . Does this suit your needs? -->
* I am leaving Thurtsday at 2pm and need _number_ tickets
    - slot{"train_status": "available"}
    - inform_train_reqmore_general: I have the _reference_ that leaves at _time_ pm. Would that work for you?   <!-- predicted: request_train: Which station are you traveling to, and on which day? -->
* Actually, I never told you where I was leaving from. I need the train to depart from _location_ .
    - slot{"train_status": "unique"}
    - _reference_ leaves at _time_ . Want to book it?
* yes please, _number_ people. And I d like the reference number please.
    - slot{"train_status": "booked"}
    - Certainly! The total fare is _number_ Pounds, payable at the station, and the reference number is _reference_ . Can I help you with anything else?
* Yes, I m also looking for a place to stay in the _area_ . I d like a guesthouse if possible.
    - slot{"hotel_status": "available"}
    - recommend_hotel: I can recommend the _hotel_name_ .   <!-- predicted: inform_hotel_request_hotel: I show _number_ hotels in the _area_ , _number_ is _pricerange_ and _number_ is _pricerange_ . I also show _number_ _pricerange_ _number_ star _hotel_type_ in the _area_ . Which area do you prefer? -->
* That sounds great. PLease book for _number_ people for _number_ nights starting on _weekday_ .
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel: I will book that for you now.   <!-- predicted: book_booking_hotel_reqmore_general: You booking if successful, the reference number is _reference_ , can I help with anything else? -->
* Thanks. I would also like the reference number, please.
    - slot{"hotel_status": "booked"}
    - book_booking_hotel: I have made your reservations and your reference numbers is _reference_ .   <!-- predicted: offerbooked_train_reqmore_general: Booking was successful for _reference_ , the total fee is _number_ _reference_ payable at the station. Your reference number is _reference_ . Do you need further assistance? -->
* That will be all, thank you for your help today!
    - bye_general: Thank you, I m glad we were able to help you.   <!-- predicted: greet_general: Great! I hope you enjoy your stay! -->


## story_SNG0983
* Can you help me find a _hotel_type_ called _hotel_name_ ?
    - slot{"hotel_status": "available"}
    - inform_hotel_reqmore_general: Sure. It s at _number_ milton road. Would you like the phone number?   <!-- predicted: inform_hotel: _hotel_name_ is a _pricerange_ guesthouse in the centre area. It has a _number_ star rating and includes parking and wifi. It s located at _number_ warkworth street. Phone number _number_ . -->
* Can you book me a reservation for _number_ people for _number_ nights starting _weekday_ ?
    - slot{"hotel_status": "booked"}
    - book_booking_hotel: Your reservation is all set. Your reference number is _reference_ .   <!-- predicted: book_booking_hotel_inform_hotel_reqmore_general: You are booked at the _hotel_name_ B & B. It is _pricerange_ , with wifi and parking included. Your reference number is _reference_ . Is there anything else? -->
* Thank you very much for your help and have a great day.
    - bye_general_greet_general: Thank you for calling. Goodbye.   <!-- predicted: reqmore_general_welcome_general: You re welcome! Is there anything else you need help with today? -->


## story_MUL1493
* Hello, I m trying to find a train that leaves from _hotel_name_ and arrives here by _time_ today. Can you help me book a ticket?
    - slot{"train_status": "available"}
    - The closest arrival time I can give you is _time_ , is that ok? And how many tickets would you like?
* That s fine. I don t want to book yet. Is the train you found going to Ely and leaving on _weekday_ ?
    - slot{"train_status": "available"}
    - inform_train: Yes i have a train that leaves on that day but that arrives around _time_   <!-- predicted: request_train: Yes, I can. Just to confirm, is your destination _hotel_name_ or another city? -->
* Could I have the departure time for that particular train please?
    - That ll be at _time_ .
* Thank you very much.
    - slot{"train_status": "unique"}
    - offerbook_train_reqmore_general: Is there anything else I can help you with? I can help with booking tickets if you would like.   <!-- predicted: offerbook_train: Okay great. would you like me to book that train ticket for you? -->
* Are there any restaurants that serve _food_type_ food in the _area_ part of town?
    - slot{"restaurant_status": "NA"}
    - Unfortunately, there are no _food_type_ restaurants on the _area_ side. Would you like to try a different type of restaurant or area?
* Try anything with _food_type_ food, that would work as well. I will need the address if you find _number_ , thanks!
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_restaurant: I have found _number_ _food_type_ restaurants on the _area_ side. There are _number_ _pricerange_ and _number_ _pricerange_ . Did you have a price range in mind?   <!-- predicted: inform_restaurant: I found _number_ options for you _restaurant_name_ at Regent Street City Centre, _restaurant_name_ at _number_ Mill Road City Centre, and _restaurant_name_ at _number_ _hotel_name_ Road City Centre -->
* No nothing in particular, could you tell me the address of the first _number_ listed?
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_recommend_restaurant: I would recommend _restaurant_name_ . The address is _number_ Newmarket Road Fen Ditton. Would you like me to book a reservation for you?   <!-- predicted: inform_restaurant: I found _number_ options for you _restaurant_name_ at Regent Street City Centre, _restaurant_name_ at _number_ Mill Road City Centre, and _restaurant_name_ at _number_ _hotel_name_ Road City Centre -->
* No, that is all I needed, thank you.
    - bye_general: I hope you have a great day.   <!-- predicted: bye_general_welcome_general: I m happy we could be of service. Thank you for using the _hotel_name_ TownInfo centre. Goodbye! -->


## story_SNG0500
* I m trying to find a _pricerange_ _food_type_ restaurant to have dinner at tonight. What kind of options are available for me?
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_booking_restaurant: I have _number_ places, how many people and what time?   <!-- predicted: inform_restaurant_request_restaurant: There are a total of _number_ _pricerange_ restaurants located in town. Is there a specific area you are going to be in? -->
* Actually, can you suggest _number_ of them. Can I get their contact info as well?
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_recommend_restaurant: Sure, I would suggest _restaurant_name_ at _number_ Millers Yard City Centre. You can reach them at _number_ . I could reserve it for you.   <!-- predicted: reqmore_general: Yes nice place. Did you need any info on it ? -->
* No, that s ok, I can take it from here. Thank you for all your help.
    - You re welcome! Have a great day. Goodbye.


## story_SNG0782
* Hi! What can you tell me about _number_ -star guesthouses in town?
    - slot{"hotel_status": "available"}
    - There are _number_ matching your request. Do you have any preferences such as area, price, parking, or internet?
* Yes, I would like a guesthouse in the _area_ part of town and it should include wifi.
    - slot{"hotel_status": "unique"}
    - There are _number_ _hotel_name_ is _pricerange_ , located at _number_ roseford road cb22ha and _hotel_name_ is _pricerange_ , located at _number_ mowbray road cb17sr. Shall we book?
* Yes, let s try Rosa s for _number_ nights starting _weekday_ . There will be _number_ of us.
    - slot{"hotel_status": "booked"}
    - You are all set for checking in on _weekday_ . Your reference number is _reference_ . Can I help with anything else?
* That will be all, thank you so much.
    - greet_general: No problem. Glad to help.   <!-- predicted: bye_general_welcome_general: You re welcome, have a great day. Bye! -->


## story_MUL1273
* Hello, I m looking for information on the _hotel_name_ .
    - slot{"hotel_status": "unique"}
    - The alpha-milton guesthouse is in the _area_ area, moderately priced, showing _number_ stars. There is no internet or parking. Should I book this for you?
* Yes, please book _number_ nights at the alpha-milton guesthouse for me. I would like to check in on _weekday_ .
    - slot{"hotel_status": "available"}
    - For how many people?
* Actually, I don t need a reservation. I am looking for a _food_type_ restaurant in the center of town, though.
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_recommend_restaurant: The _restaurant_name_ is good and is located at the Doubletree by Hilton. Can I reserve a table for you?   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* can i get the address, phone number, and price range please?
    - slot{"restaurant_status": "available"}
    - inform_restaurant: No problem. The address is _hotel_name_ Granta Place Mill Lane. The phone number is _number_ . It is in _pricerange_ price range.   <!-- predicted: inform_restaurant_reqmore_general: Certainly, the phone number for the _restaurant_name_ restaurant is _number_ and the address is _number_ Regent Street City Centre. May I help you with anything else today? -->
* Can you book a table for _number_ at _number_ pm tomorrow night?
    - slot{"restaurant_status": "available"}
    - request_booking_restaurant: Sure, just to confirm you need that for _number_ people?   <!-- predicted: recommend_hotel_request_booking_hotel: OK, how about _hotel_name_ ? To book a stay I ll need to know the first day you want to stay, how many days, and how many guests. -->
* Yes please. Can you let me know if the reservation is successful.
    - slot{"restaurant_status": "NA"}
    - nobook_booking_restaurant: I have not been able to book it.   <!-- predicted: inform_hotel: Actually, _hotel_name_ doesn t meet your requirements. But I do have other options that are moderately priced, such as _hotel_name_ , Arbury Lodge Guesthouse, and _hotel_name_ . -->
* Ok, that s ok. I ll take care of it later. Thanks so much. Good day to you. Bye.
    - bye_general: Have a nice day.   <!-- predicted: inform_hotel: Actually, _hotel_name_ doesn t meet your requirements. But I do have other options that are moderately priced, such as _hotel_name_ , Arbury Lodge Guesthouse, and _hotel_name_ . -->


## story_MUL1860
* Hi, I am looking for some _attraction_type_ to go to in the centre of town. Any ideas?
    - slot{"attraction_status": "available"}
    - recommend_attraction: i d like to suggest to you _attraction_name_ entrance there is free   <!-- predicted: inform_attraction_reqmore_general: I have _number_ _attraction_type_ attractions. _number_ are in the centre, with _number_ in the _area_ and _area_ . Are you interested in information about _number_ of them in a certain area? -->
* Great, can I have the address and postcode?
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: Of course. The _attraction_type_ is on Jesus Lane and the postcode is cb58bs. Can I help you with anything else?   <!-- predicted: inform_attraction_inform_train_reqmore_general: The _attraction_name_ s address is Market Street, postcode cb23nz. There are many trains arriving in Stansted Airport by _time_ . Would you like to narrow your search further? -->
* I m also going to need to catch a train into _hotel_name_ for _weekday_ .
    - slot{"train_status": "available"}
    - request_train_select_train: Where will you be departing from and what time would you like to travel on _weekday_ ?   <!-- predicted: request_train: Where will you be departing from and what will be your departing time? -->
* I d like to go from _hotel_name_ to Ely, and I need to be there by _time_ for a wedding I m attending.
    - slot{"train_status": "available"}
    - inform_train: I have a train leaving _hotel_name_ to ely on _weekday_ at _time_ and you ll arrive by _time_ . Will that work for you?   <!-- predicted: inform_train_offerbook_train: I have _number_ trains that will get you to _hotel_name_ by _time_ . _reference_ will get you there at _time_ . Would that work? -->
* Could you please tell me the train ID?
    - inform_train: That would be the _reference_ .   <!-- predicted: greet_general_inform_train: Certainly. The train s ID is _reference_ , and the price for a ticket is _number_ pounds. -->
* That s all. Thanks.
    - reqmore_general_welcome_general: Thank you for contacting us. Is there anything else you will be needing today?   <!-- predicted: welcome_general: welcome anytime you need us -->
* No that is all. Thank you!
    - Thank you! Have a good day. Good bye!


## story_MUL0496
* Hello! I need a train departing _hotel_name_ after _time_ , please.
    - slot{"train_status": "available"}
    - What day would you like to travel?
* I would like to leave on _weekday_ and go to _location_ .
    - slot{"train_status": "available"}
    - I have _number_ trains departing _hotel_name_ on _weekday_ to _location_ . The earliest is leaving at _time_ arriving by _time_ , will this suit you?
* Yes. I d like _number_ tickets on the _time_ train, please. And can I have the reference number?
    - slot{"train_status": "booked"}
    - Booking was successful for _reference_ , the total fee is _number_ _reference_ payable at the station. Your reference number is _reference_ . Do you need further assistance?
* Yes. I would like to know about places to go in the _area_ area of town.
    - slot{"attraction_status": "available"}
    - inform_attraction_request_attraction: Well, there are quite a few museums and colleges you can visit in this area. Do you want to pay an entrance fee?   <!-- predicted: inform_attraction_reqmore_general: I have _number_ _attraction_type_ attractions. _number_ are in the centre, with _number_ in the _area_ and _area_ . Are you interested in information about _number_ of them in a certain area? -->
* I would like to go to a concerthall.
    - slot{"attraction_status": "NA"}
    - nooffer_attraction: I m sorry but I don t have any concert halls in the _area_ part of town.   <!-- predicted: nooffer_restaurant_request_restaurant: I am sorry I can find no place that serves that in the centre area. Would you like to try another area or food type? -->
* I suppose a _attraction_name_ would do as well. Any recommendations for museums _area_ of town?
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: Absolutely! We have _number_ of them. Would you like details on any specific _number_ ?   <!-- predicted: inform_attraction_recommend_attraction: I have _number_ museums. I could suggest the broughton house gallery it has a free entrance fee. -->
* Any of them would be fine. Can you just give me the name, address with postcode and the phone number? Thanks.
    - inform_attraction: Sure thing! I ve picked for you _attraction_name_ _attraction_name_ . Their phone is _number_ and they re located in postcode cb30aq at _number_ high street, fen ditton. Is that everything you need today?   <!-- predicted: inform_attraction_reqmore_general: Certainly! _attraction_name_ is a _attraction_name_ located on the _area_ side of town. Their address is castle street and their phone number is _number_ . Is there anything else? -->
* No, that s all I need. Thank you.
    - bye_general_welcome_general: You re welcome. Have a great day.   <!-- predicted: bye_general: Thank you and enjoy your visit. -->


## story_MUL0352
* I need a train to _hotel_name_ , departing from the Peterborough station.
    - slot{"train_status": "available"}
    - There are a total of _number_ trains traveling from Peterborough to _hotel_name_ . What day would you like to leave?
* I would like to travel on _weekday_ and arrive by _time_ .
    - slot{"train_status": "unique"}
    - I have a train scheduled to depart Peterborough at _time_ and will arrive in _hotel_name_ by _time_ . Would you me like to book this for you?
* Yes, for _number_ people, please.
    - slot{"train_status": "booked"}
    - Okay all booked! The arrival time is actually _time_ and your reference number is _reference_ .
* Thanks! I m also looking for a _food_type_ place located in the centre?
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_restaurant: There are _number_ that match your preference. Do you have a price range? Or do you know the name of the restaurant?   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* I would like a restaurant in the _pricerange_ price range. Can you find _number_ ?
    - slot{"restaurant_status": "available"}
    - There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference?
* _restaurant_name_ sounds delicious, please provide the address.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_booking_restaurant: Absolutely! The address is _number_ _hotel_name_ Road City Centre post code cb21eg. How many people would you like me to make a reservation for?   <!-- predicted: inform_attraction_reqmore_general: Sure thing. The address is pool way, whitehill road, off newmarket road. Can I help with anything else? -->
* No reservation needed at this time. In fact, I have everything I need. Thanks for your help today, I m all set.
    - bye_general: Thank You, have a great day. Goodbye   <!-- predicted: bye_general_welcome_general: My pleasure. Please call again if you need more help. I am happy to be of service. -->


## story_MUL1418
* I need to get train ticket leaving _hotel_name_ after _time_ please.
    - slot{"train_status": "available"}
    - inform_train_request_train: Ok I have a total of _number_ entries that leave after that time. Do you have a specific day or destination you would like to select ?   <!-- predicted: request_train: What day of the week are you traveling and what is your departure station? -->
* I need to go to _location_ on _weekday_ .
    - slot{"train_status": "unique"}
    - offerbook_train: I would recommend train ID _reference_ which leaves _hotel_name_ at _time_ and arrives at _location_ at _time_ .   <!-- predicted: inform_train_offerbook_train: Ah, it appears that the earliest train, _reference_ , leaves at _time_ , but it does arrive by _time_ . If that is okay, I could book that for you. -->
* What is the exact travel time on the _reference_ ?
    - The total travel time will be _number_ minutes. Is there anything else I can help you with today?
* I could use some help finding a restaurant that is moderately priced.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_restaurant: We have many options that are moderately priced. Is there a specific area or type of cuisine you are looking for?   <!-- predicted: inform_attraction_request_restaurant: The Botanic Gardens are in the centre. Would you like the restaurant to also be in the center? Do you have any type of cuisine in mind? -->
* I don t care about the cuisine but I want it to be in the _area_ .
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_inform_restaurant_recommend_restaurant: We have _restaurant_name_ . It is an _food_type_ restaurant located in the _area_ . It is moderately priced. Would you like me to book it for you?   <!-- predicted: inform_booking_hotel_inform_hotel: We have several such choices in the _area_ , _area_ and _area_ . If you have no preference for location shall I just book _number_ for you? -->
* That won t be necessary. What is the postcode?
    - slot{"restaurant_status": "available"}
    - inform_restaurant: _restaurant_name_ s postcode is cb30ad.   <!-- predicted: inform_attraction_reqmore_general: The postcode is cb30ag. Is there anything else I can help you with? -->
* Thanks for all your help.
    - bye_general_welcome_general: You re welcome, have a lovely day!   <!-- predicted: greet_general: My pleasure. Thank you for contacting _hotel_name_ TownInfo centre. Have a nice visit. -->


## story_SNG01755
* I m looking for a place to dine in the centre.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_restaurant: There are many restaurants in the centre of town, do you have a preference of food?   <!-- predicted: request_hotel: Can you please tell me what type of place and if you have any preferences? -->
* Is there anywhere that serves _food_type_ food?
    - slot{"restaurant_status": "NA"}
    - nooffer_restaurant_reqmore_general: Unfortunately there is not. What else may I check for you?   <!-- predicted: nooffer_restaurant_request_restaurant: I m sorry, but I could not find any listings for restaurants serving _food_type_ style food. Do you have any other favorite types of cuisines? -->
* Is there anywhere in the centre that serves _food_type_ food?
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_restaurant: I ve found _number_ options, sir. May I ask what type of price range were you looking for?   <!-- predicted: inform_restaurant: I found _number_ options for you _restaurant_name_ at Regent Street City Centre, _restaurant_name_ at _number_ Mill Road City Centre, and _restaurant_name_ at _number_ _hotel_name_ Road City Centre -->
* I d like something in the _pricerange_ price range.
    - slot{"restaurant_status": "available"}
    - There are _number_ _pricerange_ _food_type_ restaurants in the centre of town--_restaurant_name_ and Shiraz.
* book either for me
    - I recommend _restaurant_name_ , great word of mouth. What day and time do you want to dine? How many will be going, please?
* Can we do _weekday_ at _time_ ?
    - slot{"restaurant_status": "available"}
    - request_booking_restaurant: Sure for how many people?   <!-- predicted: book_booking_restaurant_reqmore_general: Your table for _number_ is reserved for _weekday_ at _time_ and they ll hold your table for _number_ minutes. Your reference number is _reference_ . Can I help you with anything else today? -->
* Never mind. I ll book the table myself. May I have the address and postcode? And the phone number, while you re at it.
    - Of course. _restaurant_name_ is located at Thompsons Lane Fen Ditton. The post code is cb58aq. The phone number is _number_ . Do you need any further assistance?
* No thank you that is all I need for now.
    - Glad I could help. Have a good day. Bye.


## story_SNG0322
* Hi, I d like to find a train from _hotel_name_ to _location_ .
    - slot{"train_status": "available"}
    - Certainly, there are many trains going that route. Can you specify which day you d like to travel?
* I would like to travel on _weekday_ .
    - slot{"train_status": "available"}
    - I ve got a full schedule of trains going that route on _weekday_ . Do you have a preferred time to leave or get there?
* I d like to arrive by _time_ .
    - slot{"train_status": "available"}
    - I have a train that arrives at _time_ . Will this do for you?
* Yes that would be perfect. Could I have the price and departure time?
    - slot{"train_status": "available"}
    - Yes the departure time is _time_ and the cost of the journey will be _number_ pounds.
* Great, thanks for your help!
    - reqmore_general: Not a problem! Do you need anything else?   <!-- predicted: bye_general_welcome_general: My pleasure. Please call again if you need more help. I am happy to be of service. -->
* No thanks. I appreciate the help. Have a good day.
    - You as well! Goodbye!


## story_PMUL1194
* Hello, I need information about _attraction_name_ .
    - slot{"attraction_status": "available"}
    - inform_attraction_request_attraction: There are _number_ local colleges, do you have a particular area you are interested in?   <!-- predicted: inform_attraction: That s a great choice! It is an _attraction_type_ attraction in the centre of town at market square, postcode cb23pq. The phone number is _number_ and the entrance fee is _number_ pounds. -->
* I don t have an area preference.
    - slot{"attraction_status": "available"}
    - _attraction_name_ is an architectural attraction in the center of town. They are located on Trinity Lane, in postcode cb21tt.
* What is the phone number?
    - The phone number is _number_ . Do you need any more information?
* Yes, I m looking for a train that leaves on _weekday_ for _hotel_name_
    - slot{"train_status": "available"}
    - i have over _number_ entries. let s try to narrow that down. what time would you like to arrive?
* _weekday_ at _time_ for _number_ people please
    - slot{"train_status": "available"}
    - request_train_select_train: Just to confirm, you want to leave on _weekday_ , or _weekday_ ? And where are you departing from?   <!-- predicted: offerbooked_train: Okay, I have booked you on _reference_ leaving _weekday_ at _time_ and arriving _time_ . Your reference number is _reference_ . -->
* leaving ely anytime after _time_ and I need to know how long the ride is and the specific arrival time please.
    - slot{"train_status": "available"}
    - _reference_ departs at _time_


## story_SNG1036
* I wasn t planning to stay in town tonight, but it looks like I m going to have to. Can you help me find a pretty _pricerange_ room?
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel_inform_hotel: The _hotel_name_ is a _hotel_type_ in the _area_ part of town in the _pricerange_ price range. Would you like me to book a room for you?   <!-- predicted: inform_hotel: I ve found _number_ hotels matching your preferences. The _hotel_name_ is in the _pricerange_ price range and is located in the centre of town if you are interested. -->
* I am looking for a _pricerange_ place to stay including free parking
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel_inform_hotel: _hotel_name_ is _pricerange_ and includes free parking and wifi. Would you like to book a room?   <!-- predicted: inform_booking_hotel_inform_hotel_recommend_hotel: All the _number_ hotels are _number_ star hotels. I recommend the _hotel_name_ or the _hotel_name_ . Should I book _number_ of those for you and your party? -->
* How many stars does it have? I d like a _pricerange_ place in the _area_ with _number_ stars and free parking.
    - slot{"hotel_status": "available"}
    - Yes, _hotel_name_ is a _pricerange_ _number_ star _hotel_type_ that includes free parking.
* Do they have internet there?
    - slot{"hotel_status": "unique"}
    - Yes, there is free internet provided. Would you like me to book a room?
* Sure you can book that for me, thank you!
    - request_booking_hotel: I would be happy to book a room. Please let me know your arrival day, how many nights you re staying, and the number of people who will be staying.   <!-- predicted: recommend_hotel_request_booking_hotel: OK, how about _hotel_name_ ? To book a stay I ll need to know the first day you want to stay, how many days, and how many guests. -->
* Actually, I m not ready to book yet. I think I have the information I need, thank you!
    - welcome_general: It was a pleasure.   <!-- predicted: inform_booking_hotel_inform_hotel: The _hotel_name_ is in the _pricerange_ price range. I have _hotel_name_ also in the _area_ in the _pricerange_ price range. Would you like to book? -->


## story_MUL0237
* I am looking for an _pricerange_ place to dine which serves _food_type_ food.
    - slot{"restaurant_status": "available"}
    - Several restaurants fit your criteria. Do you prefer a specific area?
* Yes, I am looking to stay in the centre of town.
    - slot{"restaurant_status": "available"}
    - inform_restaurant: The top _number_ places serving _food_type_ cuisine are _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Would you like more options?   <!-- predicted: nooffer_restaurant_request_restaurant: I m sorry, but I could not find any listings for restaurants serving _food_type_ style food. Do you have any other favorite types of cuisines? -->
* Any of those would be fine. I need a table for _number_ at _time_ on _weekday_ . Is it possible to book at _number_ of those places?
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_reqmore_general: Your table for _number_ is reserved at _restaurant_name_ . Your reference number is _reference_ . Is there anything else I can help you with today?   <!-- predicted: nobook_booking_restaurant_request_booking_restaurant: I am sorry none of them have booking available for that time,another time maybe? -->
* I m also looking for a train leaving _hotel_name_ on _weekday_ .
    - slot{"train_status": "available"}
    - There are _number_ trains leaving _hotel_name_ that day, do you have a destination or time?
* I am looking to go to _location_ and arrive by _time_
    - slot{"train_status": "available"}
    - inform_train_select_train: There are _number_ trains that fit what you are looking for. I can book you at _time_ , _time_ , or _time_ . Which do you prefer?   <!-- predicted: inform_train: There a few trains that will get you there. _reference_ departs at _time_ and arrives at _time_ . Does that work for you? -->
* I would like to book the _time_ train
    - slot{"train_status": "available"}
    - request_train: Sure thing! How many tickets do you need?   <!-- predicted: inform_train_request_train: I have several options to get you where you are going that arrive before _time_ . Which day would you be traveling? -->
* Actually, I don t need any tickets today. But can you tell me the travel time for that train?
    - inform_train_reqmore_general: Sure, the travel time is about _number_ minutes, is there anything else I can help you with?   <!-- predicted: inform_train: The total travel time _number_ minutes. You depart at _time_ and arrive at _time_ on _weekday_ . Is this acceptable? -->
* That is all I need. Thanks, and have a nice day.
    - bye_general: Okay. Thank you for calling!   <!-- predicted: bye_general_welcome_general: You re quite welcome. If you need anything else just message us again. Thanks for contacting the _hotel_name_ TownInfo Centre and have a great day! -->


## story_PMUL1259
* I want a train going to _hotel_name_ .
    - slot{"train_status": "available"}
    - request_train: Where are you leaving from and what day?   <!-- predicted: inform_train: There are several trains departing for _hotel_name_ on _weekday_ . _number_ train departs every hour starting at _time_ -->
* I am departing from Ely on _weekday_ .
    - slot{"train_status": "available"}
    - What time would you need to arrive? I have quite a few options to choose from.
* I want to go to _hotel_name_ , leave after _time_ .
    - slot{"train_status": "unique"}
    - Train _reference_ is departing from Ely to _hotel_name_ . It is leaving _weekday_ at _time_ . The price per ticket is _number_ pounds. Should I book it for you?
* Yes, please. I will need the reference number
    - request_train: Okay, can you please tell me how many people are in your party?   <!-- predicted: book_booking_train_request_train: Your _hotel_type_ reference number is _reference_ . How many people do you need train tickets for? -->
* _number_ of us
    - slot{"train_status": "booked"}
    - offerbooked_train_reqmore_general: The booking was successful. The fee will be _number_ _reference_ and the reference number is _reference_ . Is there anything else I can help you with?   <!-- predicted: book_booking_hotel: I have booked your room here is your information Booking was successful.Reference number is _reference_ -->
* I would also like to visit a _attraction_type_ in the _area_ .
    - slot{"attraction_status": "available"}
    - there is a _attraction_type_ there called _attraction_name_ . anything else today?
* Yes, I just need their postcode
    - slot{"attraction_status": "available"}
    - inform_attraction: Postcode is cb23hg.   <!-- predicted: greet_general_inform_attraction_reqmore_general: Certainly. The Lynne Strover Gallery s postcode is cb30aq. Can I help you with anything else? -->
* Ok, that s great, thank you for your help.
    - reqmore_general: Is there anything else you need help with today?   <!-- predicted: bye_general_welcome_general: It was my pleasure. Feel free to get in touch if you need anything else. -->
* No that s all, thanks!
    - bye_general_welcome_general: You are welcome, enjoy your day.   <!-- predicted: bye_general: Hope you have a great trip. Good bye. -->


## story_PMUL3957
* What can you tell me about the the good luck _food_type_ food takeaway?
    - slot{"restaurant_status": "available"}
    - inform_restaurant_reqmore_general: It s an _pricerange_ _food_type_ restaurant in the _area_ area of town. Would you like their contact info?   <!-- predicted: inform_restaurant: I found _number_ options for you _restaurant_name_ at Regent Street City Centre, _restaurant_name_ at _number_ Mill Road City Centre, and _restaurant_name_ at _number_ _hotel_name_ Road City Centre -->
* No I would like a reservation for _number_ people at _time_ on _weekday_ .
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant: I was able to book it, reference number is _reference_   <!-- predicted: book_booking_restaurant_reqmore_general: OK, I ve got your booked. The reference number is _reference_ and they ll hold your table for _number_ minutes. Can I help you with anything else? -->
* Thanks so much.
    - reqmore_general: Is there anything else I can help you with today?   <!-- predicted: bye_general: You are welcome, have a great trip! -->
* I would also like a train from _location_ on _weekday_ too.
    - slot{"train_status": "available"}
    - request_train: What time would you like to arrive?   <!-- predicted: request_taxi: I d be happy to help you with a taxi, what is your destination departure and what time would you like to arrive leave? -->
* It should arrive in _hotel_name_ by _time_ on the same day that I made the restaurant reservation for.
    - slot{"train_status": "booked"}
    - I got you _number_ ticket on the tr0363 you will arrive at _time_ , and reference is _reference_ , anything else?
* No, I think that that is all I need. Thank you very much!
    - Anytime! Enjoy your visit.


## story_PMUL4716
* I am planning a trip in _hotel_name_
    - Great! I can help you with any tourist information you may need.
* I am sorry, I meant a trip into _location_ . I am coming from _hotel_name_ and looking for a train.
    - slot{"train_status": "available"}
    - Ok, just tell me what day and time and I will be able to tell you what is available.
* I m leaving on _weekday_ . I d like to leave after _time_ .
    - slot{"train_status": "unique"}
    - inform_train_offerbook_train_request_train: _reference_ leaves at _time_ and costs _time_ . how many tickets do i book?   <!-- predicted: inform_train_offerbook_train: _reference_ leaves _hotel_name_ for _location_ on _weekday_ at _time_ . Would you like me to book it for you? -->
* _number_ people. I need the reference number too.
    - slot{"train_status": "unique"}
    - inform_train_offerbook_train: Ah, it appears that the earliest train, _reference_ , leaves at _time_ , but it does arrive by _time_ . If that is okay, I could book that for you.   <!-- predicted: offerbooked_train_reqmore_general: I booked _number_ tickets for you on _reference_ leaving Broxbourne at _time_ . _number_ _reference_ is payable at the station. Reference number is _reference_ . Will that be all? -->
* Yes, please book that train.
    - slot{"train_status": "booked"}
    - offerbooked_train_reqmore_general: I have the tickets booked for you. What else can I help with?   <!-- predicted: inform_train: You are all set. The train ID is _reference_ and it is _number_ pounds. The reference number is _reference_ . -->
* I also need things to do in town.
    - request_attraction: What sort of attraction are you thinking of doing?   <!-- predicted: inform_restaurant_request_restaurant: We have several options available to you. What type of cuisine would you prefer? We have _food_type_ , _food_type_ , _food_type_ , and _food_type_ as options. -->
* What would you suggest?
    - recommend_attraction: There are many churches in this area.   <!-- predicted: inform_hotel_reqmore_general: I also have many pricing options and amenity options. Could you give me some direction? -->
* Before I forget, I need the reference number for the train booking. Also, I am looking for attractions in the _area_ part of town, maybe something outdoors, if possible.
    - slot{"attraction_status": "available"}
    - slot{"train_status": "booked"}
    - inform_attraction_offerbooked_train: Of course, the train reference is _reference_ . Also, there are _number_ parks in the _area_ wandlebury country _attraction_type_ , and sheep s green and lammas land _attraction_type_ fen causeway.   <!-- predicted: inform_attraction_request_attraction: There are _number_ attractions in the _area_ . What type of attractions were you looking for? -->
* Thank you. May I have the phone number for wandlebury country _attraction_type_ , please?
    - slot{"attraction_status": "available"}
    - inform_attraction: the phone number is _number_   <!-- predicted: inform_hotel_reqmore_general: Absolutely! The phone number is _number_ . Is there anything else I can help you with today? -->
* That should be all fr now.
    - bye_general: welcome any time you need us   <!-- predicted: bye_general_greet_general: Thanks for letting us assist you today. Have a great visit! -->


## story_PMUL3309
* I am planning a trip in _hotel_name_
    - reqmore_general: great, would you like some information?   <!-- predicted: greet_general: Great! I can help you with any tourist information you may need. -->
* I m looking to go to _location_ . I want to leave on _weekday_ and arrive by _time_ .
    - slot{"train_status": "unique"}
    - offerbook_train: Train _reference_ arrives in _location_ at _time_ , will that work for you?   <!-- predicted: inform_train: I have _number_ trains that would suit your needs. May I suggest the _number_ that arrives by _time_ ? -->
* That would be fine. I ll need the travel time, price, and train ID, please?
    - inform_train: train id is _reference_ leaves at _time_ and will cost _number_ pounds   <!-- predicted: greet_general_inform_train: Certainly. The train s ID is _reference_ , and the price for a ticket is _number_ pounds. -->
* Thank you. Also i need to book a reservation at a restaurant named _restaurant_name_ .
    - slot{"restaurant_status": "available"}
    - inform_restaurant_select_restaurant: Okay, we have _number_ _restaurant_name_ . _number_ in the _area_ and _number_ in the centre. Which would you prefer?   <!-- predicted: request_booking_restaurant: Ok, i am getting the info up now, how many people will this be for and what time? -->
* I ll go with the _number_ in the centre. I need a booking for _number_ at _time_ on _weekday_ .
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_reqmore_general: Your table is reserved, reference _reference_ . Can I help you with anything else today?   <!-- predicted: book_booking_restaurant: I have successfully booked a table for _number_ on _weekday_ at _time_ for you. The table will be reserved for _number_ minutes and your reference number is _reference_ . -->
* That is all I need.
    - bye_general: Ok. Have a great day.   <!-- predicted: bye_general_greet_general_welcome_general: Thank you so much for calling! Enjoy your trip! Goodbye! -->


## story_PMUL2210
* I want to find a theatre in town to go to. Do you have any suggestions?
    - slot{"attraction_status": "available"}
    - inform_attraction_request_attraction: I think we can help with that. I have _number_ theaters listed. Which part of town are you in?   <!-- predicted: inform_hotel_request_hotel: There are _number_ hotels which are _number_ stars, _number_ in the _area_ and _number_ in the centre. Is there an area which you prefer? -->
* Anything in the centre of town available?
    - slot{"attraction_status": "available"}
    - inform_attraction: The adc theatre is in this area.   <!-- predicted: inform_hotel: That narrows it down to _number_ choices. I have the _hotel_name_ and the _hotel_name_ . Both are hotels located in the _area_ . Both have a _number_ star rating. -->
* What is the cost to get in? I need the postcode and the phone number as well.
    - inform_attraction: Their phone number and post code are _number_ cb58as rspectively, and I have no information on their entrance fees.   <!-- predicted: inform_attraction_reqmore_general: sheep s green and lammas land _attraction_type_ fen causeway number is _number_ and postcode is cb22ad. wandlebury country _attraction_type_ number is _number_ postcode is cb223ae. Do you need anything else? -->
* I also need a reservation for _number_ at _time_ on _weekday_ at an _food_type_ restaurant in the _pricerange_ price range. Please provide the reference number after booking.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_restaurant: I have several _food_type_ restaurants, did you want to stay in the centre area?   <!-- predicted: inform_restaurant_request_booking_restaurant_request_restaurant: There are a number of restaurants that fit what you are looking for. What area would you like and how many people? -->
* No, just as long as it is in the _pricerange_ range would be good.
    - recommend_restaurant: Okay, I recommend _restaurant_name_ in the _area_ . Would you like their information?   <!-- predicted: inform_restaurant: The _restaurant_name_ is a moderately priced _food_type_ restaurant in the centre area at _number_ Norfolk Street city centre. The phone number is _number_ and the postcode is cb12lf. -->
* Actually could you make a reservation for _number_ people at _time_ on _weekday_ please?
    - slot{"restaurant_status": "booked"}
    - I have made those reservations and your reference number is _reference_ .
* I d also like to book a tax to take us from the theater to the restaurant.
    - slot{"taxi_status": "booked"}
    - inform_taxi_reqmore_general: Booking completed!Booked car type _color_ _cartype_ Contact number _number_ Anything else?   <!-- predicted: inform_train_request_train: You ve got _number_ choices from very early morning to somewhat late evening. What would you prefer? -->
* I need to book a taxi to commute between the _number_ places
    - inform_taxi_reqmore_general: Booking completed! Booked car type _color_ _cartype_ . Contact number _number_ Anything else?   <!-- predicted: inform_taxi: Okay! Your taxi is a _color_ _color_ _cartype_ . Contact number _number_ -->
* No, that is it, thank you.
    - Thank you for contacting us and have a nice day.


## story_SNG01353
* I m interested in rooms for the night where you can get free wifi.
    - slot{"hotel_status": "available"}
    - inform_hotel_request_hotel: There are _number_ hotels or guesthouses with free wifi. What price range are you looking for?   <!-- predicted: request_hotel: Yes I have many options. What side of town did you want to stay on and what price range are you looking for. -->
* I m looking for something in a _pricerange_ price range, but it must have at least a _number_ star rating.
    - slot{"hotel_status": "available"}
    - request_hotel_select_hotel: What part of town are you interested in? _area_ , _area_ or _area_ ?   <!-- predicted: inform_hotel_select_hotel: We have lots of great hotels. Would you like to stay with the centre part of town or some other area? -->
* I don t have a preference for the area.
    - slot{"hotel_status": "available"}
    - recommend_hotel: How about _hotel_name_ ?   <!-- predicted: inform_hotel_reqmore_general: The _hotel_name_ is in the _pricerange_ price range and they do offer parking. Can I help with anything else? -->
* that will be nice. get me the reference numbers
    - slot{"hotel_status": "available"}
    - request_booking_hotel: When would you like to book this for?   <!-- predicted: reqmore_general: Sorry, just to clarify, did you actually not need a taxi after all then? -->
* Please book for _weekday_ for _number_ nights and _number_ people.
    - slot{"hotel_status": "NA"}
    - Sorry, the _hotel_type_ can t accommodate you for that time frame? Want to try a different date?
* No, I need it for those days. Can you try different _hotel_type_ ?
    - recommend_hotel: I can try for the _hotel_name_ , if you d like. They re on Chesterton Road.   <!-- predicted: inform_booking_hotel_inform_hotel_recommend_hotel: All the _number_ hotels are _number_ star hotels. I recommend the _hotel_name_ or the _hotel_name_ . Should I book _number_ of those for you and your party? -->
* Sounds good. Can you try and book that _number_ please.
    - slot{"hotel_status": "NA"}
    - inform_hotel_nobook_booking_hotel_request_booking_hotel: Sorry, the _hotel_name_ is not able to accomodate you either. I checked with the other moderately priced _number_ star lodgings with free wifi, and none have those dates available. Will any other stay work for you?   <!-- predicted: nobook_booking_hotel: Sorry, it was not successful. Can I check another _hotel_type_ or shorten the stay? -->
* Can we try for just _number_ nights then?
    - slot{"hotel_status": "booked"}
    - I ve booked that for you. The reference number is _reference_ . May I help with anything else?
* nope, that s all I need thank you!
    - bye_general_welcome_general: You re welcome. Have a great day.   <!-- predicted: bye_general: Have a great trip! Thank you for contacting us for all your booking needs. Enjoy your trip! -->


## story_PMUL3424
* Hi, you can help me find a _pricerange_ restaurant on the _area_
    - slot{"restaurant_status": "available"}
    - inform_restaurant_reqmore_general: _restaurant_name_ is a _pricerange_ restaurant. They serve _food_type_ cuisine. Does that sound good?   <!-- predicted: inform_restaurant_request_restaurant: There are _number_ restaurants in _hotel_name_ . To help narrow down results, is there a particular type of food you are looking for? -->
* Sounds great! please book it for _number_ people at _number_ !_number_ on _weekday_
    - slot{"restaurant_status": "booked"}
    - Your reservation the _restaurant_name_ was successfully booked for _weekday_ at _number_ _number_ for _number_ . Your Reference number is _reference_ .
* I also need a train on _weekday_ .
    - request_train: I can help with that, too. Where are you departing from and where are you going, please?   <!-- predicted: request_taxi: I can help with that. What is your departure site, destination, and the time you need it? -->
* I will be departing _hotel_name_ and going to stansted Airport.
    - slot{"train_status": "available"}
    - I have _number_ trains. Do you have a preferred arrival or departure time?
* I want the train to leave after _time_
    - inform_train: There is a train that leaves at _time_ .   <!-- predicted: inform_train_offerbook_train: The train that leaves earliest after _time_ is the _reference_ train leaving at _time_ . Would that suffice? -->
* That should be perfect. Can I get reservations for _number_ ?
    - slot{"train_status": "booked"}
    - offerbooked_train: Yes, I booked the tickets and your reference number is _reference_   <!-- predicted: offerbooked_train_reqmore_general: Booking was successful for _reference_ , the total fee is _number_ _reference_ payable at the station. Your reference number is _reference_ . Do you need further assistance? -->
* Perfect!! Thank you so much.
    - greet_general: Thanks you for visiting us in _hotel_name_ and enjoy your trip!   <!-- predicted: reqmore_general: You are welcome. Is there anything else I can help you with today? -->


## story_MUL0286
* I need to find a restaurant that serves Weish food in the centre of town please.
    - slot{"restaurant_status": "NA"}
    - nooffer_restaurant_reqmore_general: I m sorry, but there are no restaurants that match your criteria. Would you like to broaden your search?   <!-- predicted: nooffer_restaurant_request_restaurant: I m sorry, but I could not find any listings for restaurants serving _food_type_ style food. Do you have any other favorite types of cuisines? -->
* Yes, are there any Weish restaurants in the _pricerange_ price range that are in _area_ _hotel_name_ ?
    - slot{"restaurant_status": "NA"}
    - nooffer_restaurant: I m sorry, but there are no _food_type_ restaurants in all of _hotel_name_ .   <!-- predicted: nooffer_restaurant_request_restaurant: Unfortunately there are none fitting that criteria either, would you like me to search for a different type of restaurant? -->
* Can you change my food preference to _food_type_ then? I still want to be in the _pricerange_ range and center of town.
    - slot{"restaurant_status": "available"}
    - I found _number_ options for you _restaurant_name_ at Regent Street City Centre, _restaurant_name_ at _number_ Mill Road City Centre, and _restaurant_name_ at _number_ _hotel_name_ Road City Centre
* Please book a table for _number_ at _restaurant_name_ .
    - slot{"restaurant_status": "available"}
    - request_booking_restaurant: I cannot book a reservation for you until I know what time and day your planning on going there.   <!-- predicted: inform_booking_restaurant_request_booking_restaurant: Sure, I d be happy to book this for you. What day, time and how many people will be dining? -->
* I apologize. I would like a table for _number_ at _time_ on _weekday_ . Please tell me my reference number, if you don t mind.
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_reqmore_general: I have confirmed your reservation at _restaurant_name_ s on _weekday_ at _time_ for _number_ . The reference number is _reference_ . Is there anything else you need help with?   <!-- predicted: book_booking_restaurant: You are booked! Your table will be reserved for fifteen minutes and your reference number is _reference_ . -->
* Yes, I m also looking for a train to _hotel_name_ arriving by _time_ .
    - slot{"train_status": "available"}
    - There are _number_ trains that meet those criteria. Where are you departing from and on what day?
* It should be on _weekday_ as well, and depart from the stansted airport
    - slot{"train_status": "available"}
    - inform_train_request_train: There are _number_ trains that will arrive prior to _time_ . Do you prefer a particular arrival time?   <!-- predicted: inform_train_offerbook_train_request_train: _reference_ arrives at _time_ after a _number_ minute trip. How many tickets would you like? -->
* Yes I need to arrive by _time_ as I stated earlier.
    - slot{"train_status": "unique"}
    - I found _number_ that arrives by _time_ it is _reference_ , would you like to book that?
* Sure that sounds good, I will need _number_ tickets please, and the reference number.
    - slot{"train_status": "booked"}
    - offerbooked_train: Booking was successful, the total fee is _number_ _reference_ payable at the station. Reference number is _reference_ .   <!-- predicted: greet_general_offerbooked_train_reqmore_general: Great! I have you booked for _number_ tickets on Train _reference_ with a total fee of _number_ _reference_ . Your reference number is _reference_ . Anything else? -->
* Perfect, thank you!
    - You re welcome. Can I help you with anything else?
* No, thank you. That s all I need today.
    - bye_general: Thank you for using our service. Have a wonderful day!   <!-- predicted: bye_general_welcome_general: Ok have a great day good bye. -->


## story_PMUL0006
* I m looking for a place to stay in _hotel_name_ .
    - inform_hotel_request_hotel: We have _number_ locations to stay, do you have any other requirements?   <!-- predicted: inform_hotel: I ve found _number_ hotels matching your preferences. The _hotel_name_ is in the _pricerange_ price range and is located in the centre of town if you are interested. -->
* I d like a moderately priced _hotel_type_ in the _area_ , with free wifi.
    - slot{"hotel_status": "available"}
    - inform_hotel_reqmore_general: _hotel_name_ is your choice. its located in _number_ hills road. can i give you the address   <!-- predicted: inform_hotel_select_hotel: I have _number_ options with those specifications. The _hotel_name_ and the _hotel_name_ both with free wifi and parking. Which would you prefer? -->
* You just gave me the address. Does it have free parking?
    - inform_hotel_reqmore_general: Yes, both free internet and free parking. Can I help you with anything else today?   <!-- predicted: greet_general_inform_hotel_reqmore_general: Of course! The address of the _hotel_name_ is kingfisher way, hinchinbrook business _attraction_type_ , huntingdon and it s phone number is _number_ , would you like anything else? -->
* I m looking for a _food_type_ restaurant as well. Is there anything near the _hotel_type_ ?
    - slot{"restaurant_status": "available"}
    - inform_restaurant_select_restaurant: There are _number_ _food_type_ restaurants in the _area_ . _number_ are in the _pricerange_ range and _number_ _pricerange_ . Do you have a preference?   <!-- predicted: inform_hotel_select_hotel: I have _number_ hotels in the _pricerange_ price range and _number_ guesthouses in the _pricerange_ price range. Do you have a preference? -->
* I really need that to be in the _area_ .
    - inform_restaurant_select_restaurant: Yes, I have _restaurant_name_ if you would like a _pricerange_ option, or there are _number_ more _pricerange_ options. Do you have a preference?   <!-- predicted: inform_booking_restaurant_inform_restaurant: I have _number_ restaurants that fit those criteria. _restaurant_name_ , _restaurant_name_ , the _attraction_type_ , _restaurant_name_ and restaurant _number_ _number_ . Which would you like a booking for? -->
* _restaurant_name_ would be just fine. I need the postcode please.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_reqmore_general: The postcode is cb17dy. Is there anything else I can help you with?   <!-- predicted: inform_restaurant_request_booking_restaurant: Their postcode is cb11lh and if you want a reservation just let me know the time, party size, and day and I ll make it for you. -->
* Thanks. Yes, I will need a taxi from the _hotel_type_ to _restaurant_name_ restaurant.
    - slot{"taxi_status": "available"}
    - What time would you like to arrive at the restaurant?
* I m not sure I just need to leave the _hotel_type_ by _time_ .
    - slot{"taxi_status": "booked"}
    - a _color_ _cartype_ has been booked for you. the contact is _number_
* Thanks for all of your help, I m all set now. Bye.
    - bye_general: Good bye, have a great day.   <!-- predicted: bye_general_greet_general_welcome_general: Thank you for using our service. Call us anytime. Take care. Goodbye. -->


## story_SNG0069
* Can you book me a taxi from _hotel_name_ to _restaurant_name_ ?
    - slot{"taxi_status": "available"}
    - Easy enough. What time would you like to leave by as well as arrive to?
* I would like to arrive at De Luca by _time_ . It doesn t matter when I leave.
    - slot{"taxi_status": "booked"}
    - inform_taxi: I booked that for you. The car will be a _color_ _cartype_ and the contact number is _number_ .   <!-- predicted: inform_taxi_reqmore_general: Alright, I got you booked. the car will be a _color_ _cartype_ and the contact number is _number_ . Anything else I can help you with? -->
* Thank you very much for you help today.
    - bye_general_welcome_general: You are very welcome, have a great day!   <!-- predicted: reqmore_general_welcome_general: You are welcome. Can I help you find anything else? -->


## story_PMUL2563
* Hi, I am traveling to _hotel_name_ and could use some help for sure. I am so excited to see some local tourist attractions.
    - We have _number_ attractions to choose from, anything specific that you would like to tell us to help narrow it down?
* I m looking for a _hotel_type_ called _hotel_name_ .
    - slot{"hotel_status": "available"}
    - _hotel_name_ is a _number_ -star _hotel_type_ in the center of town. Its address is Sleeperz _hotel_type_ , _location_ .
* Can you please book a room for _number_ people for _number_ nights starting on _weekday_ ?
    - slot{"hotel_status": "booked"}
    - Booking was successful.Reference number is _reference_ anything else i can help?
* Thanks. I am also looking for places to go in town. Perhaps an attraction in the city centre.
    - slot{"attraction_status": "available"}
    - recommend_attraction: I have the _attraction_name_ located at jesus lane and it s free entrance.   <!-- predicted: inform_attraction_request_attraction: We have several things to do! _attraction_type_ , colleges, museums...What type of attraction are you most interested in? -->
* That sounds perfect. Thanks!
    - reqmore_general: Can I help you with anything else?   <!-- predicted: greet_general: Great! I can help you with any tourist information you may need. -->
* No thanks. That s all I need. Goodbye.
    - Thank you for contacting us, have a nice day.


## story_PMUL0919
* I am looking for a dining place that serves _food_type_ food.
    - slot{"restaurant_status": "available"}
    - inform_restaurant: There are many _food_type_ restaurants. What price range do you prefer?   <!-- predicted: inform_restaurant_request_restaurant: I have found _number_ _food_type_ restaurants on the _area_ side. There are _number_ _pricerange_ and _number_ _pricerange_ . Did you have a price range in mind? -->
* _pricerange_ would be great.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_recommend_restaurant: I found _number_ that would meet your needs. What about _restaurant_name_ ? It is located at _number_ Regent Street City Centre   <!-- predicted: inform_restaurant_select_restaurant: I have the _restaurant_name_ which serves _food_type_ . I also have _restaurant_name_ that serves _food_type_ food. Which would you prefer? -->
* That sounds great. Please make me a reservation for _number_ at _time_ on _weekday_
    - slot{"restaurant_status": "available"}
    - request_booking_restaurant: How many people?   <!-- predicted: request_train: I can. Will you be departing from _location_ ? -->
* I already told you how many people. are you paying attention?
    - slot{"restaurant_status": "booked"}
    - sorry was trying to confirm. i have booked _restaurant_name_ and Reference number is _reference_ .
* Wait, is that _restaurant_name_ or a different restaurant you ve booked for me?
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant: no i booked _restaurant_name_ . is that fine?   <!-- predicted: inform_restaurant: There is _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _restaurant_name_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _area_ _food_type_ , _food_type_ , _food_type_ , and _food_type_ food available in the centre. -->
* I _restaurant_name_ an _food_type_ restaurant? We didn t discuss _restaurant_name_ at all.
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant: I changed the restaurant and booked for you. Your new Reference number is _reference_ .   <!-- predicted: inform_booking_restaurant_inform_restaurant: Absolutely! They are a great _food_type_ restaurant in the centre of town. They are on the _pricerange_ side. Would you like help in reserving a table? -->
* I also looking for a train. The train should go to _hotel_name_ and should depart from stansted airport.
    - slot{"train_status": "available"}
    - request_train: On what day do you need to travel?   <!-- predicted: inform_train_request_train: What day would you be traveling? There are _number_ trains on that route. There is a train that departs _weekday_ at _time_ and will arrive in Ely at _time_ . -->
* I need to the train on _weekday_ and I need to arrive by _time_ .
    - slot{"train_status": "unique"}
    - I have _reference_ that will get you to _hotel_name_ by _time_ . Do you need any tickets today?
* I don t need to book now. I would like the ticket price, please.
    - The price per ticket is _number_ pounds.
* That s all I need.
    - reqmore_general: May I assist you with anything else today?   <!-- predicted: bye_general_welcome_general: So happy to be of service, and thanks for using _hotel_name_ TownInfo centre today. Have a wonderful day! -->
* No thank you that will be all
    - bye_general_welcome_general: Thank you for calling. I hope you enjoy your trip. Goodbye!   <!-- predicted: bye_general: Thank you for using our system today! -->


## story_MUL0260
* Are there any trains on _weekday_ that travel from _location_ to _hotel_name_ ?
    - slot{"train_status": "available"}
    - There are several trains traveling from _location_ to _hotel_name_ on _weekday_ . Is there any particular time you are looking for? The earliest is _time_ .
* The train should arrive by _time_ please.
    - slot{"train_status": "available"}
    - inform_train_reqmore_general: The _reference_ arrives at _time_ . Does that work for you?   <!-- predicted: inform_train: There a few trains that will get you there. _reference_ departs at _time_ and arrives at _time_ . Does that work for you? -->
* I think that will work. What is the departure time of that train?
    - slot{"train_status": "unique"}
    - That train leaves at _time_ . Would you care to book passage?
* Yes please, can I get my train ID? I m also want to look for a restaurant that serves _food_type_ with a _pricerange_ price range.
    - slot{"restaurant_status": "available"}
    - inform_train_request_train: Your train ID is _reference_ . Am I correct that you will only be needing _number_ ticket?   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* I don t need a ticket right now. But can you tell me if there are any moderately priced restaurants in the center of town that serve _food_type_ food?
    - slot{"restaurant_status": "NA"}
    - I m sorry, there aren t. Another type of food, perhaps?
* Well, let s try a restaurant that serves _food_type_ food. Still in the centre.
    - slot{"restaurant_status": "unique"}
    - _restaurant_name_ and _restaurant_name_ are both moderately priced _food_type_ restaurants in the center of town. Would you like a reservation at _number_ of these?
* Varsity Restaurant. Please make a reservation for _number_ people at _time_ on _weekday_ .
    - slot{"restaurant_status": "NA"}
    - Unfortunately, I am unable to book for that day time. Would you like to book your table for another day or time?
* Could you please try for _time_ on the same day?
    - slot{"restaurant_status": "booked"}
    - Booking was successful at _restaurant_name_ for _time_ . The table will be reserved for _number_ minutes. Your reference number is _reference_ . Can I help with anything else?
* No, thank you. That was all I needed. Thank you. Have a good day!
    - bye_general: We are happy to help. Thank you for using our service. Have a great day!   <!-- predicted: bye_general_welcome_general: I m happy we could be of service. Thank you for using the _hotel_name_ TownInfo centre. Goodbye! -->


## story_PMUL0069
* I m looking for some _food_type_ food restaurants near the centre, please.
    - slot{"restaurant_status": "NA"}
    - nooffer_restaurant: I am sorry there are no _food_type_ Restaurants near centre.   <!-- predicted: nooffer_restaurant_request_restaurant: I m sorry, but I could not find any listings for restaurants serving _food_type_ style food. Do you have any other favorite types of cuisines? -->
* What kind of _pricerange_ restaurants are in the center of town?
    - slot{"restaurant_status": "NA"}
    - Unfortunately there aren t any _food_type_ places. Do you want to try other cuisine types?
* yes let me see the options
    - inform_restaurant_select_restaurant: There is a variety of choices; _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , Gastro Pub, etc... Do you have a preference?   <!-- predicted: nooffer_restaurant_request_restaurant: Unfortunately there are no restaurants available that fit that criteria. Is there another type of cuisine you might be interested in eating? -->
* i want _food_type_ food.
    - slot{"restaurant_status": "available"}
    - recommend_restaurant: _restaurant_name_ is a nice place would you like that info ?   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* Yes can I get a address and phone number please?
    - slot{"restaurant_status": "available"}
    - inform_restaurant_reqmore_general: Certainly, the phone number for the _restaurant_name_ restaurant is _number_ and the address is _number_ Regent Street City Centre. May I help you with anything else today?   <!-- predicted: inform_restaurant: _number_ is the phone number. _number_ Bridge Street City Centre, cb21uf is the address. -->
* Yes I am also looking for a place in the same area as the restaurant with free parking.I want it for _number_ people for _number_ nights starting _weekday_ .
    - slot{"hotel_status": "available"}
    - select_hotel: Would you like something _pricerange_ , _pricerange_ , or _pricerange_ ?   <!-- predicted: inform_hotel_request_hotel: There are _number_ available that match what you re looking for, do you have any preference for what area you want to stay in? -->
* That doesn t matter just a _hotel_type_ in the same area with free parking.
    - slot{"hotel_status": "available"}
    - inform_hotel_recommend_hotel: There are _number_ options here. Both are _pricerange_ . I recommend _hotel_name_ .   <!-- predicted: inform_restaurant_request_restaurant: I ve got _number_ _food_type_ restaurants in that area, is there a price range you want to narrow it down to? -->
* That would be great. Can you book it on _weekday_ for _number_ people and _number_ nights.
    - slot{"hotel_status": "booked"}
    - Booking was successful, and your reference number is _reference_ . Is there anything else I can assist you with?
* Perfect, thank you for all your help. That is all for now.
    - bye_general: Thank you for using our services.   <!-- predicted: bye_general_greet_general_welcome_general: You are welcome. Thank you for using our service. Goodbye! -->


## story_PMUL0713
* Hi. Can you help me find a train?
    - greet_general_request_train: Sure. Where will you be departing from and where do you want to go?   <!-- predicted: request_train: Sure! When are you wanting to travel, where are you leaving from, where would you like to go and what time? -->
* I want to depart from _location_ and go to _hotel_name_ . I also want to leave on _weekday_
    - slot{"train_status": "available"}
    - request_train: What time would you like to leave?   <!-- predicted: inform_train: _reference_ leaves for _location_ from _hotel_name_ leaves at _number_ -->
* I need to leave after _time_ . Can you help find something?
    - slot{"train_status": "unique"}
    - I have the _reference_ leaving at _time_ . Would you like me to book that for you?
* Yes that will be fine, can you book me a seat for _number_ people and give me the reference number?
    - slot{"train_status": "booked"}
    - I have booked you on the _reference_ for _number_ people with reference number is _reference_ . The total fee is _number_ _reference_ payable at the station. Will that be all?
* Actually, I could use some help finding an _pricerange_ restaurant in the _area_ part of town.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_select_restaurant: I have _number_ restaurants that meet your requests. Would you be interested in _food_type_ , _food_type_ , _food_type_ , or _food_type_ cuisine?   <!-- predicted: inform_restaurant: The top _number_ places serving _food_type_ cuisine are _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Would you like more options? -->
* I would like _food_type_ , please
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_recommend_restaurant_reqmore_general: _hotel_name_ Lodge restaurant fits your criteria. Would you like more information on it or would you like to book a table?   <!-- predicted: inform_booking_restaurant_inform_restaurant: I have _number_ restaurants that fit those criteria. _restaurant_name_ , _restaurant_name_ , the _attraction_type_ , _restaurant_name_ and restaurant _number_ _number_ . Which would you like a booking for? -->
* I just need the address please.
    - The address is _hotel_name_ Lodge _hotel_type_ _number_ Huntingdon Road City Centre.
* Thank you for the address. That is all the help I need today.
    - bye_general_greet_general: Enjoy the rest of your day, goodbye!   <!-- predicted: inform_attraction_reqmore_general: Sure thing. The address is pool way, whitehill road, off newmarket road. Can I help with anything else? -->


## story_PMUL3310
* I am looking for a brazliian restaurant in the centre.
    - slot{"restaurant_status": "NA"}
    - nooffer_restaurant: Sorry, I couldn t find any food of that type.   <!-- predicted: nooffer_restaurant_request_restaurant: I m sorry, but I could not find any listings for restaurants serving _food_type_ style food. Do you have any other favorite types of cuisines? -->
* There are no _food_type_ restaurants anywhere in _hotel_name_ ?
    - slot{"restaurant_status": "NA"}
    - No, their are not any. Would you like to pick a different type of food?
* Yes, what about _food_type_ please.
    - slot{"restaurant_status": "available"}
    - request_restaurant: what price range are you comfortable with?   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* Something in the _pricerange_ price range would be good.
    - slot{"restaurant_status": "available"}
    - request_restaurant: Do you have a preference as to what area of town you dine in?   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* Yes, the centre is preferable.
    - How about _restaurant_name_ ? It s located in the centre and _pricerange_ price range.
* Sounds good! Please book a table for _number_ people at _time_ on _weekday_ .
    - slot{"restaurant_status": "booked"}
    - Your table has been booked. Your reference number is _reference_ . Is there anything else I can help you with today?
* Thanks. Yes, I also need a train from _hotel_name_ to Ely, please.
    - slot{"train_status": "available"}
    - Those trains run every _number_ hours, starting at _time_ . What time would you like to depart?
* Thank you! Anytime is fine, as long as I arrive by _time_ on _weekday_ .
    - slot{"train_status": "unique"}
    - inform_train_offerbook_train_request_train: Train _reference_ departs _hotel_name_ at _time_ and arrives in Ely at _time_ . The price is _number_ pounds. Do you want me to book? If yes, for how many passengers?   <!-- predicted: inform_train_offerbook_train: The _reference_ will be arriving just before _time_ on _weekday_ . It departs at _time_ and is an _number_ minute ride. Would you like me to book it? -->
* Yes please book for _number_ people
    - slot{"train_status": "booked"}
    - Booking was successful, the total fee is _number_ _reference_ payable at the station .Reference number is _reference_ . Can I help you with anything else?
* Thank you. That was all I needed today. Goodbye.
    - I am glad that I can help. Have a nice stay.


## story_MUL1159
* Hey, can you help me out? I am looking for something to do. What kind of _attraction_type_ is out there in the center of town?
    - slot{"attraction_status": "NA"}
    - nooffer_attraction_request_attraction: There are no _attraction_type_ attractions in the centre of town. Would you like to look in a different area?   <!-- predicted: inform_attraction_request_attraction: I m sorry, there are no _attraction_type_ attractions in the centre of the city. Would you like to try a different area of the city? -->
* That s not necessary. Are there any colleges in that area instead?
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: There are _number_ colleges in town centre. _hotel_name_ and Caius _attraction_name_ is on trinity street with free entrance. Do you want more information on any others?   <!-- predicted: inform_attraction: _attraction_name_ , _attraction_name_ , _attraction_name_ , and _attraction_name_ are some of the colleges in that area. -->
* That actually sounds great. Could you give me the phone number for _hotel_name_ and Caius _attraction_name_ ?
    - slot{"attraction_status": "available"}
    - The phone number for the _hotel_name_ and Caius _attraction_name_ is _number_ . Can I help you with anything else?
* Actually, yes. I am looking for a _pricerange_ place to stay with free parking.
    - slot{"hotel_status": "available"}
    - request_hotel: What part of town would you like to stay in?   <!-- predicted: inform_hotel_select_hotel: I have _number_ options with those specifications. The _hotel_name_ and the _hotel_name_ both with free wifi and parking. Which would you prefer? -->
* I would prefer the _area_ side.
    - slot{"hotel_status": "available"}
    - inform_hotel_request_hotel: There are several guest houses on the _area_ side. Do you need free parking or internet?   <!-- predicted: inform_attraction_reqmore_general: I have the _hotel_name_ _attraction_name_ of Technology located in the _area_ side of town. It s at the site of the Old Pumping Station on Cheddar s lane. Would you like more information? -->
* Yes, both please. I m looking to get a room just for me for _number_ nights on _weekday_ at a place that offers wifi and parking free.
    - slot{"hotel_status": "available"}
    - request_booking_hotel: I am sorry, but that was not successful. Would you like to pick a different day or shorter stay?   <!-- predicted: inform_hotel_request_hotel: There are _number_ available that match what you re looking for, do you have any preference for what area you want to stay in? -->
* How about _number_ night?
    - slot{"hotel_status": "booked"}
    - book_booking_hotel: Great! You re booked at _hotel_name_ for _number_ night. Your reference number is _reference_ . Would you like more information?   <!-- predicted: book_booking_hotel_reqmore_general: You re booked at the _hotel_name_ Guesthouse for _number_ night on _weekday_ . The reference number is _reference_ . Can I help with anything else? -->
* I d also like a taxi between the places if possible.
    - slot{"taxi_status": "available"}
    - I can help with that. When would you like to either leave or arrive? And do you want the taxi from the _attraction_name_ to the _hotel_type_ or the other way around?
* I need to go from the _attraction_name_ to the _hotel_type_ , and I want to leave the _attraction_name_ by _time_ , please.
    - slot{"taxi_status": "booked"}
    - OK, I have a _color_ _reference_ taxi booked to pick you up. Their contact number is _number_ . Is there anything else I can do for you today?
* No, that is all I will need today. Thank you very much.
    - You re quite welcome! Thanks for contacting the _hotel_name_ TownInfo Centre and have a great day!


## story_PMUL4644
* I m hoping you can help me find an _pricerange_ _hotel_type_ on the _area_ end
    - slot{"hotel_status": "NA"}
    - There are no results. Is there another area we can search or a different price range?
* I am looking specifically for a guesthouse in the _pricerange_ price range in the _area_ . Can you look again please?
    - slot{"hotel_status": "NA"}
    - nooffer_hotel: I m sorry, there are no hotels meeting your requirements.   <!-- predicted: inform_booking_hotel_nobook_booking_hotel: I m sorry, my system is not allowing me to book that location for some reason. Would you like to try again? -->
* Perhaps you could check the _pricerange_ price range in the _area_ area of town.
    - slot{"hotel_status": "available"}
    - recommend_hotel: _hotel_name_ is very nice.   <!-- predicted: inform_booking_restaurant_inform_restaurant_nooffer_restaurant: There are no _food_type_ restaurants on the _area_ side but there is _number_ on the _area_ side. Would that suffice? -->
* Okay, great! I ll need it booked for _weekday_ , _number_ nights, and _number_ people, please?
    - slot{"hotel_status": "booked"}
    - book_booking_hotel_reqmore_general: Your booking for the _hotel_name_ guesthouse is successful. Your reference number is _reference_ . Can I help you with anything else?   <!-- predicted: book_booking_hotel: Sure, booking was successful. Your confirmation number is _reference_ . -->
* Yes, I m also looking for a place to dine. I d like for it to be in the _area_ and serve _food_type_ food.
    - slot{"restaurant_status": "NA"}
    - We don t have any that match. Do you have any other location preferences?
* Okay can you look out for any in still the same location with the _hotel_type_ that serves _food_type_ food.
    - slot{"restaurant_status": "unique"}
    - _restaurant_name_ is _food_type_ . Want to book?
* No thank you. I just need the price range and postcode.
    - slot{"restaurant_status": "available"}
    - inform_restaurant: _restaurant_name_ is in the _pricerange_ price range, and the postcode is cb41nl.   <!-- predicted: recommend_restaurant_reqmore_general: If you ask me, the _restaurant_name_ serves the best _food_type_ food around. Their postcode is cb17dy. You can reach them at _number_ . Can I help with anything else? -->
* Thank you for all your help!
    - reqmore_general: Can I be of further assistance today?   <!-- predicted: bye_general_welcome_general: My pleasure. Please call again if you need more help. I am happy to be of service. -->
* That s all, goodbye!
    - bye_general: Have a great day.   <!-- predicted: bye_general_greet_general_welcome_general: Thank you for using our service. Call us anytime. Take care. Goodbye. -->


## story_SNG0715
* Is there an _pricerange_ _food_type_ restaurant in town.
    - slot{"restaurant_status": "available"}
    - recommend_restaurant: Yes, The _restaurant_name_ in the city centre is a good, _pricerange_ restaurant.   <!-- predicted: inform_restaurant_request_restaurant_select_restaurant: there are _number_ in town. did you have a certain part of town you want to dine in? i have some in the centre and _area_ . -->
* Excellent! I don t need a table right now, but if you could give me the address and phone number, that would be great.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_reqmore_general: It is located at _number_ Mill Road City Centre and the phone number is _number_ . Is there anything else I can help you with?   <!-- predicted: inform_restaurant: I found _number_ options for you _restaurant_name_ at Regent Street City Centre, _restaurant_name_ at _number_ Mill Road City Centre, and _restaurant_name_ at _number_ _hotel_name_ Road City Centre -->
* No thanks. That would be all for today. Have a nice day.
    - You re welcome, goodbye


## story_MUL0379
* I am looking to get to the _restaurant_name_ restaurant please, how do I get there?
    - slot{"restaurant_status": "available"}
    - reqmore_general_request_taxi: Would you like for me to book you a taxi to the restaurant?   <!-- predicted: inform_restaurant_request_restaurant: There are fourteen restaurants in the _area_ . Is there any kind of food you re looking for? -->
* I need you to book the restaurant for me if that s okay. For _number_ people at _time_ on _weekday_ is what I request. Can I get the reference number too?
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_bye_general: Okay I booked it and your reference number is _reference_ . Have a great day.   <!-- predicted: book_booking_restaurant_reqmore_general: It is booked here is your ref number _reference_ is there anything else you need? -->
* Actually, I m also looking for a train. I need to go to _location_ on the same day as the restaurant booking.
    - slot{"train_status": "available"}
    - No problem. Would you like to specify where you re departing from and what time you d like?
* I am departing from _location_ and need to go to _hotel_name_ . I want to arrive by _time_ .
    - slot{"train_status": "available"}
    - inform_train_request_train: I have several options to get you where you are going that arrive before _time_ . Which day would you be traveling?   <!-- predicted: inform_taxi: Booking completed! your taxi will be _color_ _cartype_ Contact number is _number_ -->
* I will be traveling on _weekday_ .
    - slot{"train_status": "unique"}
    - There are _number_ trains for that search. Would you look me to book you the _number_ that leaves at _time_ ?
* What are the travel times for those trains?
    - inform_train: They are both _number_ minutes.   <!-- predicted: inform_train_offerbook_train: The train ID for that is _reference_ and the travel time is _number_ minutes. Would you like me to book you a seat? -->
* Thank you, that should be all for today.
    - bye_general: Excellent! Have a wonderful day, and thank you for using our service.   <!-- predicted: greet_general: My pleasure. Thank you for contacting _hotel_name_ TownInfo centre. Have a nice visit. -->


## story_PMUL4001
* I am planning a trip in _hotel_name_
    - reqmore_general: Would you like to come by bus, or train?   <!-- predicted: greet_general: Great! I can help you with any tourist information you may need. -->
* I m actually looking for a particular attraction called the fitzwilliam _attraction_name_ .
    - slot{"attraction_status": "available"}
    - reqmore_general: Yes nice place. Did you need any info on it ?   <!-- predicted: inform_attraction: That s a great choice! It is an _attraction_type_ attraction in the centre of town at market square, postcode cb23pq. The phone number is _number_ and the entrance fee is _number_ pounds. -->
* What type of attraction is that?
    - inform_attraction_reqmore_general: It s a _attraction_name_ . Will that be all?   <!-- predicted: inform_attraction: _attraction_name_ is in the center and it s known for it s _attraction_type_ . The entrance fee is free. -->
* Thanks. I do actually need help finding a train. I want to go to _location_ on _weekday_ .
    - slot{"train_status": "available"}
    - request_train: Okay, and what time would you like to leave?   <!-- predicted: inform_train_request_train: There are _number_ trains traveling on _weekday_ . Where will you be departing from and where is your destination? -->
* I would like to depart _hotel_name_ after _time_ .
    - slot{"train_status": "available"}
    - request_train: how many tickets please?   <!-- predicted: inform_train: There a few trains that will get you there. _reference_ departs at _time_ and arrives at _time_ . Does that work for you? -->
* I ll need tickets for _number_ people. Can I have the reference number please?
    - slot{"train_status": "booked"}
    - offerbooked_train_reqmore_general: Your train booking for _number_ on the _reference_ was successful. Your Reference number is _reference_ . Is there anything else I can help you with?   <!-- predicted: offerbooked_train: I was able to book you _number_ ticket on train _reference_ . Your total cost is _number_ _reference_ payable at the station. Your reference number is _reference_ . -->
* naw i m good thanks
    - bye_general: Well, have a great day.   <!-- predicted: bye_general_greet_general: Thanks for letting us assist you today. Have a great visit! -->
* Likewise, thanks very much!
    - You are very welcome, it was a pleasure helping you. Goodbye.


## story_PMUL3495
* Can you help me find a _attraction_name_ to visit?
    - slot{"attraction_status": "available"}
    - inform_attraction_request_attraction: We have _number_ colleges. Is there a certain area you would like to visit?   <!-- predicted: greet_general_inform_attraction_reqmore_general: I certainly can. _attraction_name_ is a _attraction_name_ located in the center of town, on King s Parade. There s a _number_ pound entrance fee. Do you need any additional information? -->
* Not really, what do you suggest? Can I have the address, postcode, and entrance fee?
    - slot{"attraction_status": "available"}
    - recommend_attraction: Sue i suggest _attraction_name_ that is in the center, has a postcode of cb23bu, an address of saint andrew s street and the entrance is free of cost.   <!-- predicted: inform_restaurant: There is _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _restaurant_name_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _area_ _food_type_ , _food_type_ , _food_type_ , and _food_type_ food available in the centre. -->
* Thank you. can you also find me a _food_type_ restaurant?
    - slot{"attraction_status": "available"}
    - slot{"restaurant_status": "available"}
    - request_restaurant: what is our price range?   <!-- predicted: inform_restaurant_request_restaurant: There are _number_ _food_type_ restaurants in the area. _number_ are moderately priced and _number_ are _pricerange_ . Can I ask what price range you would like? -->
* Price is no object, you usually only get to place like _hotel_name_ once in your life. I will go with what you recommend, I just need their address.
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_recommend_restaurant: I would recommend _restaurant_name_ at Thompsons Lane Fen Ditton. Would you like me to book it for you?   <!-- predicted: inform_restaurant_request_booking_restaurant: Their postcode is cb11lh and if you want a reservation just let me know the time, party size, and day and I ll make it for you. -->
* Is that in the centre area?
    - slot{"restaurant_status": "available"}
    - inform_restaurant: yes it is in the centre   <!-- predicted: inform_train: They are both _number_ minutes. -->
* What is the address?
    - The address is Thompsons Lane Fen Ditton
* Can you book a taxi for me to get from _attraction_name_ to _restaurant_name_ ? I ll need to leave _attraction_name_ by _time_ . Please give contact number and car type.
    - slot{"taxi_status": "booked"}
    - inform_taxi: Your booking is complete. The booked car type is a _color_ _cartype_ . The contact number is _number_ .   <!-- predicted: inform_taxi_reqmore_general: Alright, I got you booked. the car will be a _color_ _cartype_ and the contact number is _number_ . Anything else I can help you with? -->
* Thank you for your help!
    - reqmore_general_welcome_general: You are welcome. Is there anything else you will be needing today?   <!-- predicted: bye_general_welcome_general: Glad I could be of help, thank you. -->
* That is all for today, thanks for the help!
    - Happy to help, good day too.


## story_PMUL0276
* I am looking for an _pricerange_ place to eat.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_reqmore_general: We have plenty of high end _pricerange_ options in _hotel_name_ , _number_ to be exact. Anything I can do to narrow down your options?   <!-- predicted: inform_restaurant_request_restaurant: There are _number_ _pricerange_ restaurants in town. Do you have a food preference or an area of town you want to eat in? -->
* Are there any _food_type_ restaurants in the centre of town?
    - slot{"restaurant_status": "NA"}
    - inform_booking_restaurant_inform_restaurant_nooffer_restaurant: There are not any _pricerange_ _food_type_ restaurants in the centre, but there is a moderately priced _number_ . Would that work for you?   <!-- predicted: nooffer_restaurant_request_restaurant: I m sorry, but I could not find any listings for restaurants serving _food_type_ style food. Do you have any other favorite types of cuisines? -->
* Could you check again for an _pricerange_ _number_ ?
    - slot{"restaurant_status": "unique"}
    - It is _restaurant_name_ , would you like a reservation?
* Yes I need it _weekday_ at _time_ for _number_ people.
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant: Booking was successful. The table will be reserved for _number_ minutes. Reference number is _reference_ .   <!-- predicted: book_booking_restaurant_reqmore_general: Your table for _number_ is reserved for _weekday_ at _time_ and they ll hold your table for _number_ minutes. Your reference number is _reference_ . Can I help you with anything else today? -->
* Thanks. I m also looking for _hotel_name_ . Do you know where it is?
    - slot{"hotel_status": "available"}
    - Yes, that s a great guesthouse in the _area_ . It s address is _number_ barton road
* I would like to book rooms for the same group of people for _number_ nights starting _weekday_ .
    - slot{"hotel_status": "booked"}
    - book_booking_hotel_reqmore_general: Booking was successful. Reference number is _reference_ . can i be of more assistance?   <!-- predicted: book_booking_hotel_inform_hotel: All right, I ve booked you a room at _hotel_name_ . The reference number is _reference_ . What else can I do for you? -->
* Yes I also need a taxi that will get me to the restaurant by the booked time please.
    - slot{"taxi_status": "booked"}
    - I booked a taxi for you. It s a _color_ _cartype_ . The contact number is _number_ . Is there anything else I can assist you with?
* that is it for today. have a great day
    - welcome_general: I m glad I could help.   <!-- predicted: bye_general: Thanks so much for visiting! Enjoy your trip! -->


## story_SNG0412
* Oh, yes I m hoping you can help me with finding a train departing out of _hotel_name_ .
    - slot{"train_status": "available"}
    - request_train: Certainly! Where would you like to go?   <!-- predicted: request_taxi: I d be happy to help you with a taxi, what is your destination departure and what time would you like to arrive leave? -->
* I need to go to _location_ .
    - slot{"train_status": "available"}
    - inform_train_request_train: There are plenty of trains going there. What day and time would you like to travel?   <!-- predicted: request_train: On what day will you be traveling? Do you prefer a specific time as well? -->
* I would like to leave on _weekday_ after_time_ after _time_ .
    - slot{"train_status": "available"}
    - I have a train leaving _hotel_name_ at _time_ , and arriving on _location_ at _time_ .
* What is the price on that train?
    - inform_train_reqmore_general: The price is _number_ pounds, payable at the station. May I help with anything else?   <!-- predicted: inform_train: The price would be _number_ pounds and the train ID is _reference_ . -->
* No, that was all I needed. Thank you so much for your help!
    - Thank you for contacting us. You have a great trip in _hotel_name_ .


## story_PMUL1046
* Where is the train that arrives at _time_ and leaves to _hotel_name_ ?
    - slot{"train_status": "available"}
    - request_train: What day do you wish to travel and where are you departing from?   <!-- predicted: inform_train_request_train: There s a train running every day leaving at _time_ and arriving at _time_ . Did you have a particular day in mind? -->
* I want to depart from Broxbourne on _weekday_ .
    - slot{"train_status": "available"}
    - _reference_ arrives in _hotel_name_ by _time_ . Would that work for you?
* Yes. Please book for _number_ people.
    - slot{"train_status": "booked"}
    - offerbooked_train_reqmore_general: Okay, tickets fro _number_ have been booked! Your reference number is _reference_ . Can I help you with anything else?   <!-- predicted: offerbooked_train: I have booked for you train _reference_ the total fee is _number_ _reference_ payable at the station .Reference number is _reference_ -->
* Thank you. Now I would like to party all night at a good night club. Can you help with that?
    - slot{"attraction_status": "available"}
    - inform_attraction: Yes, I can help you find a _attraction_type_ .   <!-- predicted: reqmore_general: Yes nice place. Did you need any info on it ? -->
* I would like _number_ in the _area_ .
    - slot{"attraction_status": "NA"}
    - nooffer_attraction: I m so sorry, I m not showing any nightclubs in the _area_ . Could I look in a different part of town for you?   <!-- predicted: inform_attraction_reqmore_general: There is a great _attraction_type_ on the _area_ side called Cineworld _attraction_type_ . The are located at _hotel_name_ leisure _attraction_type_ , clifton way. Their phone number is _number_ . Is there anything else? -->
* Okay are there any good colleges in that area?
    - slot{"attraction_status": "available"}
    - inform_attraction: Queens _attraction_name_ would fit that criteria. can I get you more info on it?   <!-- predicted: greet_general_inform_attraction_request_attraction: You re in luck! _hotel_name_ has a great number of museums. Did you have an area in mind? -->
* What s the entrance fee?
    - slot{"attraction_status": "available"}
    - The entrance fee is _number_ pounds. Did you need any more information?
* Yes, I also need the address and postcode please.
    - inform_attraction_reqmore_general: Sure! It s on Silver Street, and the postcode is _reference_ . Can I help you with anything else?   <!-- predicted: inform_restaurant: cb58jj is there postcode. Their address is _number_ Newmarket Road Fen Ditton -->
* Nothing more. Thank you for the train and _attraction_name_ information. Goodbye.
    - bye_general_welcome_general: you re welcome, enjoy your visit!   <!-- predicted: recommend_hotel: If price is not an issue, I recommend the _pricerange_ _hotel_name_ . If you want something cheaper, I recommend _hotel_name_ . -->


## story_PMUL0994
* I d like to take a train from _hotel_name_ on _weekday_ . Can you please show me the times?
    - slot{"train_status": "available"}
    - request_train: What is your destination?   <!-- predicted: inform_train_request_train: There are many trains to peterborough. What is your departure station and what time do you want to depart arrive? -->
* I am going to _location_ , and would like to arrive by _time_ .
    - slot{"train_status": "unique"}
    - _reference_ will get you there by _time_ . Do you need some seats booked?
* Yes. Can you please book _number_ seats?
    - slot{"train_status": "booked"}
    - Your booking was successful. Your total fee is _number_ payable at the station. Your reference number is _reference_ . Is there anything else we can do to assist you?
* I am also looking for a restaurant in the centre of town. I d like it to be _pricerange_ price range, please.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_restaurant: There are many wonderful restaurants in the centre, do you have a cuisine in mind?   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* Not really, pick something tasty for us and book a table, please! _time_ on that same day, same group.
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_inform_restaurant_reqmore_general: I booked you a table at _restaurant_name_ , a _food_type_ restaurant. Your reference number is _reference_ . Do you need anything else?   <!-- predicted: book_booking_restaurant: You are booked! Your table will be reserved for fifteen minutes and your reference number is _reference_ . -->
* No, that is all for now. Thank you for your help. goodbye
    - bye_general: Thank you for using our system.   <!-- predicted: bye_general_welcome_general: You re welcome. Thank you for calling. Enjoy your trip! -->


## story_MUL0570
* Hello, do you know of any points of interest in the centre of _hotel_name_ ?
    - slot{"attraction_status": "available"}
    - There are _number_ attractions in the center of town. What types are you interested in?
* I m not sure. What types of attractions are there?
    - inform_attraction: You could visit a _attraction_type_ or _attraction_name_ . There are also _number_ museums that are free of charge to enter.   <!-- predicted: inform_attraction_reqmore_general: I have _number_ _attraction_type_ attractions. _number_ are in the centre, with _number_ in the _area_ and _area_ . Are you interested in information about _number_ of them in a certain area? -->
* I would like to visit a _attraction_name_ . May I have the entrance fee and postcard?
    - slot{"attraction_status": "available"}
    - There is _attraction_name_ , which has a free entrance fee. Their postcode is cb23bu.
* Can I have information for a train departing from Ely? I m looking to arrive in _hotel_name_ by about _time_ on _weekday_ .
    - slot{"train_status": "available"}
    - inform_train: _reference_ will arrive around _time_ on _weekday_ if you re interested in that.   <!-- predicted: inform_train_request_train: There are more than _number_ trains to bishops Stratford, could you tell me what day you would like to leave, where you would like to leave from, and the times. -->
* I ll take it for just me what is the travel time, and the price please?
    - The travel time is _number_ minutes and the price is _number_ _reference_ .
* Great thank you I think I have all the information I need
    - slot{"train_status": "unique"}
    - offerbook_train: Would you like me to book that train for you?   <!-- predicted: inform_booking_hotel_inform_hotel: I found _hotel_name_ located at _number_ _hotel_name_ road. Would you like me to book that for you now? -->
* No thank you. Appreciate the help!
    - bye_general_welcome_general: You are welcome. Have a good day!   <!-- predicted: reqmore_general_welcome_general: You re very welcome. Is there anything else at all that I could assist you with? -->


## story_PMUL3785
* Can you help me find information on the _hotel_name_ ?
    - slot{"hotel_status": "available"}
    - inform_hotel_reqmore_general: That is a great _number_ star _hotel_type_ . It is _pricerange_ , but beautiful. What would you like to know?   <!-- predicted: request_taxi: Sure, I can do that. Do you know the name of the restaurant? Also, when would you like to be picked up and arrive by? -->
* i want to book it for _number_ nights
    - slot{"hotel_status": "available"}
    - Okay, what day would you like me to make the reservation for and for how many people?
* Book it starting from _weekday_ and it will be for _number_ people and I ll also need the reference number. We also need to find a place to eat.
    - slot{"hotel_status": "booked"}
    - Thee booking was successful and your reference number is _reference_ .
* Something classy nearby for dinner, preferably _food_type_ or _food_type_ cuisine?
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_restaurant: There are many _food_type_ restaurants. Were you wanting something _pricerange_ ?   <!-- predicted: inform_restaurant: I ve located the _restaurant_name_ for you. It serves _food_type_ food, it s in the _area_ area and is in the _pricerange_ price range. The phone number is _number_ . -->
* Yes I d like _number_ in the _pricerange_ range. If there s more than _number_ whichever you recommend will be fine.
    - slot{"restaurant_status": "available"}
    - recommend_restaurant: I would recommend _restaurant_name_ , it is an _pricerange_ _food_type_ restaurant at _number_ Norfolk Street.   <!-- predicted: select_restaurant: The restaurants are _restaurant_name_ , _restaurant_name_ and _restaurant_name_ . -->
* Okay I need a reservation for _weekday_ , _number_ people at _time_ . Can you please include the reference number?
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_reqmore_general: I have managed to book your table for _number_ on _weekday_ . Your reference number is _reference_ . Is there anything else I can help you with?   <!-- predicted: book_booking_train_reqmore_general: Your reservation is set. The reference number is _reference_ . Can I help you with anything else? -->
* thank you very much
    - It was my pleasure. Feel free to get in touch if you need anything else.


## story_SNG0600
* I m looking for a specific restaurant. It s called _restaurant_name_ . Can you help with this?
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_inform_restaurant: Sure can. _restaurant_name_ is an _pricerange_ _food_type_ restaurant in the _area_ part of town. Would you like a reservation?   <!-- predicted: inform_booking_restaurant_recommend_restaurant: _restaurant_name_ is an _food_type_ restaurant in the centre. It s _pricerange_ , but I hear it s great. Would you like me to book it for you? -->
* Yes for _number_ people at _time_ on a _weekday_ . I will need a reference number as well.
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_reqmore_general: I ve made the reservation and the reference number is _reference_ . What else can I help you with?   <!-- predicted: book_booking_restaurant: Your table for _number_ at _restaurant_name_ at _time_ this _weekday_ was successful. The table will be reserved for _number_ minutes. Your Reference number is _reference_ . -->
* I think that takes care of everything, thanks!
    - Oh, it was my pleasure. I m here if you need anything else.
* Thank you. Have a great day!
    - bye_general: You have a great day!   <!-- predicted: reqmore_general: Ok. Do you need anything else then? -->


## story_SNG0867
* I d like to find a _pricerange_ place to stay.
    - slot{"hotel_status": "available"}
    - I can certainly help you with that. We have _number_ listings for _pricerange_ lodgings. Do you have any other requirements?
* I would like for it to be located in the center of town.
    - slot{"hotel_status": "available"}
    - inform_hotel_select_hotel: Sure. I found _number_ guesthouses. _number_ with _number_ stars and _number_ with _number_ stars. Do you have a preference?   <!-- predicted: inform_hotel: We have _number_ option for you. We have the _hotel_name_ and the lovell _hotel_type_ . Both have your commendations you want. -->
* No, I don t have a preference. Do those places have wi-fi?
    - slot{"hotel_status": "unique"}
    - Yes, they both do. The _hotel_name_ B&B is our inexpensive _number_ star guesthouse. Would you like me to see if I could book you room?
* I am not ready to book yet. Thanks for the information.
    - reqmore_general: You are very welcome! Is there anything else I can assist you with?   <!-- predicted: request_hotel: Name of _hotel_type_ please. I want to be sure to get correct destination. -->
* That is all! Thanks!
    - bye_general: Have a great day!   <!-- predicted: inform_booking_hotel_inform_hotel: Yes, all of the hotels and guesthouses are able to accommodate _number_ guests per booking. Are you ready to book? If so, I just need a little more info. -->


## story_SNG01873
* I need to be picked up from _attraction_name_ hut city centre after _time_
    - slot{"taxi_status": "available"}
    - request_taxi: Where will you be heading to ?   <!-- predicted: request_train: Sorry, I m confused - are you leaving from _hotel_name_ or is _hotel_name_ your destination? If it is your destination, what is your departure site? -->
* I am headed to _hotel_name_ .
    - slot{"taxi_status": "booked"}
    - Great. Your booking is complete. A _color_ _cartype_ will pick you up and can be reached by dialing _number_
* Thanks. That takes care of everything for me. Bye!
    - Have a great day and thank you for contacting us.


## story_PMUL0768
* I need a place to dine in the centre of town, serving _food_type_ food.
    - slot{"restaurant_status": "NA"}
    - I cannot find an _food_type_ restaurant in that area, would you like me to look up another area or cuisine type?
* Can you check another area?
    - slot{"restaurant_status": "NA"}
    - There are none in town. Is there another type of food you would like?
* Sure, how about _food_type_ ? _pricerange_ prices in the centre is necessary.
    - slot{"restaurant_status": "available"}
    - Restaurant _number_ _number_ is located on DeVere University Arms Regent Street City Centre.
* I need a table for _number_ on _weekday_ . At _time_ .
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_reqmore_general: I have booked it Reference number is _reference_ . Can I help you with anything else?   <!-- predicted: book_booking_restaurant: Here is your booking information Booking was successful. The table will be reserved for _number_ minutes.Reference number is _reference_ . -->
* Thank you very much for your time. Have a nice day!
    - bye_general: Thank you for contacting us today. Have a nice day.   <!-- predicted: reqmore_general: You re very welcome! Don t hesitate to call again if you need anything else. -->


## story_PMUL4034
* I am planning a trip in _hotel_name_ .
    - slot{"hotel_status": "available"}
    - reqmore_general: sure, what can i help you find?   <!-- predicted: greet_general: Great! I can help you with any tourist information you may need. -->
* I need a train from _location_ to _hotel_name_ on _weekday_ , please. I need to get there at about _time_ .
    - slot{"train_status": "unique"}
    - _reference_ will arrive by _time_ . Would you like to book a seat?
* Can you book it for me and get a reference number ?
    - How many tickets do you need?
* I need _number_ tickets.
    - slot{"train_status": "booked"}
    - Booking was successful, the total fee is _number_ _reference_ payable at the station .Reference number is _reference_ .what else do i do for you?
* Yes, I d like to stay at _hotel_name_ once we get to town for _number_ nights.
    - slot{"hotel_status": "available"}
    - request_booking_hotel: What day would you like to begin your stay? And for how many guests?   <!-- predicted: book_booking_hotel: Since you mentioned a _hotel_type_ rather than a guesthouse, I ve booked you at the _hotel_name_ , but just let me know if you prefer the other. Your reference is _reference_ . -->
* I d like to stay on _weekday_ , _number_ nights, _number_ people. I also need a reference number.
    - slot{"hotel_status": "booked"}
    - book_booking_hotel_reqmore_general: You are all set! Your reference number for your booking is _reference_ . Is there anything else I can help you with?   <!-- predicted: book_booking_hotel: Okay, your booking was successful! We have you booked at the _hotel_name_ . Your reference number is _reference_ . -->
* That is all. Thanks so much!
    - bye_general_welcome_general: Your welcome if you have any query. please contact us   <!-- predicted: bye_general: Okay, great! have a great trip! -->


## story_MUL1899
* I need some time in the sun, can you help me find a _attraction_type_ to visit?
    - slot{"attraction_status": "available"}
    - inform_attraction: _attraction_name_ is in the _area_ and is free admission.   <!-- predicted: inform_attraction_reqmore_general: I have _number_ _attraction_type_ attractions. _number_ are in the centre, with _number_ in the _area_ and _area_ . Are you interested in information about _number_ of them in a certain area? -->
* Can I get the phone number and address?
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: Their address is Cherry Hinton Hall, Cherry Hinton Road. The phone number to reach them is _number_ . Is there any other info you need?   <!-- predicted: greet_general_inform_hotel_reqmore_general: Of course! The address of the _hotel_name_ is kingfisher way, hinchinbrook business _attraction_type_ , huntingdon and it s phone number is _number_ , would you like anything else? -->
* Yeah, I also need to find a train to hop on for _weekday_ .
    - slot{"train_status": "available"}
    - request_train: Where will you be departing from and traveling to?   <!-- predicted: inform_train_request_train: There are _number_ trains traveling on _weekday_ . Where will you be departing from and where is your destination? -->
* I will be departing from _location_ and will be traveling to _hotel_name_ .
    - slot{"train_status": "available"}
    - What time would you like to leave by or arrive by?
* I would like to arrive by _time_ in _hotel_name_ .
    - slot{"train_status": "unique"}
    - _reference_ will arrive in _hotel_name_ by _time_ , would you like to book a ticket?
* No, thank you. What is the price?
    - inform_train_reqmore_general: The price for the train that will arrive at _time_ and leaves at _time_ is _number_ pounds. Is there anything I can assist you with?   <!-- predicted: inform_train: Sure, it takes _number_ minutes and costs _number_ pounds. -->
* No, that was everything I needed, thank you for your help.
    - greet_general: Great, glad I could help!   <!-- predicted: bye_general_welcome_general: So happy to be of service, and thanks for using _hotel_name_ TownInfo centre today. Have a wonderful day! -->


## story_MUL1466
* I m currently planning my trip to _hotel_name_ , but need some help finding a certain restaurant.
    - Sure, I can help you with that. What type of cuisine are you looking for?
* Actually, I m looking for some info on _restaurant_name_ restaurant. Can you tell me about them?
    - slot{"restaurant_status": "unique"}
    - Absolutely! They are a great _food_type_ restaurant in the centre of town. They are on the _pricerange_ side. Would you like help in reserving a table?
* I need their address, and postcode.
    - inform_restaurant: They are at _number_ Mill Road City Centre, postcode cb12as   <!-- predicted: inform_restaurant_request_booking_restaurant: Their postcode is cb11lh and if you want a reservation just let me know the time, party size, and day and I ll make it for you. -->
* Thanks. Can you also help me find a train to Bishops Stortford?
    - slot{"train_status": "available"}
    - inform_train_request_train: There are more than _number_ trains to bishops Stratford, could you tell me what day you would like to leave, where you would like to leave from, and the times.   <!-- predicted: request_train: Sure! When are you wanting to travel, where are you leaving from, where would you like to go and what time? -->
* I am leaving _hotel_name_ on _weekday_ , can you please tell me the travel time on that ride?
    - slot{"train_status": "unique"}
    - Sure, it is a _number_ minute trip. Would you like a ticket?
* I need to leave after _time_ also.
    - slot{"train_status": "available"}
    - inform_train: The _reference_ departs _hotel_name_ at _time_ , would that suit you?   <!-- predicted: request_train: May I ask for your departure city? -->
* No that s all I needed. Thanks for your help.
    - You re very welcome! Thank you!


## story_MUL0492
* I am looking for a theatre to visit while in _hotel_name_ . Preferably _number_ in the centre of town.
    - slot{"attraction_status": "available"}
    - recommend_attraction: Would you like to try the _hotel_name_ arts theatre?   <!-- predicted: inform_attraction_reqmore_general: I have _number_ _attraction_type_ attractions. _number_ are in the centre, with _number_ in the _area_ and _area_ . Are you interested in information about _number_ of them in a certain area? -->
* That sounds great! could you tell me how much the entrance fee would cost?
    - slot{"attraction_status": "available"}
    - Unfortunately I do not have that information in my system. I could give you their phone number, though, if you like.
* Could you please find the entrance fee for me? I am unable to make the phone call right now.
    - inform_attraction: Unfortunately the entrance fee for the _hotel_name_ arts theatre is not in the system right now.   <!-- predicted: inform_attraction_reqmore_general: The Fitzwilliam _attraction_name_ is located in the area of centre. Their phone number is _number_ . There is no entrance fee. Is there anything else I can do for you? -->
* Okay. I am looking for a train that departs on _weekday_ from _location_ and goes to _hotel_name_ . Arrival by _time_ .
    - slot{"train_status": "unique"}
    - inform_train_offerbook_train: _reference_ arrives at _time_ , after leaving at _time_ . Would you like this _number_ ?   <!-- predicted: inform_train_select_train: There is a train that arrives at _time_ the closest before that is a train that arrives at _time_ . Which _number_ would you like? -->
* What is the price?
    - inform_train_request_train: The price will be _number_ pounds. How many tickets would you like?   <!-- predicted: inform_train_offerbook_train: Sure. It takes approximately _number_ minutes and costs _number_ pounds per ticket. Would you like me to book it for you? -->
* I just need _number_ ticket. Can you book that for me please?
    - slot{"train_status": "booked"}
    - offerbooked_train_reqmore_general: Absolutely. Here is your reference number _reference_ . Can I help you with anything else today?   <!-- predicted: offerbooked_train: I have booked for you train _reference_ the total fee is _number_ _reference_ payable at the station .Reference number is _reference_ -->
* No, that s all I need. Thank you for your help.
    - welcome_general: You re welcome, have a great day!   <!-- predicted: bye_general_welcome_general: You re welcome. I hope you have a great trip! Goodbye. -->


## story_SNG02207
* I need to book a tax departing from _location_ .
    - slot{"taxi_status": "available"}
    - request_taxi: What is your destination and when would you like to depart?   <!-- predicted: request_train: Ok, just tell me what day and time and I will be able to tell you what is available. -->
* I m going to broxbourne train station and i need to arrive by _time_
    - slot{"taxi_status": "booked"}
    - I have you in a _color_ _cartype_ , _number_ is the number to call if you need to speak to them.
* Wonderful, thanks for your help.
    - reqmore_general: My pleasure. Do you need any other assistance while in town?   <!-- predicted: bye_general_welcome_general: You re welcome, farewell! Text back anytime! -->
* No thank you.
    - reqmore_general: Okay. Please let us know if there s anything else we can do for you during your visit to _hotel_name_ .   <!-- predicted: welcome_general: you re welcome, thank you for using our system. -->


## story_MUL0383
* I would like a train to _hotel_name_ that leaves after _time_ .
    - slot{"train_status": "available"}
    - There are very many trains that fit your requirements, where are you leaving from and what day would you like to leave?
* I d like to leave on _weekday_ from Stansted Airport.
    - slot{"train_status": "available"}
    - Ok, there are _number_ trains that fit those requirements, can you tell me what time you would like to arrive by?
* I don t mind we can get there any time.
    - slot{"train_status": "unique"}
    - _reference_ leaves at _time_ and arrives by _time_ , would you like me to book a seat for you?
* Yes can you give me the travel time?
    - slot{"train_status": "booked"}
    - offerbooked_train: Sure, I was able to book your seat and your reference number is _reference_ which is payable at the station. The travel time is _number_ minutes.   <!-- predicted: inform_train_reqmore_general: Certainly. The travel time is _number_ minutes and the price is _number_ pounds. Is there anything else I can assist with? -->
* Thanks! Also, could you tell me if there are any places in the center of town that serve _food_type_ ? Something _pricerange_ would be great.
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_inform_restaurant_recommend_restaurant: There are _number_ . How about _restaurant_name_ ? Should I book you a table?   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* Yes that sounds great, I need a table for _number_ at _time_ on _weekday_ please.
    - slot{"restaurant_status": "NA"}
    - nobook_booking_restaurant_request_booking_restaurant: Unfortunately that time is not available do you have another time you d like to try?   <!-- predicted: inform_restaurant_nobook_booking_restaurant_request_booking_restaurant: I m sorry, but I attempted reservations at your specified time at all _number_ restaurants, and none have availability at that time. Would you like to try a different time? -->
* Okay, is there an available time at _time_ ? Also, can I get a reference number?
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_reqmore_general: That booking was successful. Your reference number is _reference_ . Is there anything else I can do for you?   <!-- predicted: offerbooked_train_reqmore_general: Sure, the train is actually number _reference_ and your reference number is _reference_ . The price will be _number_ _reference_ payable at the station. Is there anything else today? -->
* I think that s everything, thank you
    - bye_general_welcome_general: You are welcome. Have a nice day.   <!-- predicted: bye_general: Thank you, Enjoy your day, goodbye. -->


## story_MUL2063
* Hello I m looking for a _pricerange_ _hotel_type_ that includes wifi.
    - slot{"hotel_status": "available"}
    - inform_hotel: I actually have just _number_ located in the _area_ that is _pricerange_ . It is _hotel_name_ . They are _number_ -star rated and offer free parking and wifi. Can I book you?   <!-- predicted: inform_hotel_request_hotel: I have _number_ hotels in town matching that requirement ranging from _number_ to _number_ stars guest houses and hotels. Do you have a preference for the area? -->
* Great. I just needed to know _number_ would be available if I decide to make the trip. You ve been a great help. Thanks. Bye.
    - bye_general: Thank you for contacting _hotel_name_ TownInfo centre. I hope you have a pleasant trip! Goodbye!   <!-- predicted: inform_booking_restaurant_inform_restaurant_reqmore_general: They serve _food_type_ food. Do you need any other information, or help making a booking? -->
* Hold on, let me go ahead and book the _hotel_type_ for _number_ people starting on _weekday_ for _number_ nights. Please send me the reference number once reservation is made.
    - slot{"hotel_status": "booked"}
    - book_booking_hotel_reqmore_general: I have reserved _hotel_name_ for _number_ people for _number_ nights beginning _weekday_ . Your reference number is _reference_ . Can I help with anything else?   <!-- predicted: book_booking_hotel_inform_hotel_reqmore_general: You are booked at the _hotel_name_ B & B. It is _pricerange_ , with wifi and parking included. Your reference number is _reference_ . Is there anything else? -->
* I would also like to see if I could catch a train from _location_ to _hotel_name_ .
    - slot{"train_status": "available"}
    - inform_train: I show _number_ possible trains. What day were you looking for?   <!-- predicted: inform_train_request_train: There are a total of _number_ trains traveling from _location_ to _hotel_name_ . Is there a particular day that you would like to travel on? -->
* I want to arrive _weekday_ by _time_ , is that possible.
    - slot{"train_status": "unique"}
    - Train _reference_ looks like a good fit. Would you like me to book it for you?
* No thank you. Could you give me it s departure time?
    - inform_train_reqmore_general: _time_ is its departure time. Could I help you with anything else?   <!-- predicted: inform_train: _reference_ will arrive in _hotel_name_ _weekday_ by _time_ , it will depart peterborough at _time_ . Does this suit your needs? -->
* That is all for now. Thanks
    - inform_train_reqmore_general: Just in case you want to arrive closer to _time_ , _reference_ leaves _location_ at _time_ and arrives in _hotel_name_ by _time_ . Please let me know if you need anything else.   <!-- predicted: greet_general: Okay, great. Have a wonderful trip. Goodbye. -->
* I sure will, thanks again!
    - No problem. Have a great day!


## story_PMUL4930
* Can you tell me about any _food_type_ restaurants in the centre?
    - slot{"restaurant_status": "NA"}
    - inform_restaurant_nooffer_restaurant_request_restaurant: I m sorry I do not have any _food_type_ restaurants in _hotel_name_ . Is there another type of cuisine you might be interested in?   <!-- predicted: nooffer_restaurant_request_restaurant: I m sorry, but I could not find any listings for restaurants serving _food_type_ style food. Do you have any other favorite types of cuisines? -->
* How about _number_ that serves _food_type_ food?
    - slot{"restaurant_status": "available"}
    - inform_restaurant_select_restaurant: We have several in the center, and _number_ in the _area_ . They are in assorted price ranges. Do you have any preferences?   <!-- predicted: inform_restaurant: I found _number_ options for you _restaurant_name_ at Regent Street City Centre, _restaurant_name_ at _number_ Mill Road City Centre, and _restaurant_name_ at _number_ _hotel_name_ Road City Centre -->
* Whatever you recommend, please book me for _number_ people at _time_ on _weekday_ .
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant: I have made a booking for _restaurant_name_ . The table will be reserved for _number_ minutes.Reference number is _reference_ .   <!-- predicted: book_booking_restaurant_reqmore_general: I was able to book a table for you. The Reference number is _reference_ . Is there anything else you need? -->
* I also need to find a _number_ star room.
    - slot{"hotel_status": "available"}
    - recommend_hotel: How about the _hotel_name_ ? They are moderately priced and have both internet and parking.   <!-- predicted: inform_hotel_request_hotel: I was able to get _number_ results for what you are looking for, is there a certain price range you would like? -->
* That sounds great. Could you give me the address please?
    - slot{"hotel_status": "unique"}
    - Sure, the address is _number_ chesterton road post code cb41er. Would you like a reservation?
* No thanks. I do want a taxi though to go from the _hotel_type_ to the restaurant, arriving by my reservation time. Tell me the car type and contact number.
    - slot{"taxi_status": "booked"}
    - I ve booked a _color_ _cartype_ , phone number _number_ . Will that be all?
* That is everything, thanks for you help.
    - Great. Enjoy your stay!


## story_MUL1417
* I m looking for a train to _hotel_name_ that leaves on _weekday_ .
    - slot{"train_status": "available"}
    - The _location_ travels to _hotel_name_ on _weekday_ . Where are you leaving from?
* I m leaving from Peterborough and want to arrive by _time_ .
    - slot{"train_status": "unique"}
    - The _reference_ leaves at _time_ and arrives by _time_ . Would you like me to book it?
* Can you tell me the price of the ticket please?
    - inform_train: Sure - tickets from Peterborough to _hotel_name_ are _number_ _reference_ each.   <!-- predicted: inform_train_reqmore_general: Sure, _reference_ is a _number_ minute trip and each seat costs _number_ pounds. Can I help you with anything else today? -->
* Great I also am looking for a restaurant called _restaurant_name_
    - slot{"restaurant_status": "available"}
    - inform_restaurant: _restaurant_name_ is an _food_type_ restaurant in the _pricerange_ price range.   <!-- predicted: inform_restaurant_request_restaurant: There are a total of _number_ _pricerange_ restaurants located in town. Is there a specific area you are going to be in? -->
* I would like to book _restaurant_name_ for _number_ at _time_ on _weekday_ , please.
    - slot{"restaurant_status": "NA"}
    - That time is not available. What other time would work for you?
* How about _time_ ?
    - slot{"restaurant_status": "booked"}
    - I was able to book you for _time_ on _weekday_ . Tables are held for _number_ minutes. The reference is _reference_ .
* Thanks! That s all I need. Goodbye!
    - It was a pleasure. Have a nice day. Goodbye.


## story_MUL2378
* Hello, I am looking for a _food_type_ restaurant in the centre. Could you help me with that?
    - slot{"restaurant_status": "unique"}
    - I have _number_ restaurant name _restaurant_name_ in the _pricerange_ price range. would you like me to book it?
* Are there any other choice? If not I would like to get a table on Wensday at _number_ for _number_ please.
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_inform_restaurant: I looked and this was the only restaurant serving _food_type_ food. I have booked you a table. The table will be reserved for _number_ minutes. Ref _reference_ . Any thing else?   <!-- predicted: offerbooked_train_reqmore_general: I have made the booking and here is the information-Booking was successful, the total fee is _number_ _reference_ payable at the station .Reference number is _reference_ Anything else I can help you with? -->
* Are there any places to go in the same area as the restaurant?
    - slot{"attraction_status": "available"}
    - There are dozens of places to go in city centre. What type of attraction are you interested in today?
* I don t really mind, as long as it is near the restaurant. What looks good to you?
    - recommend_attraction_select_attraction: I would like to suggest _attraction_name_ located in the centre. Is that okay?   <!-- predicted: inform_restaurant: There is _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _restaurant_name_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _area_ _food_type_ , _food_type_ , _food_type_ , and _food_type_ food available in the centre. -->
* Yes that is fine can you please provide the postcode?
    - slot{"attraction_status": "available"}
    - inform_attraction: The postcode is cb58bs. Is there anything else I can help with?   <!-- predicted: inform_attraction_reqmore_general: I can tell you that Byard Art is located at _number_ King s Parade, postcode cb21sj. Does that help? -->
* I also need a taxi to go between them and need it to arrive at the restaurant by the booked time.
    - slot{"taxi_status": "booked"}
    - I have booked a cab to take you to the restaurant when you leave _attraction_name_ . The booked car type is a _color_ _cartype_ .The contact number is _number_ .
* Thanks so much, that s all I need today!
    - greet_general: My pleasure. Have a great day.   <!-- predicted: bye_general_welcome_general: You re very welcome. Have a great day and text us back anytime! -->
* Goodbye again, thanks for your help.
    - greet_general: It s no problem, contact us again any time.   <!-- predicted: bye_general: My pleasure! Enjoy your trip. -->


## story_MUL1088
* I am coming to _hotel_name_ and would like to see some _attraction_type_ . Do you have any located in the centre?
    - slot{"attraction_status": "available"}
    - inform_attraction_recommend_attraction: Yes, there are _number_ places located in the centre. I recommend the _attraction_name_ on Jesus Lane.   <!-- predicted: inform_hotel_request_hotel: There are _number_ hotels which are _number_ stars, _number_ in the _area_ and _number_ in the centre. Is there an area which you prefer? -->
* Thanks! What s the entrance fee?
    - There is no entrance fee, it is free. Is there anything else I can help you with?
* I d like to find a guesthouse to stay at. I want it to be nice, so I d like an _pricerange_ _number_ .
    - slot{"hotel_status": "NA"}
    - inform_hotel_nooffer_hotel_request_hotel: It seems like all of my guesthouses are in different price ranges. No _pricerange_ ones are listed. Can I interest you in a different price range?   <!-- predicted: inform_hotel_nooffer_hotel: There are no hotels that meet that criteria in the _area_ but we do have _number_ moderately priced guesthouses available. Would _number_ of those work? -->
* Well then I need a _hotel_type_ that has free parking and a _number_ star rating.
    - slot{"hotel_status": "available"}
    - inform_hotel: I ve found _number_ hotels matching your preferences. The _hotel_name_ is in the _pricerange_ price range and is located in the centre of town if you are interested.   <!-- predicted: inform_hotel_request_hotel: I have _number_ options for you, located all over town. Do you have a certain area or price range in mind? -->
* I would like a guesthouse in the _pricerange_ price range that has _number_ stars and includes free parking.
    - slot{"hotel_status": "available"}
    - I have _number_ total guesthouses that meet your needs. They are located in the _area_ , _area_ , and _area_ . Do you have a preference?
* Can you recommend _number_ ?
    - inform_hotel: _hotel_name_ seems like a nice place because it is the first _number_ on my list how about that _number_ its probably not too shabby   <!-- predicted: recommend_hotel: If price is not an issue, I recommend the _pricerange_ _hotel_name_ . If you want something cheaper, I recommend _hotel_name_ . -->
* OK, that _number_ sounds great!
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel: Would you like me to book it for you?   <!-- predicted: inform_booking_hotel_inform_hotel: The _hotel_name_ is at _number_ Chesterton Road, and their postcode is cb41er. Would you like to book a room or are you just looking for information right now? -->
* Yes, book it for _number_ people for _number_ nights starting _weekday_ .
    - slot{"hotel_status": "NA"}
    - Unfortunately the booking was not successful.
* What if we try _number_ nights?
    - slot{"hotel_status": "booked"}
    - Your booking was successful with a reference number of _reference_ . Can I help you with anything else?
* Thanks great. Also I need to have the phone number for _attraction_name_ on Jesus Lane.
    - Sure _attraction_name_ s phone number is _number_ . Anything else?
* Not at the moment. Thank you.
    - Thank you for using our service. Have we met all of your needs today?
* Yes, you have. Thank you. Have a good day.
    - bye_general: You as well! Good bye!   <!-- predicted: reqmore_general: You re very welcome! Don t hesitate to call again if you need anything else. -->


## story_PMUL3557
* I d like to get a bite to eat in the _area_ part of town.
    - slot{"restaurant_status": "available"}
    - request_restaurant: Okay! What kind of cuisine would you like to eat?   <!-- predicted: inform_restaurant: The top _number_ places serving _food_type_ cuisine are _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Would you like more options? -->
* I would really like _food_type_ food.
    - slot{"restaurant_status": "available"}
    - How about _restaurant_name_ that serves _food_type_ food that is in the _pricerange_ price range?
* Do you have anything _pricerange_ ?
    - slot{"restaurant_status": "available"}
    - select_restaurant: Yes! Would you like to try _restaurant_name_ , or _restaurant_name_ ?   <!-- predicted: nooffer_restaurant: Sorry, I couldn t find any food of that type. -->
* _restaurant_name_ would be great. Can you book a table for _number_ at _time_ on _weekday_ ?
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_reqmore_general: Yes! I ve got your table booked, they ll hold it for _number_ minutes. Your reference number is _reference_ . Can I help you with anything else?   <!-- predicted: book_booking_restaurant: I just completed your booking. The table will be reserved for _number_ minutes and the reference number is _reference_ . Is there anything else I can help you with? -->
* I am looking for a place called _attraction_name_ what area in the city is that located?
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: It is a theatre located in the _area_ . Would you like information for it?   <!-- predicted: inform_attraction: That s a great choice! It is an _attraction_type_ attraction in the centre of town at market square, postcode cb23pq. The phone number is _number_ and the entrance fee is _number_ pounds. -->
* No, that was all I needed. But I could use a taxi from _attraction_name_ to _restaurant_name_ by _time_ .
    - slot{"taxi_status": "booked"}
    - Okay. Your booking was completed. The car type is _color_ _cartype_ . The contact number is _number_ .
* That is all I need, thank you.
    - You re welcome. Have a great day!


## story_MUL1055
* I am looking for a place to go while in _hotel_name_ . I would like something to do with boats? Do you have that?
    - slot{"attraction_status": "available"}
    - inform_attraction_request_attraction: There are _number_ different locations related to _attraction_name_ , is there any specific area you re looking to go to?   <!-- predicted: inform_restaurant_request_restaurant: We have several options available to you. What type of cuisine would you prefer? We have _food_type_ , _food_type_ , _food_type_ , and _food_type_ as options. -->
* No there is not, just please provide me with the address of _number_ that you recommend.
    - slot{"attraction_status": "available"}
    - The _hotel_name_ Punter, the address is 251a Chesterton Road, post code cb41as. Would you like to know any more info on boats in _hotel_name_ ?
* I m looking for a place to stay. I prefer a guesthouse that s _pricerange_ .
    - slot{"hotel_status": "NA"}
    - nooffer_hotel: There are not any _pricerange_ guesthouses in _hotel_name_ . Would a moderately priced guesthouse suffice?   <!-- predicted: inform_hotel_nobook_booking_hotel_request_booking_hotel: Sorry, the _hotel_name_ is not able to accomodate you either. I checked with the other moderately priced _number_ star lodgings with free wifi, and none have those dates available. Will any other stay work for you? -->
* No. I really need an _pricerange_ _number_ with _number_ stars. I don t care about the area. Can you check again for me?
    - slot{"hotel_status": "NA"}
    - inform_hotel_nooffer_hotel: Unfortunately there are no guesthouses that match your request. If you are willing to stay at a _hotel_type_ , I have _number_ _pricerange_ _number_ star options.   <!-- predicted: nobook_booking_hotel_request_booking_hotel: I m sorry, _hotel_name_ is unavailable for those nights. Would you like to try another day or just _number_ night instead? -->
* Do you have _pricerange_ guesthouse with _number_ stars available?
    - slot{"hotel_status": "available"}
    - inform_hotel: We have _number_ guesthouses that is all in the _pricerange_ price range. All have free internet and parking. _number_ in the eastside, _number_ _area_ , and _number_ centre.   <!-- predicted: inform_hotel_recommend_hotel_select_hotel: If you like guesthouses there are a lot more options for you. I could recommend _hotel_name_ , they re moderately priced but rated _number_ stars. Does that sound good? -->
* Can you book the _number_ in the centre for _number_ people for _number_ nights starting _weekday_ ?
    - slot{"hotel_status": "NA"}
    - Unfortunately the _hotel_name_ guesthouse is unavailable for that date range. Would you like to see if another day is available or book for a shorter stay?
* Can you try booking for _number_ night, instead?
    - slot{"hotel_status": "booked"}
    - book_booking_hotel: Booking was successful. Your reference number is _reference_ .   <!-- predicted: book_booking_hotel_recommend_hotel: I would recommend the _hotel_name_ , which has what you need. Your booking reference number is _reference_ . Your _number_ night stay will begin _weekday_ . Thank you! -->
* I also need to arrange for a taxi to leave from the _hotel_type_ and get to _hotel_name_ Punter.
    - slot{"taxi_status": "available"}
    - What time do you need the taxi?
* I want to leave the _hotel_type_ by _time_ .
    - slot{"taxi_status": "booked"}
    - I have confirmed booking your taxi, a _color_ _cartype_ will be picking you up.
* Can I get a contact number for that?
    - inform_taxi: Their number is _number_ .   <!-- predicted: inform_taxi_reqmore_general: Their contact number is _number_ . Do you need any further assistance? -->
* Thank you very much for all your help.
    - greet_general: No problem. Glad to help.   <!-- predicted: bye_general: Have a great trip! Thank you for contacting us for all your booking needs. Enjoy your trip! -->


## story_PMUL0076
* Hi I am looking for a restaurant in the centre of town serving _food_type_ food.
    - slot{"restaurant_status": "available"}
    - greet_general_inform_restaurant_select_restaurant: That s great! There are several _food_type_ restaurants near the city centre. Are you looking for a budget conscious option or are you comfortable with a more _pricerange_ place?   <!-- predicted: inform_restaurant_request_restaurant: There are a total of _number_ different _food_type_ restaurants in the centre of town. Is there a particular price you are looking for? -->
* A _pricerange_ option please.
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_select_restaurant: We have mahal of _hotel_name_ , the ghandi and _restaurant_name_ , do you want me to book you for _number_ of those?   <!-- predicted: inform_booking_restaurant_recommend_restaurant: I would recommend _restaurant_name_ . It is an _pricerange_ restaurant in the center. Would you like to book a reservation? -->
* Yes please for _number_ people at _time_ on _weekday_ .
    - slot{"restaurant_status": "booked"}
    - You are all set. They will hold the table for _number_ minutes and your reference number is _reference_
* Thank you, appreciate your service.
    - No problem. Is there anything else I can help you with?
* I am also looking for a _hotel_type_ .
    - slot{"hotel_status": "available"}
    - inform_hotel_select_hotel: We have lots of great hotels. Would you like to stay with the centre part of town or some other area?   <!-- predicted: inform_hotel_request_hotel: I show _number_ hotels in the _area_ , _number_ is _pricerange_ and _number_ is _pricerange_ . I also show _number_ _pricerange_ _number_ star _hotel_type_ in the _area_ . Which area do you prefer? -->
* Yes, I would love to stay at a _hotel_type_ in the centre of town. I need free parking, free wifi, and a star rating of _number_ .
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel_recommend_hotel: The _hotel_name_ matches your criteria. Would you like me to book it for you?   <!-- predicted: inform_booking_hotel_inform_hotel_recommend_hotel: All the _number_ hotels are _number_ star hotels. I recommend the _hotel_name_ or the _hotel_name_ . Should I book _number_ of those for you and your party? -->
* yeah, that sounds good.
    - slot{"hotel_status": "available"}
    - request_booking_hotel: For how many people and how many days?   <!-- predicted: request_hotel: Did you want the _hotel_type_ to be in the centre area, also? -->
* Is that a _hotel_type_ ? And what is the price range?
    - inform_hotel: This is a _pricerange_ _hotel_type_   <!-- predicted: inform_train: It is _number_ pounds per person. -->
* That sounds great what is their postcode?
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel_inform_hotel_request_booking_hotel: The postcode is _reference_ . Are you still interested in booking a room? If so, I ll need to know how many people will be staying and for how many days.   <!-- predicted: inform_restaurant_request_booking_restaurant: Their postcode is cb11lh and if you want a reservation just let me know the time, party size, and day and I ll make it for you. -->
* You ve been great. That s all I need for tonight. Thank you. Goodbye.
    - reqmore_general_welcome_general: If you need reservations in the future, please let me know. Thank you   <!-- predicted: inform_booking_hotel_inform_hotel: Yes, all of the hotels and guesthouses are able to accommodate _number_ guests per booking. Are you ready to book? If so, I just need a little more info. -->


## story_MUL0849
* Can you help me find a place i am looking for? Its name is the _attraction_name_ .
    - slot{"attraction_status": "available"}
    - inform_attraction: Sure, the address is between Victoria Road and the River, the postcode is cb43px. Would you like their phone number for directions?   <!-- predicted: inform_attraction_request_attraction: There are _number_ museums in _hotel_name_ , would you like to know of any in a specific area, or would you like a recommendation? -->
* Great, thank you, and to be sure, this is actually a pool, correct?
    - Yes, it is listed as a _attraction_name_ in the northern part of town. Is there anything else I can help you find today?
* Yes, I m also looking for a restaurant Can you help me with that, too?
    - request_restaurant: Sure, what is your price range?   <!-- predicted: request_hotel: Can you please tell me what type of place and if you have any preferences? -->
* _pricerange_ , it should be in the centre and serve _food_type_ food.
    - slot{"restaurant_status": "available"}
    - inform_restaurant: I have found _number_ _food_type_ Restaurants in Centre; _restaurant_name_ , Tang _food_type_ , HK _food_type_ , and _restaurant_name_ . Would you like there phone numbers, or address?   <!-- predicted: inform_restaurant_select_restaurant: I have the _restaurant_name_ which serves _food_type_ . I also have _restaurant_name_ that serves _food_type_ food. Which would you prefer? -->
* I am more interested in booking whichever will accept a table of _number_ at _time_ this _weekday_ ?
    - slot{"restaurant_status": "NA"}
    - nobook_booking_restaurant_request_booking_restaurant: Sir, I m afraid none of those restaurants have a table available for that time period. Do you want to try a different day or time?   <!-- predicted: inform_restaurant_nobook_booking_restaurant_request_booking_restaurant: I m sorry, but I attempted reservations at your specified time at all _number_ restaurants, and none have availability at that time. Would you like to try a different time? -->
* Yes, could you try _time_ instead please?
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_inform_restaurant_reqmore_general: I was able to book you for that time at the _restaurant_name_ located at _number_ St. Johns Street City Centre. Your reference number is _reference_ . Is there anything else?   <!-- predicted: book_booking_restaurant_reqmore_general: Your reservation has been booked. Your reference number is _reference_ . Please be aware that your table will only be reserved until _time_ . Can i provide any more assistance? -->
* No I think that s all, thank you
    - bye_general_welcome_general: You re very welcome. Have a great day and text us back anytime!   <!-- predicted: bye_general: You re welcome. Thank you for using the TownInfo centre. Goodbye. -->


## story_PMUL4440
* I m looking for this restaurant called _attraction_name_ hut fen ditton
    - slot{"restaurant_status": "available"}
    - inform_restaurant_reqmore_general: it is a moderately priced restaurant in the _area_ that serves _food_type_ food. can i _number_ you the address?   <!-- predicted: inform_restaurant_recommend_restaurant_reqmore_general: i recommend _restaurant_name_ . it is located in the _area_ side in _number_ Castle Street City Centre. can i get you the phone number? -->
* No, but could you book a table for me? _number_ people on _weekday_ at _time_ , please.
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_reqmore_general: Booking was successful. The table will be reserved for _number_ minutes. Reference number is _reference_ . Is there anything else I can help you with?   <!-- predicted: book_booking_restaurant: You are booked! Your table will be reserved for fifteen minutes and your reference number is _reference_ . -->
* I m not sure ... let me ask my wife.
    - reqmore_general: Can I help you with anything else?   <!-- predicted: book_booking_restaurant_reqmore_general: Your table is booked, ref _reference_ . Can I help you with anything else? -->
* I also need a place to stay.
    - request_hotel: Can you please tell me what type of place and if you have any preferences?   <!-- predicted: inform_hotel: I ve found _number_ hotels matching your preferences. The _hotel_name_ is in the _pricerange_ price range and is located in the centre of town if you are interested. -->
* I want a guesthouse in the _area_ with a _pricerange_ price range and _number_ stars.
    - slot{"hotel_status": "unique"}
    - _hotel_name_ would fit that criteria, would you like to make a booking?
* Yes, that would be great. I ll need to book for _weekday_ , _number_ people, and for _number_ nights.
    - slot{"hotel_status": "NA"}
    - inform_hotel_nooffer_hotel: Actually, the _hotel_name_ is in the _area_ . It is _number_ stars with a _pricerange_ price range. I didn t see anything that fit your criteria in the _area_ .   <!-- predicted: nobook_booking_hotel_request_booking_hotel: Unfortunately that booking was unsuccessful . May we try for a shorter stay or a different day? -->
* Would you check again for a guesthouse in the _pricerange_ price range, in the _area_ with _number_ stars, please?
    - slot{"hotel_status": "unique"}
    - _hotel_name_ fits your criteria. can i book this?
* Yes, sounds good. Can I get the reference with that too please?
    - slot{"hotel_status": "booked"}
    - book_booking_hotel: I have booked your room here is your information Booking was successful.Reference number is _reference_   <!-- predicted: book_booking_restaurant: I just completed your booking. The table will be reserved for _number_ minutes and the reference number is _reference_ . Is there anything else I can help you with? -->
* thank you very much
    - reqmore_general: is there anything else i can do for you?   <!-- predicted: reqmore_general_welcome_general: You are welcome. Is there anything else I can do for you today? -->
* Nope, that s all! Thanks!
    - Thank you for using our services. Have a wonderful day!


## story_MUL0821
* I m looking for a restaurant in the city centre.
    - slot{"restaurant_status": "available"}
    - There are _number_ results for restaurants in city centre. Could you be more specific on what type of food you re hungry for, or price range you d like?
* I would like a restaurant that serves _food_type_ .
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_restaurant: There are _number_ _food_type_ restaurants in the centre. Do you have a preferred price range?   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* No I do not, can you please find me the highest rated restaurant?
    - greet_general_inform_restaurant_reqmore_general: I do not have access to restaurant ratings, however _number_ of the restaurants serving _food_type_ are considered _pricerange_ . Would you like their information?   <!-- predicted: inform_restaurant: There is _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _restaurant_name_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _area_ _food_type_ , _food_type_ , _food_type_ , and _food_type_ food available in the centre. -->
* Just _number_ please, and only the address is necessary. I d also like a place to go in town, a _attraction_name_ is good, it should be in the centre
    - slot{"attraction_status": "available"}
    - slot{"restaurant_status": "available"}
    - inform_restaurant: The address for _restaurant_name_ is _number_ Trumpington Street City Centre.   <!-- predicted: inform_attraction_recommend_attraction: I have _number_ museums in the Centre. I would recommend _attraction_name_ , phone number _number_ , postal code cb23bj, address unit su43, grande arcade, saint andrews street. It is free. -->
* Okay, thanks. And a _attraction_name_ ?
    - inform_attraction_recommend_attraction: there are approximately _number_ museums in the centre of town, all with free entrance. My personal recommendation would be the _attraction_name_ .   <!-- predicted: request_booking_hotel: great! for how many people, which day, and for how long? -->
* Sounds good. What s the address and phone number of the Whipple?
    - slot{"attraction_status": "available"}
    - inform_attraction: It is located at free _attraction_name_ lane and their phone number is _number_   <!-- predicted: inform_attraction_inform_train_reqmore_general: The _attraction_name_ s address is Market Street, postcode cb23nz. There are many trains arriving in Stansted Airport by _time_ . Would you like to narrow your search further? -->
* Alright, great. I also need a taxi to get between the restaurant and the _attraction_name_ . I want to leave the restaurant by _time_ .
    - slot{"taxi_status": "booked"}
    - inform_taxi_reqmore_general: I was able to arrange your taxi service. Your vehicle will be a _color_ _reference_ , and the company s contact number is _number_ . Anything else I can help with?   <!-- predicted: inform_taxi: Okay! Your taxi is a _color_ _color_ _cartype_ . Contact number _number_ -->
* No that will be all, thank you.
    - We are happy to help. Thank you for using our service.


## story_PMUL3549
* Get me information about _attraction_name_ please
    - slot{"attraction_status": "available"}
    - Certainly! _attraction_name_ is a _attraction_name_ located on the _area_ side of town. Their address is castle street and their phone number is _number_ . Is there anything else?
* Do they charge an entrance fee?
    - They do not charge an entrance fee. Can I help with anything else?
* Thanks, can I have the post code, please?
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: Sure. The postcode is cb30aq. Is there anything else I can help you with?   <!-- predicted: inform_attraction: Yes, It is a _attraction_name_ . The postcode is cb30ag. -->
* Yes, I am also looking for a train that leaves after _time_ going to ely.
    - slot{"train_status": "available"}
    - request_train: Are you departing from _hotel_name_ ?   <!-- predicted: inform_train_request_train: I have _number_ trains travelling to _hotel_name_ , could you be more specific on what day you d like to leave and where you are departing from? -->
* Yes on _weekday_
    - slot{"train_status": "unique"}
    - OK, _reference_ leaves at _time_ would you like more info or a booking?
* Can you please book me for _number_ people?
    - slot{"train_status": "booked"}
    - offerbooked_train_reqmore_general: You are all set, the reference number is _reference_ , can I help with anything else?   <!-- predicted: offerbooked_train: I have booked for you train _reference_ the total fee is _number_ _reference_ payable at the station .Reference number is _reference_ -->
* You have answered all my questions. I appreciate it. Goodbye.
    - bye_general: Have a lovely day too.!   <!-- predicted: bye_general_welcome_general: You re welcome. Enjoy your time in _hotel_name_ and please let us know if you need anything else. Thanks! -->


## story_SNG1150
* I m trying to find a _attraction_type_ in the _area_ part of town.
    - slot{"attraction_status": "NA"}
    - nooffer_attraction_request_attraction: Unfortunately, I don t have any listings for concert halls on the _area_ side. Can I check another area of town for you?   <!-- predicted: nooffer_attraction: I am sorry, there are no swimming pools located on the _area_ side. Would you be interested in visiting a different attraction? -->
* How about an _attraction_type_ attraction instead?
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: There are _number_ _attraction_type_ attractions on the _area_ side. Would you like more information?   <!-- predicted: inform_attraction: The _attraction_name_ is a great example of _attraction_type_ , Broughton House Gallery is a good, free _attraction_name_ , and the _hotel_name_ University Botanic Gardens is a lovely _attraction_type_ . -->
* Yes and can I have the phone number and address of _number_ of attraction?
    - inform_attraction_reqmore_general: Sure. _attraction_name_ can be reached at _number_ . It is on Cherry Hinton Road, postcode cb18dw. Can I help you with anything else today?   <!-- predicted: inform_attraction: The scudamores punting co is at granta place, mill lane phone number is _number_ . The _hotel_name_ punter is at 251a chesterton road phone number _number_ . No entrance fee information listed. -->
* Thanks. That s all I need for now.
    - bye_general: Okay Thank you for calling.   <!-- predicted: bye_general_greet_general_welcome_general: Thank you for using our service. Call us anytime. Take care. Goodbye. -->


## story_SNG0797
* Hello, I need to find a _hotel_type_ with free wifi and free parking. Can you help me?
    - slot{"hotel_status": "available"}
    - There are _number_ places with free internet and parking. Do you have an area, price, star, or _hotel_type_ type preference?
* Can you find me a guesthouse that is _pricerange_ ?
    - slot{"hotel_status": "NA"}
    - nooffer_hotel_request_hotel: Unfortunately, I don t happen to have any guesthouses that are in the _pricerange_ range. Can I look in another price range perhaps?   <!-- predicted: inform_hotel: Actually, _hotel_name_ doesn t meet your requirements. But I do have other options that are moderately priced, such as _hotel_name_ , Arbury Lodge Guesthouse, and _hotel_name_ . -->
* How about in the _pricerange_ price range?
    - slot{"hotel_status": "available"}
    - inform_hotel_request_hotel: I have _number_ guesthouses that match your needs. Do you have additional requirements to narrow down the search?   <!-- predicted: inform_restaurant: I found _number_ options for you _restaurant_name_ at Regent Street City Centre, _restaurant_name_ at _number_ Mill Road City Centre, and _restaurant_name_ at _number_ _hotel_name_ Road City Centre -->
* Could you recommend _number_ with free wifi and free parking in the _pricerange_ price range, and give me the star rating and phone number?
    - recommend_hotel: _hotel_name_ is a _number_ star place that meets your requirements. The phone number is _number_ .   <!-- predicted: inform_hotel_select_hotel: I have _number_ options with those specifications. The _hotel_name_ and the _hotel_name_ both with free wifi and parking. Which would you prefer? -->
* Thank you, that will be all. Goodbye.
    - bye_general: Enjoy! Goodbye!   <!-- predicted: bye_general_welcome_general: Thanks for letting us assist you today! Have a great trip! -->


## story_SNG0061
* I would like to book a taxi to leave after _time_ going to Arbury Lodge Guesthouse.
    - slot{"taxi_status": "available"}
    - Where are you departing from?
* from _restaurant_name_
    - slot{"taxi_status": "booked"}
    - All right, a _color_ _cartype_ will pick you up. The contact number is _number_ .
* Great! Thank you for your help!
    - reqmore_general: You re welcome! What else can I do for you?   <!-- predicted: nooffer_restaurant_request_restaurant: I m sorry, but I could not find any listings for restaurants serving _food_type_ style food. Do you have any other favorite types of cuisines? -->
* No that will be all for today. Thank you!
    - bye_general: Let us know if you need anything else, bye.   <!-- predicted: bye_general_welcome_general: You are quite welcome. Thank you for using our services! -->


## story_PMUL4547
* Please find a restaurant called _restaurant_name_
    - slot{"restaurant_status": "unique"}
    - That is an _food_type_ restaurant in the center of town in the _pricerange_ price range. Could you like a reservation?
* I _reference_ like a reservation for _number_ people at _time_ on _weekday_ , please.
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant: Yes your booking was successful and the reference number is _reference_ .   <!-- predicted: book_booking_restaurant_reqmore_general: Your booking is confirmed. Your reference number is _reference_ . Please note they will only reserve the table for _number_ minutes. Is there anything else you need? -->
* Thank you for the reference number. I m also looking for a place called _attraction_name_ .
    - slot{"attraction_status": "available"}
    - inform_attraction: Ah, that s a great theatre in the _area_ part of town. Located on clifton way, phone is _number_ .   <!-- predicted: reqmore_general: Yes nice place. Did you need any info on it ? -->
* Is there an entrance fee?
    - The entrance fee is unknown. Can I help you with anything else today?
* I would also like a taxi to arrive at the restaurant on time. Can I have the taxis phone number and vehicle type?
    - slot{"taxi_status": "available"}
    - Where would you like the taxi to pick you up?
* _attraction_name_ , please.
    - slot{"taxi_status": "available"}
    - request_taxi: What is your destination and what time do you want to leave?   <!-- predicted: inform_taxi: Alright, I ve booked a _color_ _cartype_ for you. -->
* My destination is _restaurant_name_ . I need to arrive by _time_ .
    - slot{"taxi_status": "booked"}
    - Your taxi has been booked. Please look for a _color_ _cartype_ . The contact number is _number_ ..
* Thank you. I have written the information down. I appreciate you gathering the details.
    - reqmore_general: Is there anything else I can help you with today?   <!-- predicted: reqmore_general_welcome_general: You re so welcome! Is there anything else I can help you with today? -->
* No that is it, thank you!
    - bye_general: Hope you have a great trip. Good bye.   <!-- predicted: bye_general_welcome_general: You re welcome, farewell! Text back anytime! -->


## story_PMUL3158
* I want to find a place in town to visit called _attraction_name_ .
    - slot{"attraction_status": "available"}
    - inform_attraction: Hello. _attraction_name_ is in the _area_ area between Victoria Rd. and the River. Call _number_ to find more about costs.   <!-- predicted: inform_attraction_recommend_attraction: I have _number_ different options to choose from. If you would like a recommendation, the Primavera is a great _attraction_name_ to visit! Would you like more information on them? -->
* Sounds good! Do you happen to know what attraction type it is?
    - It is a swimmingpool
* now I need a _food_type_ place to eat
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_restaurant: There are a wide variety of _food_type_ restaurants in the city. Do you have a preference on where it is or the price range?   <!-- predicted: inform_hotel_request_hotel: I have several options for you, ranging from _pricerange_ to _pricerange_ in price. Do you have a price range in mind, or perhaps a certain area of town? -->
* I would like an _pricerange_ restaurant.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_restaurant: I have _number_ options for you, any particular area of town you want to dine in?   <!-- predicted: inform_hotel_request_hotel: I have about _number_ different places. Do you have a preference on the area of town? -->
* Yes it needs to be in the centre. Can you book me a table for _number_ people at _time_ on _weekday_ ?
    - slot{"restaurant_status": "available"}
    - inform_restaurant: How does _restaurant_name_ sound?   <!-- predicted: inform_booking_restaurant: Certainly. I will have that reference number for you in just _number_ second. -->
* Yes. Please book it.
    - slot{"restaurant_status": "booked"}
    - Booking was successful. The table will be reserved for _number_ minutes.Reference number is _reference_ .
* Thanks, that s all for today. Goodbye.
    - reqmore_general: Do you need anymore info?   <!-- predicted: bye_general_welcome_general: You re welcome, farewell! Text back anytime! -->


## story_MUL0536
* I am looking for Abbey Pool and Astroturf Pitch can you help me?
    - slot{"attraction_status": "available"}
    - inform_attraction: Yes, Abbey pool and astroturf pitch is a swimmingpool _area_ of town. Their number is _number_ , and address is pool way, whitehill road, off newmarket road. Postcode cb58nt.   <!-- predicted: greet_general_inform_attraction: That sounds like an exciting trip! _hotel_name_ University Botanic Gardens is located in the centre of town on Bateman Street. Its admission fee is _number_ pounds. -->
* Thank you very much for the information. That is all I needed help with. Have a nice day.
    - slot{"attraction_status": "available"}
    - reqmore_general_welcome_general: You re welcome. Let me know if I can do anything else for you.   <!-- predicted: greet_general_welcome_general: You are so very welcome! I hope you have a wonderful trip and a fantastic day, call anytime you need assistance! -->
* I actually do need to find a train going to ely.
    - slot{"train_status": "available"}
    - Is that leaving from _hotel_name_ ? And if so, what time would you like to arrive in Ely?
* Yes, I will be leaving _hotel_name_ and going to Ely, I would like it to arrive by _time_ .
    - slot{"train_status": "available"}
    - inform_train_request_train: What day would you be traveling? There are _number_ trains on that route. There is a train that departs _weekday_ at _time_ and will arrive in Ely at _time_ .   <!-- predicted: inform_train: There a few trains that will get you there. _reference_ departs at _time_ and arrives at _time_ . Does that work for you? -->
* Oops! I guess forgot to mention it s _weekday_ that I need to travel.
    - slot{"train_status": "available"}
    - inform_train: There are _number_ trains that would fit, leaving at _time_ , _time_ , or _time_ .   <!-- predicted: inform_train_request_train: The departure time is _time_ . The travel time is _number_ minutes. How many are traveling? -->
* Can I get info for the _time_ the price and the trains ID please?
    - slot{"train_status": "available"}
    - Certainly. The train s ID is _reference_ , and the price for a ticket is _number_ pounds.
* Great, thank you! That will be all I need for now.
    - reqmore_general: Are you certain you don t need further assistance?   <!-- predicted: bye_general: Okay great. I am glad I could help you. -->
* _time_ departure, _number_ pounds, _reference_ . I got it, thank you!
    - welcome_general: Thank you for using the _hotel_name_ TownInfo centre today.   <!-- predicted: inform_train: There a few trains that will get you there. _reference_ departs at _time_ and arrives at _time_ . Does that work for you? -->


## story_PMUL3688
* I am looking for a place to go in the centre of town.
    - slot{"attraction_status": "available"}
    - request_attraction: Is there any type of attraction you d like to see?   <!-- predicted: inform_attraction_select_attraction: There are _number_ in the centre of town. Scudamores Punting Co, and the _hotel_name_ Punter. Would either of those interest you? -->
* any of your choice. get me the address and entrance fee
    - inform_attraction_recommend_attraction_reqmore_general: The _attraction_name_ is located on Market Street. The entrance fee is free. Is there anything else I can help with?   <!-- predicted: inform_attraction_reqmore_general: We have no entrance fee information for any of the theatres at this time. Can I help you with anything else? -->
* I also need a train out to the airport on _weekday_ .
    - slot{"train_status": "available"}
    - request_train: Where will you be departing from, and do you have a destination in mind?   <!-- predicted: request_taxi: I d be happy to help you with a taxi, what is your destination departure and what time would you like to arrive leave? -->
* leaving _hotel_name_ and going to stansted airport and I want to leave anytime after _time_
    - slot{"train_status": "available"}
    - There is a train that leaves at _time_ .
* That will work. I will need tickets for _number_ people.
    - slot{"train_status": "booked"}
    - It is booked and your reference number is _reference_ .
* Perfect thats everything thanks
    - bye_general_welcome_general: Alright, thanks for using _hotel_name_ TownInfo, have a great day!   <!-- predicted: bye_general: i am glad i have been of help to you. great day -->


## story_MUL0230
* Can you find me a train going to _hotel_name_ on _weekday_ ?
    - slot{"train_status": "available"}
    - request_train: What departure site were you interested in?   <!-- predicted: inform_train_request_train: There are _number_ trains departing for Stevenage, where would you be departing from? -->
* I am looking to depart from bishops stortford and need to arrive by _time_ .
    - slot{"train_status": "unique"}
    - I have _number_ trains leaving from bishops stortford on _weekday_ . The last _number_ arrives in _hotel_name_ at _time_ . Would you like to book?
* I think so. How much is that train? And can you tell me the travel time?
    - inform_train: The cost is _number_ _reference_ per ticket, and the travel time is _number_ minutes.   <!-- predicted: inform_hotel_nooffer_hotel_request_hotel: It seems like all of my guesthouses are in different price ranges. No _pricerange_ ones are listed. Can I interest you in a different price range? -->
* Thanks. I m also wondering what kind of information you have on _attraction_name_ Express.
    - slot{"restaurant_status": "available"}
    - inform_restaurant: _attraction_name_ express serves _food_type_ food, is located in the centre of town, in the _pricerange_ price range, their phone number is _number_ , postcode is cb213b, and at Regent Street City Centre   <!-- predicted: inform_attraction: It s located in the _area_ part of town, the phone number there is _number_ , the address is just _attraction_name_ , Milton, the postcode is cb46az. -->
* Great! Thank you very much for your help.
    - reqmore_general_welcome_general: You are very welcome. Is there anything else I can help you with?   <!-- predicted: reqmore_general: Is there anything else I can do for you before we go? -->
* No. Thank you. That s great.
    - Happy to be of service - have a wonderful day!


## story_SNG0528
* Hi, I m looking for a restaurant with _food_type_ food. It should be in the _pricerange_ price range.
    - slot{"restaurant_status": "available"}
    - request_restaurant: What area are you wanting to be in?   <!-- predicted: inform_restaurant_request_restaurant: There are _number_ _pricerange_ restaurants in town. Do you have a food preference or an area of town you want to eat in? -->
* Doesn t really matter. Is there _number_ in the centre?
    - slot{"restaurant_status": "available"}
    - inform_restaurant_reqmore_general: Yes, there are _number_ _restaurant_name_ & _restaurant_name_ . Would you like further information?   <!-- predicted: inform_restaurant_select_restaurant: I have the _restaurant_name_ which serves _food_type_ . I also have _restaurant_name_ that serves _food_type_ food. Which would you prefer? -->
* Can I book _restaurant_name_ for _number_ people at _time_ on _weekday_ please?
    - slot{"restaurant_status": "booked"}
    - Your tabled has been reserved for _number_ people on _weekday_ at _time_ . The reference number is _reference_ .
* Thank you so much. That is all I need for now. Have a great day.
    - Thank you. Goodbye.


## story_SNG0253
* I am looking for a train to _hotel_name_ on _weekday_ .
    - slot{"train_status": "available"}
    - request_train: certainly, do you know from where you will be departing, and at what time?   <!-- predicted: inform_train: There are several trains departing for _hotel_name_ on _weekday_ . _number_ train departs every hour starting at _time_ -->
* I will depart at _location_ and should arrive by _time_ . Can you help me with this?
    - slot{"train_status": "available"}
    - Of course I can. There are _number_ possibilities, at what time would you like to leave?


## story_PMUL0685
* I m planning a trip to _hotel_name_ and am looking for a place to dine.
    - inform_restaurant_request_restaurant: There are many great places to dine in _hotel_name_ . To help narrow it down, what area are you looking for and what type of food?   <!-- predicted: request_restaurant: Do you have a certain cuisine or area in mind? -->
* I m looking for an _food_type_ restaurant in the _area_ .
    - slot{"restaurant_status": "unique"}
    - I have _number_ place. Would you like me to book it?
* Sure, I need a table for _number_ on _weekday_ at _time_ please.
    - slot{"restaurant_status": "booked"}
    - Here is your booking information Booking was successful. The table will be reserved for _number_ minutes.Reference number is _reference_ .
* Thanks I also need a train leaving _weekday_ from _hotel_name_ to _location_ leaving after _time_ .
    - slot{"train_status": "available"}
    - I have _number_ trains available. What time would you like to arrive?
* i would just like the train leaving the closest after _time_ .
    - slot{"train_status": "unique"}
    - The closest _number_ is _reference_ it leaves at _time_ would you like me to book it for you?
* I am not ready too book yet. May I have the price and travel time, please?
    - inform_train: The _reference_ takes _number_ minutes and is only _number_ pounds.   <!-- predicted: nobook_booking_attraction_reqmore_general: I can not. It doesn t give me the option to book tickets. Just general Information. Can I help you with anything else? -->
* Okay, thank you. Good-bye.
    - bye_general: Have nice day as well!   <!-- predicted: bye_general_welcome_general: You are quite welcome. Thank you for using our services! -->


## story_MUL1189
* Can you give me directions to Byard Art in _hotel_name_ ?
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: I can tell you that Byard Art is located at _number_ King s Parade, postcode cb21sj. Does that help?   <!-- predicted: request_hotel: Yes, I can certainly help you with that. Is there an area of town you prefer to stay in? And do you have a price range in mind? -->
* Yes, I will also need the phone number and entrance fee please.
    - The number is _number_ and it is free of charge.
* Can you give me the address please?
    - inform_attraction_reqmore_general: The address is _number_ king s parade. Do you need anything else?   <!-- predicted: inform_hotel_reqmore_general: Of course! I have Back Lane, Cambourne listed as the address, is there anything else I can help with today? -->
* Hmm, that number doesn t seem like it would be correct. Can you double check that for me?
    - greet_general_inform_attraction: Yes, I am so sorry for the error. The correct phone number is _number_ and admission is actually free.   <!-- predicted: reqmore_general: Yes nice place. Did you need any info on it ? -->
* Can you help me find a _number_ star _hotel_type_ , and it doesn t matter if it doesn t have internet.
    - slot{"hotel_status": "available"}
    - inform_hotel: There are _number_ options. Do you have any other preferences to narrow the search?   <!-- predicted: inform_hotel_request_hotel: I show _number_ hotels in the _area_ , _number_ is _pricerange_ and _number_ is _pricerange_ . I also show _number_ _pricerange_ _number_ star _hotel_type_ in the _area_ . Which area do you prefer? -->
* I would like it to be in the _pricerange_ price range and include free parking.
    - slot{"hotel_status": "available"}
    - inform_hotel_request_hotel: I have _pricerange_ hotels across _hotel_name_ do you have an area in mind?   <!-- predicted: inform_hotel_select_hotel: I have _number_ options with those specifications. The _hotel_name_ and the _hotel_name_ both with free wifi and parking. Which would you prefer? -->
* No, but I do need free wifi. Could you book a room for _weekday_ ? I will need it for _number_ nights. I will be alone.
    - slot{"hotel_status": "NA"}
    - nobook_booking_hotel_request_booking_hotel: Booking was unsuccessful. Would you like to shorten your stay or add another day?   <!-- predicted: inform_hotel_request_hotel: There are _number_ available that match what you re looking for, do you have any preference for what area you want to stay in? -->
* How about _number_ night? Could you also please provide me with the reference number? I would also like to book a taxi.
    - slot{"hotel_status": "booked"}
    - book_booking_hotel: Booking was successful at _hotel_name_ . Reference number is _reference_ .   <!-- predicted: offerbooked_train_request_hotel: The fee for the train tickets is _number_ _reference_ which is payable at the station. Your reference number is _reference_ . Is there a specific _hotel_type_ you have in mind? -->
* I d also like to book a taxi to go between the _number_ . I d like to leave Byard Art by _time_ .
    - slot{"taxi_status": "booked"}
    - inform_taxi_reqmore_general: I booked you a _color_ _cartype_ . The contact number is _number_ . Is there anything else I can assist you with?.   <!-- predicted: inform_taxi: Okay! Your taxi is a _color_ _color_ _cartype_ . Contact number _number_ -->
* No, that s all. Thank you!
    - You re welcome. Enjoy your time in _hotel_name_ !


## story_MUL2139
* I need to find a guesthouse in the _area_ .
    - slot{"hotel_status": "available"}
    - I have about _number_ different options. Do you have a preference on price range?
* I would prefer that be _pricerange_ .
    - slot{"hotel_status": "NA"}
    - inform_booking_hotel_inform_hotel_nooffer_hotel_reqmore_general_select_hotel: There are no _pricerange_ guesthouses however I do see _pricerange_ ones. Would you like to try _number_ of those?   <!-- predicted: inform_hotel: Actually, _hotel_name_ doesn t meet your requirements. But I do have other options that are moderately priced, such as _hotel_name_ , Arbury Lodge Guesthouse, and _hotel_name_ . -->
* Yes,but needs to be a _number_ star in the _area_
    - slot{"hotel_status": "available"}
    - inform_hotel_request_hotel: ok, there are _number_ options. Would you like free internet or parking?   <!-- predicted: inform_hotel: There are _number_ hotels in the _area_ , _hotel_name_ and _hotel_name_ which would you like? -->
* Doesn t matter. Book _number_ of them for myself and _number_ nights starting from _weekday_ .
    - slot{"hotel_status": "booked"}
    - book_booking_hotel_inform_hotel_reqmore_general: Booking at the _hotel_name_ was successful, the reference number is _reference_ . It is located at _number_ Chesterton Road, Postal Code cb41da. Is there anything else I can help with?   <!-- predicted: book_booking_hotel: Okay, your booking was successful! We have you booked at the _hotel_name_ . Your reference number is _reference_ . -->
* Yes, can you help me find a train?
    - request_train: I can. All I need is your departure location, destination, day and when you would like to either leave or arrive by.   <!-- predicted: inform_hotel_request_train: _hotel_name_ number is _number_ . I can absolutely help you with train, can you specify which day you d like to leave? -->
* I will be leaving _location_ the same day as my _hotel_type_ booking.
    - slot{"train_status": "booked"}
    - offerbooked_train: Booking was successful, the total fee is _number_ _reference_ payable at the station .Reference number is _reference_ .   <!-- predicted: greet_general_select_hotel: Okay. And did you want it in the _area_ or the _area_ ? -->
* Wow. You didn t even get the timeframe I am looking for. I can t leave until after _time_ .
    - slot{"train_status": "available"}
    - inform_train_reqmore_general: I apologize! There are _number_ trains leaving near your requested time. _number_ at _time_ and _number_ at _time_ . Will _number_ of those work?   <!-- predicted: inform_train_request_train: There are _number_ trains leaving _hotel_name_ after that time. What is your destination and day of travel? -->
* The _number_ at _time_ should be fine. Can you tell me when it arrives?
    - slot{"train_status": "available"}
    - inform_train: It will arrive at _time_ .   <!-- predicted: offerbooked_train_reqmore_general: Sure, the train is actually number _reference_ and your reference number is _reference_ . The price will be _number_ _reference_ payable at the station. Is there anything else today? -->
* What is the travel time?
    - slot{"train_status": "unique"}
    - It s _number_ minutes. Would you like to book some tickets?
* Yes please, just _number_ ticket would be fine.
    - slot{"train_status": "booked"}
    - Good news! Booking was successful, the total fee is _number_ _reference_ payable at the station .Reference number is _reference_ . Is there anything else that you need?
* No thanks. That was all I needed. Have a good day
    - bye_general: Enjoy your stay in _hotel_name_ . Bye.   <!-- predicted: bye_general_welcome_general: Thank you! Have a good day. Good bye! -->


## story_MUL0116
* Hello, I am looking for a restaurant in the town centre that serves _food_type_ .
    - slot{"restaurant_status": "available"}
    - There are _number_ restaurants in the centre of town that serves _food_type_ . Is there any particular price range you are looking for?
* Yes, I m looking for a moderately priced restaurant with _food_type_ .
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_recommend_restaurant: I can recommend Restaurant _number_ _number_ . Would you like to book a table with them?   <!-- predicted: inform_booking_restaurant_inform_restaurant: How about _restaurant_name_ ? I can book you a table there if you like. -->
* Sure. I will be booking _number_ people at _time_ on _weekday_ . Could i also get the reference number, please?
    - slot{"restaurant_status": "booked"}
    - Your reservation is complete for a party of _number_ at _time_ at a _food_type_ Restaurant _number_ _number_ in centre, and your confirmation is _reference_ .
* I also need a _hotel_type_ in the same price range as the restaurant.
    - slot{"hotel_status": "available"}
    - inform_hotel_reqmore_general: There are _number_ hotels in the _pricerange_ price range, would you like me to narrow these down by searching other amenities or location?   <!-- predicted: inform_hotel_request_hotel: I show _number_ hotels in the _area_ , _number_ is _pricerange_ and _number_ is _pricerange_ . I also show _number_ _pricerange_ _number_ star _hotel_type_ in the _area_ . Which area do you prefer? -->
* I would like something that is _number_ stars and includes free parking.
    - slot{"hotel_status": "available"}
    - I have _number_ options with those specifications. The _hotel_name_ and the _hotel_name_ both with free wifi and parking. Which would you prefer?
* Could you book a room for _number_ people, _number_ nights on _weekday_ at the _restaurant_name_ , please?
    - slot{"hotel_status": "NA"}
    - inform_booking_hotel_nobook_booking_hotel: Book was unsuccessful. Would you like to try the _hotel_name_ ?   <!-- predicted: nobook_booking_hotel_request_booking_hotel: Sorry I tried _hotel_name_ but it seems that they have all booked out at for these days. Do you want to change to another place? -->
* Sure, lets try that instead.
    - slot{"hotel_status": "NA"}
    - I was unable to book the _hotel_name_ for you on _weekday_ . Do you want to try a different day or a shorter stay?
* Can you try the _hotel_name_ for the _weekday_ , please?
    - slot{"hotel_status": "NA"}
    - nobook_booking_hotel_reqmore_general: I am sorry. _hotel_name_ still has no bookings available for _weekday_ . Would you like to try a different _hotel_type_ ?   <!-- predicted: nobook_booking_hotel_request_booking_hotel: Sorry I tried _hotel_name_ but it seems that they have all booked out at for these days. Do you want to change to another place? -->
* Yes, I need a _number_ star _hotel_type_ for _number_ people for _number_ nights on _weekday_ , moderately priced, with free parking.
    - slot{"hotel_status": "booked"}
    - OK, I have you booked in the _hotel_name_ . The Reference Number is _reference_ . Can I help you with anything else today?
* I think that s all I need. Thank you.
    - slot{"hotel_status": "available"}
    - bye_general: My pleasure, enjoy your trip.   <!-- predicted: bye_general_welcome_general: You are very welcome. Thank you for contacting the _hotel_name_ TownInfo centre and have a great day! -->


## story_PMUL3521
* Can you tell me a good _attraction_name_ in town?
    - slot{"attraction_status": "available"}
    - request_attraction: Sure, what part of town did you want to visit?   <!-- predicted: inform_attraction_reqmore_general: There are _number_ colleges in town centre. _hotel_name_ and Caius _attraction_name_ is on trinity street with free entrance. Do you want more information on any others? -->
* I d like to visit something in the _area_ part of town.
    - slot{"attraction_status": "available"}
    - recommend_attraction_reqmore_general: I d recommend _attraction_name_ . Their phone number is _number_ . Can I help you with anything else?   <!-- predicted: inform_attraction_reqmore_general: I have _number_ _attraction_type_ attractions. _number_ are in the centre, with _number_ in the _area_ and _area_ . Are you interested in information about _number_ of them in a certain area? -->
* Could you provide me with the address and entrance fee?
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: It is free to enter and the address is _number_ magdalene street. Can I help you with anything else today?   <!-- predicted: inform_attraction: Certainly, the address is _hotel_name_ leisure _attraction_type_ , clifton way, however we don t have the entrance fee listed. -->
* Yes, I also need a place to stay in the _area_ area. It should be _number_ stars and have free wifi.
    - slot{"hotel_status": "available"}
    - recommend_hotel: If price is not an issue, I recommend the _pricerange_ _hotel_name_ . If you want something cheaper, I recommend _hotel_name_ .   <!-- predicted: inform_hotel_select_hotel: I have _number_ options with those specifications. The _hotel_name_ and the _hotel_name_ both with free wifi and parking. Which would you prefer? -->
* Can you book me a room at the Marriott for _number_ nights starting _weekday_ ?
    - slot{"hotel_status": "available"}
    - request_booking_hotel: How many people do you need a room for?   <!-- predicted: recommend_hotel_request_booking_hotel: OK, how about _hotel_name_ ? To book a stay I ll need to know the first day you want to stay, how many days, and how many guests. -->
* _number_ person please.
    - slot{"hotel_status": "booked"}
    - book_booking_hotel_reqmore_general: You are set, you reference number is _reference_ . May I assist you with anything else today?   <!-- predicted: book_booking_hotel_inform_hotel: Sorry, there must have been a glitch in the system. You are booked at _hotel_name_ starting _weekday_ for _number_ days, _number_ guests. Reference is _reference_ -->
* There s nothing else I need at this time. Thank you very much for your assistance!
    - bye_general: I m happy we could be of service. Enjoy your stay in _hotel_name_ !   <!-- predicted: bye_general_inform_booking_hotel: Just let us know when you are ready to book and we will be happy to assist you. Have a great day! -->


## story_SNG0721
* Hi, I m looking for restaurants in the area that serve _food_type_ cuisine. Could you give me some suggestions?
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_restaurant: There are many _food_type_ restaurants in the city. Could you tell me in what area you would like to eat?   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* Is there something available in the _area_ ?
    - slot{"restaurant_status": "available"}
    - inform_restaurant_select_restaurant: Yes, there are _number_ . Would you like something in the _pricerange_ or _pricerange_ price range?   <!-- predicted: inform_restaurant: The top _number_ places serving _food_type_ cuisine are _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Would you like more options? -->
* I don t care about the price range. However, I need to confirm that the restaurant serves _food_type_ and is in the centre of town.
    - slot{"restaurant_status": "unique"}
    - The Restaurant _number_ _number_ meets your specifications of _food_type_ in the centre of town. Would you like me to book that for you?
* Yes. For _number_ people at _time_ on _weekday_ , please. I ll need the reference number.
    - slot{"restaurant_status": "booked"}
    - Booking was successful. The table will be reserved for _number_ minutes.Reference number is _reference_ .
* Great thanks so much!
    - reqmore_general: Is there anything else I can help you with?   <!-- predicted: offerbook_train_reqmore_general_welcome_general: You re welcome! Is there anything else I can assist you with? I can help you create a booking for the train. -->
* That s all I needed thank you
    - bye_general: You re welcome. Have a great meal!   <!-- predicted: bye_general_welcome_general: You are quite welcome. Thank you for using our services! -->


## story_MUL0148
* I am looking for a centrally located upscale restaurant.
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant: I can book you at the _restaurant_name_ if you would like.   <!-- predicted: inform_booking_restaurant_recommend_restaurant: _restaurant_name_ is a very popular restaurant in the _pricerange_ range. Would you like me to book a reservation for you? -->
* For _number_ people, at _time_ on _weekday_ . Reference number please.
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_greet_general_reqmore_general: Ok. I ve booked your table. Your reference number is _reference_ . Can I help with anything else?   <!-- predicted: book_booking_restaurant: You are booked! Your table will be reserved for fifteen minutes and your reference number is _reference_ . -->
* Yes. I a place to stay. A upscale _hotel_type_ please.
    - slot{"hotel_status": "available"}
    - There are _number_ hotels in that area, can you give me a price range and a star rating to narrow down the search?
* I prefer upscale and want to stay in a _hotel_type_ rather than a guesthouse. I also need free parking.
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel_recommend_hotel: _hotel_name_ is located _area_ and has _number_ stars. Does this sound okay to you?   <!-- predicted: recommend_hotel: If price is not an issue, I recommend the _pricerange_ _hotel_name_ . If you want something cheaper, I recommend _hotel_name_ . -->
* Does it have free parking? And internet?
    - slot{"hotel_status": "unique"}
    - Yes, the _hotel_name_ has both free parking and internet. Would you like me to book a room for you?
* Not right now. Can I please have the address and phone number of the _hotel_name_ ?
    - slot{"hotel_status": "available"}
    - Of course! The address of the _hotel_name_ is kingfisher way, hinchinbrook business _attraction_type_ , huntingdon and it s phone number is _number_ , would you like anything else?
* No, that should be it, thanks!
    - bye_general_welcome_general: So happy to be of service, and thanks for using _hotel_name_ TownInfo centre today. Have a wonderful day!   <!-- predicted: request_booking_hotel: For how many rooms and how long is your stay going to be? -->


## story_PMUL3156
* I m trying to find information about a particular restaurant called _restaurant_name_ .
    - slot{"restaurant_status": "available"}
    - slot{"hotel_status": "NA"}
    - nooffer_hotel: our records don t show that _hotel_type_ . sorry   <!-- predicted: recommend_restaurant_request_booking_restaurant: May I recommend _restaurant_name_ , it is located in the _area_ and has a _pricerange_ price range. Is there a specific date, time and number of people? -->
* Are you sure you don t have anything on _restaurant_name_ ? I need the address and postcode.
    - slot{"hotel_status": "NA"}
    - nooffer_hotel: Yes, I am sure. There is no _restaurant_name_ restaurant in our system.   <!-- predicted: inform_restaurant: I found _number_ options for you _restaurant_name_ at Regent Street City Centre, _restaurant_name_ at _number_ Mill Road City Centre, and _restaurant_name_ at _number_ _hotel_name_ Road City Centre -->
* Can you please check again? _restaurant_name_ .
    - slot{"restaurant_status": "available"}
    - inform_restaurant: Sorry about that! I found the _restaurant_name_ at _number_ Norfolk Street City Centre, cb12lf. It s a moderately-priced _food_type_ restaurant.   <!-- predicted: nooffer_restaurant_request_restaurant: I am sorry I can find no place that serves that in the centre area. Would you like to try another area or food type? -->
* Great, thanks so much. Can I also get help booking a room at the _hotel_name_ please?
    - slot{"hotel_status": "available"}
    - request_booking_hotel: sure for what length of stay and how many people please?   <!-- predicted: recommend_hotel_request_booking_hotel: OK, how about _hotel_name_ ? To book a stay I ll need to know the first day you want to stay, how many days, and how many guests. -->
* _number_ people. _number_ nights, starting from _weekday_ . Please give me the reference number, please.
    - slot{"hotel_status": "booked"}
    - book_booking_hotel_reqmore_general: Your booking was successful. The reference number is _reference_ . Can I help you with anything else?   <!-- predicted: book_booking_hotel_inform_hotel_reqmore_general: You are booked at the _hotel_name_ B & B. It is _pricerange_ , with wifi and parking included. Your reference number is _reference_ . Is there anything else? -->
* I would like to book a taxi from the hong house to the _hotel_type_ leaving by _time_
    - slot{"taxi_status": "booked"}
    - inform_taxi: No problem. I booked a _color_ _cartype_ that will pick you up by _time_ .   <!-- predicted: inform_taxi_reqmore_general: The taxi picking you up will be a _color_ _cartype_ Contact number _number_ . Is there anything else I can assist you with? -->
* Wonderful, thank you for everything.
    - Have a great trip! Thank you for contacting us for all your booking needs. Enjoy your trip!
* _number_ more thing. Can you please give me the taxi contact number.
    - inform_taxi: Sure! The contact number is _number_ . The car will be a _color_ _cartype_ .   <!-- predicted: inform_taxi_reqmore_general: Their contact number is _number_ . Do you need any further assistance? -->
* Thank you very much. Have a great day.
    - bye_general: No problem, have a great day!   <!-- predicted: reqmore_general_welcome_general: You re very welcome. Is there anything else at all that I could assist you with? -->


## story_PMUL3663
* Hello, I need a train to Ely on _weekday_ please
    - slot{"train_status": "available"}
    - inform_train_request_train: We have _number_ trains traveling to Ely on _weekday_ . What time would you like to arrive?   <!-- predicted: inform_train: There are several trains departing for _hotel_name_ on _weekday_ . _number_ train departs every hour starting at _time_ -->
* How about _number_ arriving by _time_ departing from _hotel_name_ .
    - slot{"train_status": "unique"}
    - _reference_ will get you to Ely by _time_ on _weekday_ . Should I book you a ticket?
* Yes, that would be great. I ll need tickets for _number_ people. Do you have a reference number?
    - slot{"train_status": "booked"}
    - offerbooked_train: Booking was successful, the total fee is _number_ _reference_ payable at the station .Reference number is _reference_ .   <!-- predicted: greet_general_offerbooked_train_reqmore_general: Great! I have you booked for _number_ tickets on Train _reference_ with a total fee of _number_ _reference_ . Your reference number is _reference_ . Anything else? -->
* I m also looking for a _attraction_name_ . Can you recommend _number_ ?
    - slot{"attraction_status": "available"}
    - greet_general_recommend_attraction: how about _attraction_name_ ? it looks lovely   <!-- predicted: inform_attraction: _hotel_name_ _attraction_name_ of Technology is located on the _area_ side at The Old Pumping Station, Cheddars Lane. Their phone number is _number_ and they charge an entrance fee of _number_ pounds. -->
* That will work. Could you get me the phone number and area its in?
    - slot{"attraction_status": "available"}
    - greet_general_inform_attraction_reqmore_general: Sure! It s in the _area_ area of town, and the phone number is _number_ . Can I help you with anything else?   <!-- predicted: inform_attraction_reqmore_general: Their address is Cherry Hinton Hall, Cherry Hinton Road. The phone number to reach them is _number_ . Is there any other info you need? -->
* You were great today. Thanks so much for all the help. That is all. Goodbye.
    - bye_general_greet_general_welcome_general: It was a pleasure to help. Have a good day. Goodbye.   <!-- predicted: bye_general_welcome_general: You re welcome. Thanks for contacting the _hotel_name_ TownInfo Centre and have a great day! -->


## story_SNG1016
* Do you have information about the _hotel_type_ _hotel_name_ ?
    - slot{"hotel_status": "available"}
    - _hotel_name_ is a _pricerange_ guesthouse in the centre area. It has a _number_ star rating and includes parking and wifi. It s located at _number_ warkworth street. Phone number _number_ .
* Sounds good. Can you book it for _number_ nights checking in on _weekday_ ? There will be _number_ of us.
    - slot{"hotel_status": "NA"}
    - Booking was unfortunately unsuccessful. Can we try another day or a shorter stay?
* Can we try _number_ night?
    - slot{"hotel_status": "booked"}
    - book_booking_hotel_reqmore_general: That did the trick, your booking was successful and your reference number is _reference_ . Is there anything else you need help with today?   <!-- predicted: book_booking_hotel_recommend_hotel: I would recommend the _hotel_name_ , which has what you need. Your booking reference number is _reference_ . Your _number_ night stay will begin _weekday_ . Thank you! -->
* That shall be all. Thanks!
    - Enjoy your stay! Goodbye!


## story_SNG0580
* I d like to find a resturant that serves _pricerange_ _food_type_ food!
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_inform_restaurant: _restaurant_name_ is located in the centre and it is _pricerange_ ! Would you like me to book it for you?   <!-- predicted: inform_booking_hotel_inform_hotel: I have several options for you, most are located in the _area_ area of town, is that acceptable? I can book _number_ for you if you would like. -->
* Yes, go ahead and book it and please send me the address.
    - inform_restaurant_request_booking_restaurant: The address is Regent Street City Centre. What day and time would you like to book? How many people?   <!-- predicted: inform_attraction_reqmore_general: Sure thing. The address is pool way, whitehill road, off newmarket road. Can I help with anything else? -->
* I do not need to book it. What is the postcode and the area please?
    - inform_restaurant: The postcode is cb21db   <!-- predicted: nobook_booking_attraction_reqmore_general: I can not. It doesn t give me the option to book tickets. Just general Information. Can I help you with anything else? -->
* Thanks very much!
    - bye_general_welcome_general: You re welcome! Have a great day! Goodbye.   <!-- predicted: reqmore_general_welcome_general: You re welcome. Is there anything else we can help you with today? -->


## story_MUL2151
* Hello! Can you give me information about trains going to _hotel_name_ and leaving on _weekday_ ?
    - slot{"train_status": "available"}
    - inform_train_request_train: There are over _number_ trains leaving. Do you have a specific time you d like to arrive by?   <!-- predicted: request_train: Where will you be departing from and what will be your departing time? -->
* I am looking to depart from steveage and leave after _time_ please.
    - slot{"train_status": "available"}
    - inform_train: The first train after _time_ is the _reference_ , leaving Stevenage _time_ , arriving _hotel_name_ _time_ . Would this be to your liking?   <!-- predicted: inform_train_offerbook_train: Ah, it appears that the earliest train, _reference_ , leaves at _time_ , but it does arrive by _time_ . If that is okay, I could book that for you. -->
* Yes please can you book seats for _number_ people and give me the reference number?
    - slot{"train_status": "booked"}
    - offerbooked_train: Your booking was completed and the total fee is _number_ _reference_ payable at the station .Reference number is _reference_ .   <!-- predicted: offerbooked_train_reqmore_general: Sure, the train is actually number _reference_ and your reference number is _reference_ . The price will be _number_ _reference_ payable at the station. Is there anything else today? -->
* I also need a place to stay. Can you recommend an _pricerange_ _hotel_type_ in the _area_ ?
    - slot{"hotel_status": "NA"}
    - nooffer_hotel_request_hotel: Unfortunately there are no _pricerange_ hotels in the _area_ . I could check another area if you would like.   <!-- predicted: inform_hotel_select_hotel: We have _number_ entries that match your preferences. Would you prefer _area_ , _area_ , or _area_ ? -->
* Are there any _pricerange_ places to stay in the _area_ ? It doesn t need to be a _hotel_type_ , but I would like free parking.
    - slot{"hotel_status": "NA"}
    - nooffer_hotel_request_hotel: Unfortunately, there are no hotels available with your preferences. Would you like me to find you _number_ in a different price range or area?   <!-- predicted: inform_hotel_nooffer_hotel: There are no hotels that meet that criteria in the _area_ but we do have _number_ moderately priced guesthouses available. Would _number_ of those work? -->
* How about _number_ in the _area_ ?
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel_inform_hotel: I have the _hotel_name_ that is _pricerange_ . Would you like to book a stay?   <!-- predicted: inform_booking_hotel_recommend_hotel: My favorite is _hotel_name_ , it is located in the _area_ area. Would you like me to book this _number_ ? -->
* Yes please, book the _hotel_type_ and give the address with the postcode. Thanks.
    - slot{"hotel_status": "available"}
    - inform_hotel_request_booking_hotel: The addres is _number_ norman way, coldhams business _attraction_type_ , cb13lh. When would you like to stay?   <!-- predicted: inform_hotel_reqmore_general: _hotel_name_ is located on the _area_ end. The address is _number_ _hotel_name_ road, postcode	cb21en. Can I get you any more information? -->
* I d like you to book it for _weekday_ night for _number_ people.
    - slot{"hotel_status": "available"}
    - request_booking_hotel: How many nights would you like to stay?   <!-- predicted: offerbooked_train: Your booking was completed and the total fee is _number_ _reference_ payable at the station .Reference number is _reference_ . -->
* Just _number_ night please.
    - slot{"hotel_status": "NA"}
    - inform_booking_hotel_nobook_booking_hotel: I m sorry, my system is not allowing me to book that location for some reason. Would you like to try again?   <!-- predicted: nobook_booking_hotel: Sorry, it was not successful. Can I check another _hotel_type_ or shorten the stay? -->
* Please try _number_ in the _area_ .
    - inform_hotel_request_hotel: _hotel_name_ is the only _pricerange_ _hotel_type_ in the _area_ . Would you like to try a different price range?   <!-- predicted: nobook_booking_hotel_reqmore_general: I am sorry. _hotel_name_ still has no bookings available for _weekday_ . Would you like to try a different _hotel_type_ ? -->
* Yes, can you try _number_ in the _pricerange_ price range please?
    - slot{"hotel_status": "available"}
    - There are _number_ moderately price hotels there, would you like to try the wankworth house?
* Yes, can I get the post code please?
    - slot{"hotel_status": "available"}
    - Certainly! The post code is cb11ee.
* Alright that s all I needed today thank you so much.
    - bye_general: Thank you for contacting _hotel_name_ TownInfo Centre. Enjoy your trip!   <!-- predicted: bye_general_welcome_general: You are very welcome. You have a lovely day. -->


## story_PMUL4048
* i am looking for a _attraction_name_ in the _area_ part of town.
    - slot{"attraction_status": "NA"}
    - nooffer_attraction: I am sorry, there are no swimming pools located on the _area_ side. Would you be interested in visiting a different attraction?   <!-- predicted: inform_booking_restaurant_inform_restaurant_nooffer_restaurant: There are no _food_type_ restaurants on the _area_ side but there is _number_ on the _area_ side. Would that suffice? -->
* How about a _attraction_type_ instead?
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: Cineworld _attraction_type_ in the _area_ side is located at _hotel_name_ Leisure _attraction_type_ , Clifton Way _reference_ and their phone number is _number_ . Is there any other information I can get you?   <!-- predicted: inform_attraction_recommend_attraction: _attraction_name_ is my favorite place on the _area_ side! I don t have any information on the entrance fee, but their phone is _number_ . -->
* What s the postcode and enterance fee?
    - Unfortunately I don t have any information on the entrance fee. The postcode is cb17dy. Can I help you with anything else?
* I am also looking for a restaurant that serve _food_type_ food in the _area_ side of town.
    - slot{"restaurant_status": "unique"}
    - _restaurant_name_ meets your criteria. Would you like to book a table?
* Yes. Book for _number_ people on _weekday_ at _time_ .
    - slot{"restaurant_status": "booked"}
    - You have a table booked for _number_ people at _time_ on _weekday_ . It will be reserved for _number_ minutes. The reference number is _reference_ .
* I also need to book a taxi to commute between the _number_ . I need to get to the restaurant by the booked time.
    - slot{"taxi_status": "booked"}
    - inform_taxi: Your taxi service is booked. Be expecting a _color_ Volkwagen. If you need to reach them, please call _number_ .   <!-- predicted: greet_general_inform_taxi: No problem! I have booked you a cab that will take you to the restaurant by _time_ . Look for a _color_ _cartype_ taxi. The cab s contact number is _number_ . -->
* Thank you, that is all I need today.
    - I am glad I can help. Enjoy your stay.
* I will. Thank you.
    - welcome_general: You re welcome, have a great day!   <!-- predicted: bye_general_welcome_general: You are quite welcome. Thank you for using our services! -->


## story_PMUL3520
* I need a train going to _hotel_name_ that will depart after _time_ from broxbourne.
    - slot{"train_status": "available"}
    - inform_train: I have train _reference_ that would suit you.   <!-- predicted: inform_train_request_train: What day would you be traveling? There are _number_ trains on that route. There is a train that departs _weekday_ at _time_ and will arrive in Ely at _time_ . -->
* Could you just tell me when that _number_ departs?
    - Train _reference_ departs Broxbourne at _time_ and arrives at _hotel_name_ at _time_ .
* Great can you get me a booking for _number_ people?
    - slot{"train_status": "booked"}
    - Booked! Your reference number is _reference_ . Can I help with anything else?
* Thank you. Yes. I am also looking for an _food_type_ restaurant.
    - slot{"restaurant_status": "available"}
    - inform_restaurant: There are _number_ . _number_ located in the centre that are _pricerange_ in price and _number_ in the _area_ that is _pricerange_ .   <!-- predicted: inform_restaurant_request_restaurant: I have found _number_ _food_type_ restaurants on the _area_ side. There are _number_ _pricerange_ and _number_ _pricerange_ . Did you have a price range in mind? -->
* I want the _number_ in the _area_ , please book me a table for _number_ people.
    - slot{"restaurant_status": "available"}
    - request_booking_restaurant: Certainly. Can you please tell me for what day you would like for me to make this reservation?   <!-- predicted: inform_booking_restaurant_inform_restaurant: I have _number_ restaurants that fit those criteria. _restaurant_name_ , _restaurant_name_ , the _attraction_type_ , _restaurant_name_ and restaurant _number_ _number_ . Which would you like a booking for? -->
* can you book it for _weekday_ after_time_ ?
    - slot{"restaurant_status": "available"}
    - request_booking_restaurant: What time exactly would you like to dine?   <!-- predicted: book_booking_hotel: You re all ready to go! The reference number is _reference_ . -->
* Actually, I d like a moderately priced _food_type_ restaurant in the centre. I need the postcode and address please. Sorry, I keep changing my request!
    - slot{"restaurant_status": "available"}
    - recommend_restaurant_select_restaurant: No problem. How about _restaurant_name_ located at _number_ Saint Andrews Street City Centre with phone number _number_ ? There is also _restaurant_name_ if you prefer.   <!-- predicted: inform_restaurant: I found _number_ options for you _restaurant_name_ at Regent Street City Centre, _restaurant_name_ at _number_ Mill Road City Centre, and _restaurant_name_ at _number_ _hotel_name_ Road City Centre -->
* The Varsity is good. Can I get the postcode please?
    - slot{"restaurant_status": "unique"}
    - The post code is cb23ar. Shall I book it ?
* Yes, please make the booking and email me the reference number.
    - request_booking_restaurant: How many people will the reservation be for?   <!-- predicted: offerbooked_train_reqmore_general: Sure, the train is actually number _reference_ and your reference number is _reference_ . The price will be _number_ _reference_ payable at the station. Is there anything else today? -->
* I do not need a reservation for the restaurnt just information.
    - reqmore_general: Ok. Do you need anything else then?   <!-- predicted: inform_booking_restaurant_request_booking_restaurant: Sure, I d be happy to book this for you. What day, time and how many people will be dining? -->
* No that will be all thank you so much for all your help.
    - bye_general_welcome_general: Okay, thanks for all of your questions. I m glad I was able to help you today. Goodbye. I hope I helped with the reservations.   <!-- predicted: bye_general: Have a great trip! Thank you for contacting us for all your booking needs. Enjoy your trip! -->


## story_MUL0990
* I am looking for information on a restaurant called _restaurant_name_ .
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_inform_restaurant: _restaurant_name_ , on _number_ Mill Road City Centre, is a _pricerange_ _food_type_ restaurant. Would you like me to make a reservation for you?   <!-- predicted: inform_booking_restaurant_recommend_restaurant: _restaurant_name_ is an _food_type_ restaurant in the centre. It s _pricerange_ , but I hear it s great. Would you like me to book it for you? -->
* Not now. What area of town is that in?
    - inform_restaurant: _restaurant_name_ is in the centre of town.   <!-- predicted: nooffer_attraction: Unfortunately there is no good _attraction_type_ on the _area_ end but I can look in other parts of town if you want -->
* Could you give me their phone number?
    - inform_restaurant_reqmore_general: Yes! The phone number for _restaurant_name_ is _number_ . Can I help you with anything else?   <!-- predicted: inform_attraction_reqmore_general: Absolutely. Their phone number is _number_ . Is there anything else I can do for you today? -->
* Yes, I will need the price range for that restaurant and the area it is in as well please.
    - inform_restaurant_reqmore_general: The _restaurant_name_ is in the centre area and in the _pricerange_ price range. Can I help you with anything else?   <!-- predicted: inform_booking_restaurant_inform_restaurant: _restaurant_name_ is a restaurant in the _area_ serving _food_type_ food in the _pricerange_ price range. Do you need more information or want to reserve a table? -->
* Yes I would like to go the Fitzwilliam _attraction_name_ . Can you give me the address?
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: Yes, The Fitzwilliam _attraction_name_ is located on Trumpington Street, postcode cb21rb. Is there anything else I can help you with?   <!-- predicted: inform_attraction_inform_train_reqmore_general: The _attraction_name_ s address is Market Street, postcode cb23nz. There are many trains arriving in Stansted Airport by _time_ . Would you like to narrow your search further? -->
* I also want to book a taxi from the _attraction_name_ to the restaurant. I want to by _time_ .
    - slot{"taxi_status": "booked"}
    - Alright, a _color_ _cartype_ will pick you up at the Fitzwilliam _attraction_name_ . Your contact number is _number_ .
* Thank you! That ll be it today. Goodbye!
    - bye_general_welcome_general: So happy to be of service - have a wonderful day!   <!-- predicted: bye_general: You are welcome. Please contact us again if we can help in the future. Have a great day. -->


## story_PMUL0615
* Hi, I m looking for a restaurant suggestion in _hotel_name_ .
    - request_restaurant: What type of food and price range would you be interested in?   <!-- predicted: request_hotel: Can you please tell me what type of place and if you have any preferences? -->
* I d like some _food_type_ food, please!
    - slot{"restaurant_status": "available"}
    - greet_general_request_restaurant: I can definitely help you with that. What price range were you looking for?   <!-- predicted: request_restaurant: There absolutely are! To narrow down the locations which area would you like and at what price range? -->
* I want something _pricerange_ .
    - slot{"restaurant_status": "available"}
    - request_restaurant: What area do you want the restaurant to be in?   <!-- predicted: inform_attraction_request_restaurant: The Botanic Gardens are in the centre. Would you like the restaurant to also be in the center? Do you have any type of cuisine in mind? -->
* In the centre of town, if possible.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_recommend_restaurant_reqmore_general: _restaurant_name_ is located in17 Hills Road City Centre. can i give you the phon number?   <!-- predicted: inform_restaurant: I found _number_ options for you _restaurant_name_ at Regent Street City Centre, _restaurant_name_ at _number_ Mill Road City Centre, and _restaurant_name_ at _number_ _hotel_name_ Road City Centre -->
* Yes, I would like the phone number. I also need a train on _weekday_ to _hotel_name_ from _location_ . I would like to leave after _time_ .
    - inform_restaurant_request_train: Here is the phone number _number_ . Is there any particular time you would like to arrive by?   <!-- predicted: inform_train_offerbook_train_reqmore_general: The next train leaves _hotel_name_ at _time_ . Would you like more information or can I book it for you? -->
* Any time will do, as long as it leaves after _time_ .
    - slot{"train_status": "unique"}
    - _reference_ leaves _location_ on _weekday_ at _time_ and arrives in _hotel_name_ at _time_ . Will that work for you?
* Is there any that leave earlier than _time_ ?
    - The earliest train after _time_ is the _number_ leaving at _time_ .
* Ok great and what is the arrival time?
    - inform_train_reqmore_general: the train will arrive at _time_ . anything else i can help you with?   <!-- predicted: inform_train_offerbook_train: _reference_ will depart at _time_ and arrive by _time_ . It will cost _number_ pounds. Would you like to reserve seats? -->
* No, thank you, that is all the information I need right now.
    - bye_general_greet_general: Have a good evening. Bye.   <!-- predicted: welcome_general: you re welcome, thank you for using our system. -->


## story_MUL1028
* I m looking for a _number_ star _hotel_type_ .
    - slot{"hotel_status": "available"}
    - There are _number_ hotels that have a _number_ star rating. Is there a price range you are wanting?
* Not really, but it needs to be in the _area_ and include free wifi.
    - slot{"hotel_status": "unique"}
    - The only _hotel_type_ that is in the _area_ with free wifi is _hotel_name_ . Would you like to go ahead and book a room?
* Yes, for _number_ nights please.
    - slot{"hotel_status": "available"}
    - Before I can book a room for you I need to know a few details. What day would you arrive? How many days would you stay? How many people are staying?
* I just need the phone number for the _hotel_type_ please.
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel_inform_hotel: The phone number for the _hotel_name_ is _number_ . Can I help you with booking for this _hotel_type_ ?   <!-- predicted: greet_general_inform_booking_hotel_inform_hotel: Sure, I have it right here. Its a _pricerange_ priced guesthouse with a _number_ star rating, free internet and parking. Phone number is _number_ can I book it for you? -->
* No, but I d like to know the address and phone number for wandlebury country _attraction_type_ .
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: The phone number for Wandlebury Country _attraction_type_ is _number_ . Is there anything else I can assist you with?   <!-- predicted: greet_general_inform_hotel_reqmore_general: Of course! The address of the _hotel_name_ is kingfisher way, hinchinbrook business _attraction_type_ , huntingdon and it s phone number is _number_ , would you like anything else? -->
* May I also get the address for wandlebury country _attraction_type_ please.
    - inform_attraction: The number is _number_ .   <!-- predicted: inform_attraction_inform_train_reqmore_general: The _attraction_name_ s address is Market Street, postcode cb23nz. There are many trains arriving in Stansted Airport by _time_ . Would you like to narrow your search further? -->
* What is the address, please?
    - inform_attraction: The address is wandlebury ring, gog magog hills, babraham.   <!-- predicted: inform_attraction_reqmore_general: The _hotel_name_ Punter, the address is 251a Chesterton Road, post code cb41as. Would you like to know any more info on boats in _hotel_name_ ? -->
* Was there anything else I could help you with today?
    - reqmore_general: Have all of your needs been met for today? Do you require further assistance with anything?   <!-- predicted: greet_general_inform_hotel_recommend_attraction: Yes, the Lovell is indeed a _number_ star location. Might I suggest the _hotel_name_ Arts Theatre for your _attraction_type_ during your stay? It s a highly recommended experience. -->
* No. I have everything I need. Thank you and goodbye.
    - bye_general: Thank you for using our service. Have a great day!   <!-- predicted: bye_general_reqmore_general_welcome_general: Okay, great. I m glad I could help. Don t hesitate to contact us again if you need additional assistance. Goodbye. -->


## story_PMUL0630
* I would like for you to find a train that leaves on _weekday_ after _time_ .
    - slot{"train_status": "available"}
    - greet_general_request_train: Okay, let me look that up for you. Do you have a destination or a departure site?   <!-- predicted: inform_train_request_train: There are _number_ trains traveling on _weekday_ . Where will you be departing from and where is your destination? -->
* I m going to _hotel_name_ from _location_ .
    - slot{"train_status": "unique"}
    - The _reference_ leaves _hotel_name_ at _time_ and gets into _location_ by _time_ . Will that work for you?
* Yes, that will work. For _number_ people, please.
    - slot{"train_status": "booked"}
    - Reference number is _reference_ . Will you need anything else?
* Do you think you can find me a great _food_type_ food place. I want something really fancy. It s for an anniversary dinner.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_restaurant_select_restaurant: there are _number_ in town. did you have a certain part of town you want to dine in? i have some in the centre and _area_ .   <!-- predicted: inform_restaurant: There is _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _restaurant_name_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _area_ _food_type_ , _food_type_ , _food_type_ , and _food_type_ food available in the centre. -->
* Out of the _number_ , how many are _pricerange_ ? I would like an _pricerange_ restaurant location doesn t matter to much.
    - inform_restaurant: They are all _pricerange_ .   <!-- predicted: inform_restaurant_select_restaurant: I have the _restaurant_name_ which serves _food_type_ . I also have _restaurant_name_ that serves _food_type_ food. Which would you prefer? -->
* How about an _food_type_ joint?
    - inform_restaurant_recommend_restaurant: Ok I suggest _restaurant_name_ it is _pricerange_ and located in the centre. They serve _food_type_ food.   <!-- predicted: inform_restaurant: I found _number_ options for you _restaurant_name_ at Regent Street City Centre, _restaurant_name_ at _number_ Mill Road City Centre, and _restaurant_name_ at _number_ _hotel_name_ Road City Centre -->
* perfect, what is their phone
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_inform_restaurant: The phone number is _number_ . Would you like me to book reservations for that?   <!-- predicted: inform_attraction_reqmore_general: Absolutely. Their phone number is _number_ . Is there anything else I can do for you today? -->
* Not at this time, thank you.
    - reqmore_general: Is there anything else I can do for you today?   <!-- predicted: bye_general_welcome_general: My pleasure. Please call again if you need more help. I am happy to be of service. -->
* No thank you that will be all! Bye!
    - welcome_general: You re welcome, have a great day!   <!-- predicted: bye_general: I hope you enjoy your trip. Have a great day and goodbye. -->


## story_MUL0014
* I m looking for a place to stay in the _area_ of town. It doesn t need to have free parking.
    - slot{"hotel_status": "available"}
    - inform_hotel_select_hotel: There are _number_ hotels that are in the area you are looking for. Would you prefer a _number_ or _number_ star rated _hotel_type_ ?   <!-- predicted: inform_hotel_request_hotel: There are _number_ matching your request. Do you have any preferences such as area, price, parking, or internet? -->
* I don t care about the star rating as long as it s _pricerange_ .
    - slot{"hotel_status": "available"}
    - recommend_hotel_reqmore_general: _hotel_name_ is the only _pricerange_ _hotel_type_ in the _area_ area. Would you like any more information on this location?   <!-- predicted: inform_hotel: That narrows it down to _number_ choices. I have the _hotel_name_ and the _hotel_name_ . Both are hotels located in the _area_ . Both have a _number_ star rating. -->
* That is perfect can you book that for me please.
    - slot{"hotel_status": "booked"}
    - book_booking_hotel_inform_hotel: _hotel_name_ is located in the _area_ . It has a _number_ star rating and is _pricerange_ . There is free parking and internet. I have booked it for you.   <!-- predicted: book_booking_restaurant: Certainly, the reference number is _reference_ . -->
* Thank you. Can you make sure that it s for _number_ people staying for _number_ nights, starting _weekday_ ? Also, would you mind sending me the reference number?
    - slot{"hotel_status": "booked"}
    - book_booking_hotel: You re all set the reference is _reference_ .   <!-- predicted: book_booking_hotel_reqmore_general: I have made the reservation. The reference number is _reference_ . Is there anything else you need today? -->
* I d also like to try a restaurant a friend mentioned. _restaurant_name_ ?
    - slot{"restaurant_status": "unique"}
    - _restaurant_name_ is an _food_type_ restaurant on the _area_ side, _number_ Milton Road Chesterton. Phone number is _number_ . Would you like me to book a reservation?
* Yes I d like a reservation for _number_ at _time_ , please.
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_request_booking_restaurant: Sure, i can make a reservation, is that going to be on _weekday_ ?   <!-- predicted: book_booking_restaurant: Great it s all set _reference_ is the reference number -->
* Yes, the same day. Can I get the reference number, please?
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_reqmore_general: Your table has been successfully booked for _weekday_ . Your reference number is _reference_ . Is there anything else I can help you with?   <!-- predicted: offerbooked_train_reqmore_general: I was able to book _number_ tickets for you on that train. Your reference number is _reference_ . Is there anything else for today? -->
* No that is all. Thank you!
    - bye_general_welcome_general: Okay! Thank you for calling.   <!-- predicted: bye_general_greet_general_welcome_general: Enjoy your visit. Thank you for contacting _hotel_name_ TownInfo Centre. Good bye. -->


## story_MUL1657
* Hi, I need a train to broxbourne, please.
    - slot{"train_status": "available"}
    - What day will you be traveling?
* I will be leaving on _weekday_ and I am departing from _hotel_name_ .
    - slot{"train_status": "available"}
    - There are _number_ trains that day do you have a time you will be traveling?
* I need to arrive by _time_ and I want to book it for _number_ people.
    - slot{"train_status": "unique"}
    - I have _number_ that leaves at _time_ and arrives at _time_ . Would you like be to book that _number_ ?
* Yes please, book that for _number_ people and I need the reference number.
    - slot{"train_status": "booked"}
    - The booking was successful and your feference number is _reference_ . May I help you with anything else today?
* I am looking for a restaurant called _restaurant_name_ and would like to book the same _number_ people there on the same day. Is that a possibility?
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_inform_restaurant_request_booking_restaurant: _restaurant_name_ is a _food_type_ restaurant on the _area_ side falling in the _pricerange_ price range. I can try making a reservation for you; how many people in your party?   <!-- predicted: inform_booking_restaurant_inform_restaurant: _restaurant_name_ is an _food_type_ restaurant on the _area_ side, _number_ Milton Road Chesterton. Phone number is _number_ . Would you like me to book a reservation? -->
* Like I mentioned previously, it ll be for the same _number_ people, on the same day (_weekday_ ), at _time_ please.
    - slot{"restaurant_status": "booked"}
    - Your booking was successful. The reference number is _reference_ . Is there anything else I can help you with?
* That will be all. Thank you for your help!
    - bye_general: Thank you for using _hotel_name_ TownInfo centre. Please remember us for your future travel needs.   <!-- predicted: bye_general_welcome_general: You are so welcome. Enjoy your meal. -->


## story_SNG01983
* i want a reservation that has _pricerange_ price and should be in the _area_
    - slot{"hotel_status": "available"}
    - inform_hotel: we have _number_ with your specification   <!-- predicted: recommend_hotel: If price is not an issue, I recommend the _pricerange_ _hotel_name_ . If you want something cheaper, I recommend _hotel_name_ . -->
* Oh, I also need it to have free parking and I want a _hotel_type_ .
    - slot{"hotel_status": "available"}
    - recommend_hotel: How about _hotel_name_ ? It looks great.   <!-- predicted: inform_hotel_request_hotel: I have _number_ hotels in town matching that requirement ranging from _number_ to _number_ stars guest houses and hotels. Do you have a preference for the area? -->
* Sure, please book it for _number_ person for _number_ nights starting on _weekday_ .
    - slot{"hotel_status": "NA"}
    - Booking was unsuccessful. Perhaps another day or shorter stay?
* how about starting on _weekday_ ?
    - slot{"hotel_status": "booked"}
    - Booking was successful for _weekday_ . Reference number is _reference_ .
* Thank you so much! That is all I needed.
    - Thank you goodbye


## story_PMUL1895
* Can you find a _hotel_type_ named _hotel_name_ for me? Thanks.
    - slot{"hotel_status": "unique"}
    - Sure, it is a guesthouse in the _area_ . Would you like me to book a room for you?
* Can you tell me if they have free internet?
    - inform_hotel_reqmore_general: Yes, they have free wifi. Do you need anything else?   <!-- predicted: inform_booking_hotel_inform_hotel: Yes, they both do. The _hotel_name_ B&B is our inexpensive _number_ star guesthouse. Would you like me to see if I could book you room? -->
* I would also like a train that leaves on _weekday_ and arrive by _time_ .
    - slot{"train_status": "available"}
    - There are many trains moving on _weekday_ , can I get your preferred point of departure and arrival?
* I will be going from _hotel_name_ to Bishops Stortford.
    - slot{"train_status": "available"}
    - There are multiple trains leaving that match your request. When is the earliest you would want to leave?
* I need to arrive by _time_ I don t have a preference on departing time.
    - slot{"train_status": "available"}
    - inform_train_select_train: _reference_ leaves at _time_ and arrives at _time_ . Would this _number_ work for you?   <!-- predicted: request_train: Could you please mention your day of travel? -->
* Yeah that works for me. Could you book that train for _number_ people and then give me the reference number?
    - slot{"train_status": "booked"}
    - inform_train_offerbooked_train_reqmore_general: Booking was successful, the total fee is _number_ _reference_ payable at the station. Reference number is _reference_ . Will there be anything else today?   <!-- predicted: offerbooked_train_reqmore_general: Sure, the train is actually number _reference_ and your reference number is _reference_ . The price will be _number_ _reference_ payable at the station. Is there anything else today? -->
* No, that s all I needed. Thank you very much!
    - bye_general: I m glad I could have been of service!   <!-- predicted: welcome_general: you re welcome, thank you for using our system. -->


## story_SNG0338
* I need a train that leaves on _weekday_ with an arrival of _time_ .
    - slot{"train_status": "available"}
    - request_train: Where will you be travelling to and from?   <!-- predicted: inform_train_request_train: There are _number_ trains traveling on _weekday_ . Where will you be departing from and where is your destination? -->
* I m traveling from _hotel_name_ to the _location_ .
    - slot{"train_status": "available"}
    - inform_train: The _reference_ leaves at _time_ and arrives by _time_ . Is that alright?   <!-- predicted: inform_train_request_train: I have several trains that will get you to Cabridge on time. Is there a particular departure time you would like? -->
* Yes, that sounds fine. I need _number_ tickets please.
    - slot{"train_status": "booked"}
    - Great. The reference number is _reference_ and the total fee is _number_ _reference_ . Can I help with anything else?
* Thanks, that s all I need. Have a nice day.
    - bye_general: You re very welcome. Have a safe trip!   <!-- predicted: bye_general_reqmore_general_welcome_general: Okay, great. I m glad I could help. Don t hesitate to contact us again if you need additional assistance. Goodbye. -->


## story_PMUL1657
* I need to catch a train out of _hotel_name_ after _time_ .
    - slot{"train_status": "available"}
    - request_train: Could you provide me with your destination?   <!-- predicted: inform_train_request_train: There are _number_ trains leaving _hotel_name_ after that time. What is your destination and day of travel? -->
* I d like to go to Stevenage.
    - slot{"train_status": "available"}
    - request_train: What day do you need the train?   <!-- predicted: inform_train: Train _reference_ departing from _hotel_name_ at _time_ and arriving at stansted airport at _time_ will be the best option for you. -->
* I need to leave on _weekday_ . Can you book me for _number_ people and can I get the reference number?
    - slot{"train_status": "booked"}
    - inform_train_offerbooked_train: _reference_ leaves _hotel_name_ at _time_ . The Booking was successful, the total fee is _number_ _reference_ payable at the station .Reference number is _reference_ .   <!-- predicted: offerbooked_train_reqmore_general: Sure, the train is actually number _reference_ and your reference number is _reference_ . The price will be _number_ _reference_ payable at the station. Is there anything else today? -->
* Perfect. Now if you can just help me find the _hotel_name_ _hotel_type_ ?
    - slot{"hotel_status": "available"}
    - Certainly! The _hotel_name_ _hotel_type_ is located on the _area_ side at _number_ newmarket road.
* Great, thanks! I think that s all I need today. Good bye.
    - Thank you for letting us help. Good bye


## story_SNG0755
* Hi, I d like to find a place to stay that includes free wi-fi.
    - slot{"hotel_status": "available"}
    - I have quite a few places that offer wifi, is there is a certain price range you are looking for?
* Something _pricerange_ would be good.
    - slot{"hotel_status": "available"}
    - inform_hotel_request_hotel: I have about _number_ different places. Do you have a preference on the area of town?   <!-- predicted: inform_hotel_select_hotel: I have _number_ options with those specifications. The _hotel_name_ and the _hotel_name_ both with free wifi and parking. Which would you prefer? -->
* No not really. But I would prefer a _hotel_type_ and like both free wifi and parking if possible.
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel_inform_hotel: _hotel_name_ is a _hotel_type_ in the _area_ that is _pricerange_ and has both free internet and wifi. Would you like to book this?   <!-- predicted: inform_booking_hotel_inform_hotel_recommend_hotel: All the _number_ hotels are _number_ star hotels. I recommend the _hotel_name_ or the _hotel_name_ . Should I book _number_ of those for you and your party? -->
* That s fine. I ll need it for _number_ nights starting on _weekday_ .
    - slot{"hotel_status": "NA"}
    - nobook_booking_hotel_request_booking_hotel: Unfortunately, that day doesn t work. Can we try booking another day or a shorter stay, perhaps?   <!-- predicted: inform_hotel: _hotel_name_ is a _number_ -star _hotel_type_ in the center of town. Its address is Sleeperz _hotel_type_ , _location_ . -->
* Is there another _hotel_type_ that matches that criteria?
    - Unfortunately that s the only _hotel_type_ that suits your criteria.
* I will try and restate so you can look again, I need free wifi and parking, _pricerange_ place, type of room does not matter.
    - inform_hotel_request_hotel: There are _number_ places that match your criteria. What part of town would you like to stay in?   <!-- predicted: inform_hotel_nobook_booking_hotel_request_booking_hotel: Sorry, the _hotel_name_ is not able to accomodate you either. I checked with the other moderately priced _number_ star lodgings with free wifi, and none have those dates available. Will any other stay work for you? -->
* It doesn t matter. Whatever is available nearby will be fine.
    - slot{"hotel_status": "available"}
    - request_booking_hotel: I will give it a try again. How many people will there be?   <!-- predicted: recommend_hotel: If price is not an issue, I recommend the _pricerange_ _hotel_name_ . If you want something cheaper, I recommend _hotel_name_ . -->
* there are _number_ of us.
    - slot{"hotel_status": "booked"}
    - book_booking_hotel_inform_hotel_reqmore_general: You are booked at the _hotel_name_ B & B. It is _pricerange_ , with wifi and parking included. Your reference number is _reference_ . Is there anything else?   <!-- predicted: inform_hotel_offerbooked_train: Booking was successful, the total fee is _number_ _reference_ payable at the station .Reference number is _reference_ . _hotel_name_ is located in the _area_ . -->
* No. That is all!
    - bye_general: Have a nice day and enjoy your stay. Bye.   <!-- predicted: bye_general_greet_general_welcome_general: Thank you for using our service. Call us anytime. Take care. Goodbye. -->
* Thank you for your assistance.
    - bye_general: You are welcome. Have a great time   <!-- predicted: bye_general_welcome_general: Thank you for calling _hotel_name_ TownInfo centre, it was a pleasure to assist you. Have a wonderful trip! -->


## story_MUL0533
* I m planning a trip to _attraction_name_ .
    - slot{"attraction_status": "available"}
    - greet_general_inform_attraction_reqmore_general: Great! _attraction_name_ is in town. What information can I help you with?   <!-- predicted: inform_restaurant_request_restaurant_select_restaurant: there are _number_ in town. did you have a certain part of town you want to dine in? i have some in the centre and _area_ . -->
* I d like to know what type of attraction it is, the entrance fee, and what area it s in, please.
    - inform_attraction_reqmore_general: It is a _attraction_name_ in the centre of town. There is no entrance fee. May I help you with anything else?   <!-- predicted: inform_attraction: _attraction_name_ is in the center and it s known for it s _attraction_type_ . The entrance fee is free. -->
* I m looking for a train to _hotel_name_ leaving after _time_ .
    - slot{"train_status": "available"}
    - request_train: What day of the week are you traveling and what is your departure station?   <!-- predicted: inform_train_request_train: There are very many trains that fit your requirements, where are you leaving from and what day would you like to leave? -->
* I want to depart from _location_ on _weekday_ .
    - slot{"train_status": "unique"}
    - TrainID _reference_ departs at _time_ . Their price is _number_ pounds. Would you like to book this train?
* What time does the train arrive?
    - inform_train: The _reference_ arrives by _time_ .   <!-- predicted: inform_train_offerbook_train: The train ID for that is _reference_ and the travel time is _number_ minutes. Would you like me to book you a seat? -->
* That sounds perfect. Can you go ahead and book that for me?
    - greet_general_request_train: Certainly! Are you traveling by yourself or would you need more than _number_ ticket?   <!-- predicted: request_train: Certainly! Can you tell me how many tickets you will be needing? -->
* I just need the travel time and price please
    - The travel time is _number_ minutes and it is _number_ pounds.
* That is all I need. Thank you.
    - reqmore_general: Are you certain you don t need further assistance?   <!-- predicted: bye_general: You re very welcome! Thanks for contacting _hotel_name_ TownInfo centre and have a great day! -->
* Yes. Have a nice day.
    - bye_general_welcome_general: It has been my pleasure. Feel free to contact us if you need any assistance.   <!-- predicted: request_booking_restaurant: Can you tell me the day and time you d like to eat, and how many people I should book the table for? -->


## story_PMUL1311
* Are there any good places to visit in the centre of town? Thankyou.
    - slot{"attraction_status": "available"}
    - inform_attraction_request_attraction: There are loads of fun, interesting attractions in city centre. Do you have anything specific in mind? _attraction_type_ , boats, concerthalls, museums, colleges, nightclubs, parks, swimmingpools, theatres?   <!-- predicted: inform_attraction: Yes, _number_ of them are free to visit and there are _number_ that have an entrance fee of _number_ . -->
* I don t have a preference. Please pick something for me.
    - slot{"attraction_status": "available"}
    - There are several Churches, _attraction_type_ attractions. Would you like _number_ of them?
* Pick _number_ of the best churches for me and let me know the entrance fee please.
    - slot{"attraction_status": "available"}
    - _attraction_name_ is located on Jesus Lane and the entrance is fee.
* I am also looking for a train. The train should depart from _hotel_name_ and should arrive by _time_ .The train should leave on _weekday_ and should go to _location_
    - slot{"train_status": "available"}
    - request_train: What day are you looking to travel?   <!-- predicted: inform_train_request_train: What day would you be traveling? There are _number_ trains on that route. There is a train that departs _weekday_ at _time_ and will arrive in Ely at _time_ . -->
* _weekday_ please.
    - inform_train_reqmore_general: The _reference_ arrives by _time_ . Will that work for you?   <!-- predicted: request_taxi: Okay what time will you be leaving. -->
* Yes,can you book it for me and get a reference number ?
    - The system is ready to go on the booking, how many people?
* What is the departure time for time for _reference_ , also I would like to know the travel time as well?
    - inform_train_request_train: The departure time is _time_ . The travel time is _number_ minutes. How many are traveling?   <!-- predicted: inform_train: The last train with ID _reference_ departing _location_ to _hotel_name_ on _weekday_ will be the best option for you. It will depart by _time_ and arrive by _time_ . -->
* I actually won t need any tickets. Thank you for your help!
    - bye_general_welcome_general: You re welcome. Enjoy your stay.   <!-- predicted: reqmore_general_welcome_general: No problem at all! Is there anything more I can help you with today? -->


## story_PMUL0441
* I m trying to find a _hotel_type_ called _hotel_name_ . Can you help?
    - slot{"hotel_status": "unique"}
    - Yes _hotel_name_ is located on 517a coldham lane in the _area_ . Would you like me to book a room for you?
* book for me bed and breakfast for _number_ people from tommorrow.
    - slot{"hotel_status": "available"}
    - request_booking_hotel: How many days will you be staying?   <!-- predicted: request_booking_restaurant: Okay, at what time, what day, and for how many people please? -->
* Actually don t book it just yet on second thought. Can you advise how many stars it has and the price first?
    - _hotel_name_ is a _number_ star guesthouse in the _pricerange_ price range.
* I need a a restaurant. The restaurant should be in the _area_ and should serve _food_type_ food.The restaurant should be in the _pricerange_ price range
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_recommend_restaurant: I would suggest _restaurant_name_ then. Would you like for me to book it?   <!-- predicted: inform_booking_restaurant_inform_restaurant: I have _number_ restaurants that fit those criteria. _restaurant_name_ , _restaurant_name_ , the _attraction_type_ , _restaurant_name_ and restaurant _number_ _number_ . Which would you like a booking for? -->
* Yes I would. For _number_ people on _weekday_ at _time_ .
    - slot{"restaurant_status": "booked"}
    - I was able to get that table booked for you for _weekday_ . The restaurant will hold the table for _number_ minutes. Your reference number is _reference_ .
* Thank you so much, goodbye!
    - welcome_general: you re welcome, have a great day!   <!-- predicted: bye_general_welcome_general: You are so welcome. Enjoy your meal. -->


## story_PMUL0522
* I m looking for a high quality restaurant in _hotel_name_ please.
    - slot{"restaurant_status": "available"}
    - request_restaurant: Is there a specific type of cuisine that you would prefer?   <!-- predicted: inform_restaurant_request_restaurant: There are _number_ _pricerange_ restaurants in town. Do you have a food preference or an area of town you want to eat in? -->
* No, I just want it to be _pricerange_ and located in the _area_ .
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_recommend_restaurant: I have the _restaurant_name_ it serves _food_type_ . Would you like to make reservations there?   <!-- predicted: inform_booking_restaurant_inform_restaurant: I have _number_ restaurants that fit those criteria. _restaurant_name_ , _restaurant_name_ , the _attraction_type_ , _restaurant_name_ and restaurant _number_ _number_ . Which would you like a booking for? -->
* Yes, please. There are _number_ of us coming on _weekday_ . Maybe around _time_ ?
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_reqmore_general: I was able to book a table for you. The Reference number is _reference_ . Is there anything else you need?   <!-- predicted: book_booking_restaurant: Your table for _number_ at _restaurant_name_ at _time_ this _weekday_ was successful. The table will be reserved for _number_ minutes. Your Reference number is _reference_ . -->
* I also need a train.
    - Where will you be departing from and what will be your departing time?
* I need to get to _hotel_name_ by _time_ on _weekday_ . I ll be leaving from Stevenage.
    - slot{"train_status": "unique"}
    - offerbook_train: how about _reference_ ? it leaves at _time_   <!-- predicted: inform_train_offerbook_train: _reference_ will depart at _time_ and arrive by _time_ . It will cost _number_ pounds. Would you like to reserve seats? -->
* Great, still figuring out transportation arranagments so no need to book, how long is the travel time?
    - travel time is _number_ minutes. Is there anything else I can help with?
* Can you give me the ticket price, please?
    - greet_general_inform_train_reqmore_general: Of course! The price is _number_ pounds. Can I help you with anything else today?   <!-- predicted: inform_hotel_request_hotel: I show _number_ hotels in the _area_ , _number_ is _pricerange_ and _number_ is _pricerange_ . I also show _number_ _pricerange_ _number_ star _hotel_type_ in the _area_ . Which area do you prefer? -->
* That s all for today, thank you
    - Alright thank you and have a wonderful rest of your day!


## story_PMUL2209
* Can you please tell me about _attraction_name_ ?
    - slot{"attraction_status": "available"}
    - inform_attraction: Yes, it is a _attraction_type_ located at Cherry Hinton Hall, Cherry Hinton Road. Phone is _number_ .   <!-- predicted: inform_attraction_reqmore_general: There are _number_ colleges in town centre. _hotel_name_ and Caius _attraction_name_ is on trinity street with free entrance. Do you want more information on any others? -->
* Thank you. Can you please tell me the area of town this is in?
    - inform_attraction_reqmore_general: Yes it is on the _area_ side. Anyhting else I may help you with today?   <!-- predicted: inform_attraction: Sure, I found it! It s located at _number_ Wheeler Street. It s a _attraction_type_ in the city s centre and it has a _number_ pounds entrance fee. -->
* I also need some help finding a place to dine at, can you look that up for me?
    - request_restaurant: Yes, could you tell me what type of food you would like and the part of town you prefer?   <!-- predicted: request_hotel: Can you please tell me what type of place and if you have any preferences? -->
* I want to eat in the _area_ .
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_restaurant: I have _number_ restaurants available. What type of food would you like?   <!-- predicted: inform_restaurant: The top _number_ places serving _food_type_ cuisine are _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Would you like more options? -->
* I don t have a food preference.
    - request_restaurant: what about price range?   <!-- predicted: select_restaurant: The restaurants are _restaurant_name_ , _restaurant_name_ and _restaurant_name_ . -->
* that should be _pricerange_
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_inform_restaurant: I have _attraction_name_ hut cherry hinton located at G4 _hotel_name_ Leisure _attraction_type_ Clifton Way Cherry Hinton. Would you like reservations?   <!-- predicted: inform_booking_restaurant_recommend_restaurant: I would recommend _restaurant_name_ . It is an _pricerange_ restaurant in the center. Would you like to book a reservation? -->
* I would for _number_ people please.
    - slot{"restaurant_status": "available"}
    - What day and time would you like to book the table?
* _weekday_ at... oh... _time_ .
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_reqmore_general: Your table is reserved, ref _reference_ . Can I help you with anything else today?   <!-- predicted: book_booking_restaurant: Okay, I successfully booked that table for you at _number_ for your party. Please arrive on time, as the table is only reserved for _number_ minutes.Your reference number is _reference_ . -->
* i need to find a taxi to commute me between these _number_ paces that arrives at the restaurant by my booked time.
    - slot{"taxi_status": "booked"}
    - inform_taxi_reqmore_general: You are all set! Be looking for a _color_ _cartype_ . Anything else?   <!-- predicted: inform_taxi: Okay! Your taxi is a _color_ _color_ _cartype_ . Contact number _number_ -->
* What s the taxi s phone number?
    - Their contact number is _number_ should you need to contact them!
* Great, that s all I need, thanks so much for your help! Have a great day!
    - No thank you that will be all


## story_MUL0828
* I m looking for info about a restaurant in _hotel_name_ called _restaurant_name_ .
    - slot{"restaurant_status": "available"}
    - inform_restaurant: Of course, the address is _number_ Regent Street City Centre, postcode cb21dp. Did you want the phone number as well?   <!-- predicted: inform_booking_restaurant_inform_restaurant: Absolutely! They are a great _food_type_ restaurant in the centre of town. They are on the _pricerange_ side. Would you like help in reserving a table? -->
* No, but I do want its area and price range.
    - Certainly, it is in the centre area and is in the _pricerange_ price range. Is there anything else I can help you with?
* Yes can you help me find something to do in the center of town that involves looking at a _attraction_name_ ?
    - slot{"attraction_status": "available"}
    - inform_attraction_recommend_attraction: We actually have _number_ colleges in the center of town! _attraction_name_ on Regent Street is free to get in and a great place to visit.   <!-- predicted: inform_attraction_request_attraction: There are _number_ listings for colleges at the city centre, plenty to check out. Do you need info on any particular _attraction_name_ ? Or narrow it down by entrance fee? -->
* Could I get the phone number for _attraction_name_ ?
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: No problem. They can be reached at _number_ . Is there anything else I can help with?   <!-- predicted: greet_general_inform_attraction_reqmore_general: Of course. It is a _attraction_name_ in the centre. Their phone number _number_ . Can I tell you anything else? -->
* Yes please. I d like to find a restaurant called _restaurant_name_ . Do you have a listing for them?
    - slot{"attraction_status": "unique"}
    - inform_booking_attraction_inform_restaurant: Yes. They serve _food_type_ food and are in the centre. Would you like to book a reservation?   <!-- predicted: inform_restaurant: There is _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _restaurant_name_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _area_ _food_type_ , _food_type_ , _food_type_ , and _food_type_ food available in the centre. -->
* How much is entrance fee and may i also get a number for them?
    - inform_restaurant: I do not have an entrance fee but if you are wanting to know the price range, _restaurant_name_ is a more _pricerange_ restaurant. Their phone number is _number_ .   <!-- predicted: inform_attraction_reqmore_general: Cineworld _attraction_type_ _number_ . I m sorry but the entrance fee is not listed. Is there anything else I can help you with today? -->
* Is there an entrance fee for _attraction_name_ ?
    - It is free to enter.
* Ok, thank you! Goodbye
    - bye_general_welcome_general: You re welcome. Goodbye!   <!-- predicted: bye_general_reqmore_general_welcome_general: Okay, great. I m glad I could help. Don t hesitate to contact us again if you need additional assistance. Goodbye. -->


## story_MUL1278
* Hello, I m looking for a place to stay. I d like it to be in the _area_ and have zero stars.
    - slot{"hotel_status": "unique"}
    - The city centre _area_ b and b matches your request. Would you like to book it?
* Do they offer free parking?
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel_inform_hotel: Yes, they offer both free parking and free internet. Can I make a reservation for you?   <!-- predicted: inform_hotel: Actually, _hotel_name_ doesn t meet your requirements. But I do have other options that are moderately priced, such as _hotel_name_ , Arbury Lodge Guesthouse, and _hotel_name_ . -->
* I would like you to pick _number_ , and tell em the adress and what type of room it is please.
    - inform_hotel_request_booking_hotel: There are at 328a Histon Road and it is a guesthouse. I will need the dates you want to stay in order to book it please.   <!-- predicted: inform_hotel_recommend_hotel: I would recommend the _hotel_name_ . It is indeed a _hotel_type_ despite it s name and is very cute. -->
* I don t think I ll make that reservation just yet, but can you help me find an _pricerange_ restaurant in the same areas as the _hotel_type_ ?
    - slot{"restaurant_status": "available"}
    - request_restaurant: Sure. do you have any kind of food preference?   <!-- predicted: inform_booking_hotel_inform_hotel: The _hotel_name_ is at _number_ Chesterton Road, and their postcode is cb41er. Would you like to book a room or are you just looking for information right now? -->
* Yes please make sure it is _food_type_ and _pricerange_ price range.
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_inform_restaurant_select_restaurant: I have _number_ choices for you then, _restaurant_name_ or _restaurant_name_ . Do either of those sound good? I would be happy to book a reservation for you.   <!-- predicted: inform_booking_restaurant_recommend_restaurant: I would recommend _restaurant_name_ . It is an _pricerange_ restaurant in the center. Would you like to book a reservation? -->
* Let s try _restaurant_name_ and can I get the reference number please.
    - request_booking_restaurant: I ll need some more information to make the reservation first. What day and time, and for how many people?   <!-- predicted: inform_restaurant_request_booking_restaurant: Yes, the _restaurant_name_ is in the _area_ . I would be happy to book a table for you if you can tell me the day, time, and number of people. -->
* It ll be _number_ people at _time_ on _weekday_ .
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_reqmore_general: The booking was successful. Your reference number is _reference_ . Can I help you with anything else?   <!-- predicted: book_booking_restaurant: Here is your booking information Booking was successful. The table will be reserved for _number_ minutes.Reference number is _reference_ . -->
* No, you have answered all my questions. Thank you very much. Good bye.
    - Thank you for using _hotel_name_ TownInfo centre. Please remember us for all of your future travel needs.


## story_PMUL1173
* I d like to find a place to go in the center of town.
    - slot{"attraction_status": "available"}
    - recommend_attraction: How about _attraction_name_ ?   <!-- predicted: inform_hotel_request_hotel: There are _number_ hotels which are _number_ stars, _number_ in the _area_ and _number_ in the centre. Is there an area which you prefer? -->
* Ok, what s the address and postcode?
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: Market Square, town center. Post code cb23pq. Anything else?   <!-- predicted: inform_attraction_inform_train_reqmore_general: The _attraction_name_ s address is Market Street, postcode cb23nz. There are many trains arriving in Stansted Airport by _time_ . Would you like to narrow your search further? -->
* Yes, I also need to book a train for _weekday_ . Can you help me with that?
    - slot{"train_status": "available"}
    - inform_train_request_train: You are looking for a train to _hotel_name_ , correct? Where will you be traveling from?   <!-- predicted: request_train: Certainly, where will you be departing from and what time would you like to leave? -->
* I will be travelling from _hotel_name_ actually and going to _location_ .
    - slot{"train_status": "available"}
    - request_train: What day will you be traveling?   <!-- predicted: inform_train_request_train: Those trains run every _number_ hours, starting at _time_ . What time would you like to depart? -->
* I would like to leave on _weekday_ .
    - request_train: And at what time would you like to travel?   <!-- predicted: inform_train_reqmore_general: I apologize! There are _number_ trains leaving near your requested time. _number_ at _time_ and _number_ at _time_ . Will _number_ of those work? -->
* I would like to arrive by _time_ . Could I get the price please?
    - slot{"train_status": "available"}
    - inform_train_select_train: I have _number_ that arrives at _time_ and another at _time_ . Both cost _number_ pounds. Do you have a preference?   <!-- predicted: inform_train_offerbook_train_request_train: the _reference_ will get you there by _time_ , how many tickets? -->
* No preference. You choose. Thanks!
    - request_train: How many tickets would you like?   <!-- predicted: recommend_hotel: If price is not an issue, I recommend the _pricerange_ _hotel_name_ . If you want something cheaper, I recommend _hotel_name_ . -->
* Just for myself, please.
    - slot{"train_status": "booked"}
    - offerbooked_train_reqmore_general: I have booked you a ticket on _reference_ for _number_ pounds. The train leaves _hotel_name_ at _time_ . Your reference number is _reference_ . Can I help you further?   <!-- predicted: offerbooked_train: Booking was successful for _reference_ , the total fee is _number_ _reference_ payable at the station. Reference number is _reference_ . -->
* Thank you. That is all for today. Goodbye
    - bye_general: Have a great trip.   <!-- predicted: bye_general_welcome_general: You re welcome. I hope you have a great trip! Goodbye. -->


## story_PMUL1370
* I d like to find a train from _hotel_name_ that leaves _weekday_ .
    - slot{"train_status": "available"}
    - request_train: What is your destination?   <!-- predicted: inform_train: There are several trains departing for _hotel_name_ on _weekday_ . _number_ train departs every hour starting at _time_ -->
* I would like to travel to _hotel_name_ .
    - slot{"train_status": "available"}
    - Okay. Where are you departing from? And, do you have any particular time frame in mind?
* Yes. The departure should be from stansted airport and arrive in _hotel_name_ no later than _time_ please.
    - slot{"train_status": "unique"}
    - inform_train_offerbook_train: I have _number_ trains that arrive in _hotel_name_ from Stansted Airport before _time_ . The _reference_ leaves at _time_ and arrives at _time_ . Would you like to book it?   <!-- predicted: inform_train: There are _number_ trains within that time frame. The train that will get you to _hotel_name_ closest to _time_ is the _reference_ , which leaves at _time_ and arrives by _time_ . -->
* Yes, that would be great. Please make a booking for _number_ people and send me a copy of the reference number.
    - slot{"train_status": "booked"}
    - Booking was successful, the total fee is _number_ _reference_ payable at the station. Your reference number is _reference_ . Do you need anything else today?
* Thank you, I am also looking for some places to go while I am there. I d like to check out some colleges in the _area_ part of town.
    - slot{"attraction_status": "available"}
    - inform_attraction_select_attraction: There are _number_ colleges in that part of town. _number_ are free. Would you like to hear them?   <!-- predicted: greet_general_inform_attraction_select_attraction: I am happy to help. There are several types of places to go in the _area_ . Parks, theatre, _attraction_type_ , _attraction_name_ , _attraction_type_ . What sounds good to you? -->
* What is the phone number, and address for a free _attraction_name_ that you recommend?
    - recommend_attraction_reqmore_general: _attraction_name_ is located on magdalene street. The phone number is _number_ . Do you need anything else?   <!-- predicted: recommend_attraction: I d recommend _restaurant_name_ , the number is _number_ and address is the plough, green end, fen ditton, cb58sx -->
* No, that covers everything I needed today! Thanks again!
    - slot{"attraction_status": "available"}
    - bye_general: Great. Thank you and have a great day. Goodbye.   <!-- predicted: bye_general_greet_general_welcome_general: Thanks for using our service. Take care. Bye Bye. -->


## story_MUL1122
* I am looking for something to do, preferably on the _area_ side of _hotel_name_ ; perhaps a _attraction_name_ of sorts.
    - slot{"attraction_status": "available"}
    - inform_attraction_recommend_attraction: There are _number_ museums, I d recommend _hotel_name_ book and print gallery.   <!-- predicted: inform_attraction: _hotel_name_ _attraction_name_ of Technology is located on the _area_ side at The Old Pumping Station, Cheddars Lane. Their phone number is _number_ and they charge an entrance fee of _number_ pounds. -->
* Thank you, either _number_ will be perfect. Can you choose _number_ and get me the phone number, please? Oh! And the entrance fee, too.
    - inform_attraction_reqmore_general: _hotel_name_ Book and Print Gallery is free to enter, and their number is _number_ . Can I help you with anything else today?   <!-- predicted: inform_attraction: The scudamores punting co is at granta place, mill lane phone number is _number_ . The _hotel_name_ punter is at 251a chesterton road phone number _number_ . No entrance fee information listed. -->
* Yes, have you heard of the _hotel_name_ _hotel_type_ ?
    - slot{"hotel_status": "unique"}
    - The _hotel_name_ _hotel_type_ is located in the _area_ at _number_ barton road postcode cb39lh. The phone number is _number_ . Would you like me to book a room?
* Yes. Please book me a room for _number_ nights starting _weekday_ . We have _number_ total guests. I also need a reference number please.
    - slot{"hotel_status": "booked"}
    - book_booking_hotel_reqmore_general: Your reservation was successful. Your reference number is _reference_ . Can I help you with anything else today?   <!-- predicted: book_booking_hotel_inform_hotel_reqmore_general: You are booked at the _hotel_name_ B & B. It is _pricerange_ , with wifi and parking included. Your reference number is _reference_ . Is there anything else? -->
* I will need a taxi to take me from the _attraction_name_ to the _hotel_type_ . I am planning on leaving the _attraction_name_ at _time_ .
    - slot{"taxi_status": "booked"}
    - inform_taxi_reqmore_general: Of course! Look for a _color_ _reference_ . The contact number is _number_ . Anything else I can do for you?   <!-- predicted: inform_taxi: I have booked the taxi for you. You ll be picked up by a _color_ _cartype_ . Their phone number is _number_ -->
* No thanks. Thank you.
    - bye_general: Have a nice day!   <!-- predicted: reqmore_general: Will you need a taxi? Or anymore info on your stay? -->


## story_PMUL4462
* Hello, I am looking for a restaurant in _hotel_name_ . I believe it is called _restaurant_name_ .
    - slot{"restaurant_status": "available"}
    - It is located at _number_ Histon Road Chesterton
* Can you book me a table for _time_ on _weekday_ ?
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant: Yes I can! Table for _number_ ?   <!-- predicted: inform_booking_restaurant_inform_restaurant: That is an _pricerange_ _food_type_ restaurant. Do you want me to book a reservation? -->
* Actually, for _number_ , please.
    - slot{"restaurant_status": "booked"}
    - Okay, your booking was successful! The reference number is _reference_ . The table will be reserved for _number_ minutes.
* Great, can you also get me information or _attraction_type_ in the area
    - slot{"attraction_status": "available"}
    - inform_attraction_select_attraction: Sure. There are several churches and an _attraction_name_ attraction, all in the centre area. Do you have a preference?   <!-- predicted: inform_attraction_request_attraction: There are _number_ museums in _hotel_name_ , would you like to know of any in a specific area, or would you like a recommendation? -->
* What do you recommend?
    - _attraction_name_ is lovely, they are on trinity lane and free admission
* Can I get the postcode for that? I also need to book a taxi to the _restaurant_name_ .
    - slot{"attraction_status": "available"}
    - slot{"taxi_status": "available"}
    - inform_attraction_request_taxi: The postcode is cb21tt. Are you looking for a taxi from _attraction_name_ to the _restaurant_name_ ?   <!-- predicted: greet_general_request_train: I can help you with that. Can you please tell me what station you will be leaving from and your destination. Also a time preference. -->
* Yes I do. I d like to make sure I arrive at the restaurant by the booked time. Can you check?
    - slot{"taxi_status": "available"}
    - request_taxi: What time do you want to leave?   <!-- predicted: inform_restaurant_request_restaurant: I have several listings available for you to choose from, is there any preference on the type of food they serve for you? -->
* Actually all you have to do is set the taxi so it arrives by the arrived time. Am I better off booking it myself?
    - slot{"taxi_status": "booked"}
    - inform_taxi: I have booked you a taxi for _weekday_ to arrive at _attraction_name_ at _time_ . Is there anything else I may help you with?   <!-- predicted: greet_general_inform_taxi: No problem! I have booked you a cab that will take you to the restaurant by _time_ . Look for a _color_ _cartype_ taxi. The cab s contact number is _number_ . -->
* I need the contact number and car type also.
    - inform_taxi: it is a _cartype_ _color_ in colour and contact number is _number_   <!-- predicted: inform_taxi_reqmore_general: Alright, I got you booked. the car will be a _color_ _cartype_ and the contact number is _number_ . Anything else I can help you with? -->
* Thanks for the service, good day.
    - bye_general_welcome_general: You re welcome! Have a great day!   <!-- predicted: bye_general_greet_general_welcome_general: Thank you so much for calling! Enjoy your trip! Goodbye! -->


## story_MUL2155
* I am looking for a place to stay in the _area_ of the city. I would prefer a _number_ star _hotel_type_ please.
    - slot{"hotel_status": "available"}
    - There are several guesthouses available. Do you have a price reference?
* No price preference needed
    - slot{"hotel_status": "unique"}
    - The _hotel_name_ guesthouse _hotel_type_ is located in the _area_ , has a _number_ star rating, and is moderately priced. Would you like me to book it for you?
* Does it have free wifi?
    - inform_hotel: How about the _hotel_name_ guesthouse?   <!-- predicted: inform_booking_restaurant: Yes, I can take of that reservation for you. -->
* I think that would be fine.
    - slot{"hotel_status": "available"}
    - What day would you like to stay? How many days?
* I would like it book for _weekday_ for _number_ people and _number_ nights. Can I have the booking number please.
    - slot{"hotel_status": "booked"}
    - book_booking_hotel_reqmore_general: The _hotel_type_ is booked and your reference number is _reference_ . Can I help you with anything else?   <!-- predicted: book_booking_hotel_inform_hotel_reqmore_general: You are booked at the _hotel_name_ B & B. It is _pricerange_ , with wifi and parking included. Your reference number is _reference_ . Is there anything else? -->
* I also need a train that departs from _hotel_name_ .
    - slot{"train_status": "available"}
    - What is your desired destination?
* I would like to visit _location_ on _weekday_ .
    - slot{"train_status": "available"}
    - inform_train_request_train: There are _number_ trains to _location_ on that day. Do you know what time you d like to leave or arrive by?   <!-- predicted: inform_train: The next train leaving from _hotel_name_ for _location_ departs _weekday_ at _time_ , and will arrive by _time_ . -->
* I need to be in _location_ by _time_ .
    - slot{"train_status": "unique"}
    - inform_train_offerbook_train: Train _reference_ will get you there by _time_ . Do you want tickets for that?   <!-- predicted: inform_train: I have _number_ trains that would suit your needs. May I suggest the _number_ that arrives by _time_ ? -->
* I need the departure time for that train.
    - inform_train_select_train: No problem! The departure time for _reference_ is _time_ . Will that work?   <!-- predicted: inform_train: _reference_ will arrive in _hotel_name_ _weekday_ by _time_ , it will depart peterborough at _time_ . Does this suit your needs? -->
* What is the price for that train?
    - It is _number_ pounds per person.
* Thank you, I think that is all I need for today.
    - greet_general: Great! Hope you enjoy your trip!   <!-- predicted: bye_general: Thank you for contacting _hotel_name_ TownInfo Centre. Have a wonderful day! -->


## story_MUL1254
* I want to find a _food_type_ restaurant that is _pricerange_ .
    - slot{"restaurant_status": "NA"}
    - I m very sorry, there are no results for _pricerange_ _food_type_ restaurants. Would you like to try for a different type of cuisine?
* Do you have any restaurants in the centre?
    - slot{"restaurant_status": "available"}
    - inform_restaurant_select_restaurant: I have _number_ different _pricerange_ restaurants in the centre. _number_ are _food_type_ restaurants, and the other _number_ serve _food_type_ . Do you have a preference?   <!-- predicted: nooffer_restaurant_request_restaurant: I m sorry, but I could not find any listings for restaurants serving _food_type_ style food. Do you have any other favorite types of cuisines? -->
* How about a _food_type_ restaurant located in the centre
    - slot{"restaurant_status": "available"}
    - inform_restaurant_reqmore_general: There are _number_ in that area. _attraction_name_ Hut City Centre, Ask, and Zizzi _hotel_name_ . Is there any more information you d like about any of them?   <!-- predicted: inform_restaurant: I found _number_ options for you _restaurant_name_ at Regent Street City Centre, _restaurant_name_ at _number_ Mill Road City Centre, and _restaurant_name_ at _number_ _hotel_name_ Road City Centre -->
* No, which _number_ would you recommend?
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_recommend_restaurant: I ve heard that Ask is _number_ of the best in town. Can I reserve you a table there?   <!-- predicted: inform_booking_hotel_recommend_hotel: Sure, I recommend _hotel_name_ in the centre, would you like me to make a reservation for you? -->
* Book a table for _number_ on _weekday_ at _time_ please. I ll need to have the reference number.
    - slot{"restaurant_status": "booked"}
    - Your reference number is _reference_ .
* Excellent. I m also looking for _hotel_name_ _hotel_type_ . Do they have free parking and what type of _hotel_type_ are they?
    - slot{"hotel_status": "unique"}
    - They are a guesthouse _hotel_type_ with parking. Want to book?
* Yes, I need the room for _number_ guest only. Thank you.
    - slot{"hotel_status": "booked"}
    - book_booking_hotel_greet_general: I have booked _hotel_name_ guesthouse for _number_ person. You didn t mention how many days, but that can be taken care of there. You re all set!   <!-- predicted: book_booking_hotel_reqmore_general: Great, I have booked your stay for _number_ people for _number_ nights. Your reference number is _reference_ . May I help with anything else? -->
* Alright. Thanks for the help.
    - bye_general_greet_general_welcome_general: You are welcome. Thank you for using our service. Goodbye!   <!-- predicted: bye_general: Absolutely. Thank you for contacting the help desk. Have a great day. -->


## story_MUL2089
* I d like a moderately priced _hotel_type_ with free parking, please.
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel_inform_hotel: _hotel_name_ is a _number_ -star _hotel_type_ located in _number_ chesterton road, should i book it for you?   <!-- predicted: inform_booking_hotel_recommend_hotel: May I reccommend _hotel_name_ ? It is moderately priced and fits all your criteria. Would you like me to reserve you any rooms? -->
* Is that located in the _area_ . I really want to stay somewhere in the _area_ .
    - slot{"hotel_status": "available"}
    - inform_hotel_reqmore_general: Yes that is located in the _area_ . Should I book it for you?   <!-- predicted: inform_booking_hotel_inform_hotel: The _hotel_name_ is in the _pricerange_ price range. I have _hotel_name_ also in the _area_ in the _pricerange_ price range. Would you like to book? -->
* Does it also have internet access?
    - slot{"hotel_status": "available"}
    - inform_hotel: It does have wifi.   <!-- predicted: greet_general_inform_hotel_recommend_attraction: Yes, the Lovell is indeed a _number_ star location. Might I suggest the _hotel_name_ Arts Theatre for your _attraction_type_ during your stay? It s a highly recommended experience. -->
* Does it include free parking?
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel: Yes it does. Would you like me to book you a room?   <!-- predicted: inform_booking_hotel_inform_hotel: Yes, they both do. The _hotel_name_ B&B is our inexpensive _number_ star guesthouse. Would you like me to see if I could book you room? -->
* I have to discuss it with my husband, so no thanks. Can you tell me about trains leaving _weekday_ ? I need to arrive by _time_ .
    - slot{"train_status": "available"}
    - request_train: And where do you want to travel to and from?   <!-- predicted: inform_train: I have _number_ trains departing _hotel_name_ on _weekday_ to _location_ . The earliest is leaving at _time_ arriving by _time_ , will this suit you? -->
* I will be traveling from _hotel_name_ heading to Bishops Stortford.
    - slot{"train_status": "available"}
    - inform_train: I have _number_ trains that would suit your needs. May I suggest the _number_ that arrives by _time_ ?   <!-- predicted: inform_train_request_train: i have over a thousand trains leaving from _hotel_name_ . what day and time do you wish to travel? -->
* Yes that works for me. Can I have the travel time and the train ID?
    - inform_train_reqmore_general: Yes the travel time is _number_ minutes and the trainID is _reference_ . Can I help you with anything else?   <!-- predicted: inform_train_offerbook_train: The train ID for that is _reference_ and the travel time is _number_ minutes. Would you like me to book you a seat? -->
* That will be all, thank you!
    - greet_general: You are very welcome. Have a great day.   <!-- predicted: bye_general_greet_general_welcome_general: You re quite welcome. Just let us know if you find yourself needing more information. Have a great day! -->


## story_SNG01359
* Please help me make a taxi reservation
    - Sure! Where is your departure site?
* I want to depart from the _restaurant_name_ .
    - slot{"taxi_status": "available"}
    - request_taxi_welcome_general: I can help you with that. When do you need to leave?   <!-- predicted: request_taxi: I d be happy to help you with a taxi, what is your destination departure and what time would you like to arrive leave? -->
* It doesn t matter, just so I arrive by _time_ .
    - slot{"taxi_status": "available"}
    - request_taxi_welcome_general: I can help you with that. where are you going?   <!-- predicted: inform_train_request_train: I have _number_ trains available. What is your destination and preferred departure and arrival times? -->
* I want to go to the _restaurant_name_ . And I need the car type and contact number please.
    - slot{"taxi_status": "booked"}
    - Okay, I have a _color_ _cartype_ for you with the contact number _number_ . Is there anything else you need today?
* No that is all. Thanks.
    - bye_general_welcome_general: You re welcome, have a wonderful time!   <!-- predicted: bye_general: Enjoy your dinner. Thank you for calling _hotel_name_ TownInfo Centre. Goodbye. -->


## story_SNG0095
* Hi, I m looking for a taxi. I need to leave from _restaurant_name_ at _time_ .
    - slot{"taxi_status": "available"}
    - Sure, can I have the destination for your taxi please?
* I m headed to the _attraction_name_ .
    - slot{"taxi_status": "booked"}
    - inform_taxi_reqmore_general: I have booked a taxi for you. It is a _color_ _cartype_ and the contact number is _number_ . Is there anything else I can help you with today?   <!-- predicted: inform_taxi: Okay! Your taxi is a _color_ _color_ _cartype_ . Contact number _number_ -->
* No, you have been very helpful. Thank you.
    - bye_general: Have a nice day!   <!-- predicted: bye_general_reqmore_general_welcome_general: Okay, great. I m glad I could help. Don t hesitate to contact us again if you need additional assistance. Goodbye. -->


## story_MUL0498
* Hi, could you recommend any local cinemas in the area? I m looking for any places that are near the centre.
    - slot{"attraction_status": "available"}
    - There is _number_ _attraction_type_ in the centre called Vue _attraction_type_ . Would you like the address and postcode?
* Yes, please. I would also like to know the entrance fee and phone number for that _attraction_type_ .
    - The postcode is cb11ps. The address is the _restaurant_name_ centre, _area_ road. The phone number is _number_ . The entrance fee is not present in our database.
* I also want information on any trains that depart from broxbourne to _hotel_name_ .
    - slot{"train_status": "available"}
    - There are _number_ trains that travel that route. What day and time would you like to travel?
* I want to leave on a _weekday_ and arrive by _time_ .
    - slot{"train_status": "available"}
    - inform_train_request_train: There are _number_ departures with those criteria. When do you want to leave by?   <!-- predicted: inform_train: I have _number_ trains that would suit your needs. May I suggest the _number_ that arrives by _time_ ? -->
* It doesn t matter when I leave by.
    - slot{"train_status": "unique"}
    - Train _reference_ leaves at _time_ . Would you like to book this train?
* No thanks, I m just gathering information. Could you give me the ticket price of the _time_ ?
    - inform_train: The price is _number_ pounds.   <!-- predicted: inform_train_reqmore_general: Sure, _reference_ is a _number_ minute trip and each seat costs _number_ pounds. Can I help you with anything else today? -->
* Thank you very much for the help!
    - You are welcome. If you would like help booking a train feel free to ask.


## story_PMUL4106
* Hello, I am looking for a concerthall in the centre of town.
    - slot{"attraction_status": "available"}
    - We have a concerthall in the centre by the name of _attraction_name_ , would you like more information?
* What a neat sounding name! That might be a good fit. Can you tell me the address and postcode please?
    - slot{"attraction_status": "available"}
    - inform_attraction: _attraction_name_ is located at _number_ norfolk street and their post code is cb12lf   <!-- predicted: inform_attraction_reqmore_general: I can tell you that Byard Art is located at _number_ King s Parade, postcode cb21sj. Does that help? -->
* Great what is the entrance fee too?
    - I am unsure if there is an entrance fee. Can I help with anything else?
* Yes, I also need to find a train, please.
    - greet_general_request_train: I d be happy to help with that. Can you tell me where you will be departing from?   <!-- predicted: request_train: Sure! When are you wanting to travel, where are you leaving from, where would you like to go and what time? -->
* I need to depart from Strevenage, _weekday_ , after _time_ . Arriving in _hotel_name_ .
    - slot{"train_status": "unique"}
    - There are _number_ trains that meet your needs. May I book _number_ of them for you?
* That would be great, how long is that train ride by the way?
    - inform_train: The travel time for all trains to that destination is _number_ minutes   <!-- predicted: inform_train_offerbook_train: It s _number_ minutes. Would you like to book some tickets? -->
* Can you give me the arrival time of _number_ of them? And the price please.
    - inform_train: The _reference_ leaves at _time_ and arrives by _time_ . The travel time is _number_ minutes.   <!-- predicted: greet_general_inform_attraction: That sounds like an exciting trip! _hotel_name_ University Botanic Gardens is located in the centre of town on Bateman Street. Its admission fee is _number_ pounds. -->
* Thank you for serving me, goodbye.
    - bye_general: Goodbye, enjoy your day.   <!-- predicted: request_train_welcome_general: Okay, if you d like a booking, I ll need to know how many tickets you need. Or, if we re done here, have a very nice day. -->


## story_MUL1071
* Hello, I m looking for places to go in the centre.
    - slot{"attraction_status": "available"}
    - inform_attraction_request_attraction: There are many attractions in the centre like museums, _attraction_type_ , _attraction_name_ , and concerthalls. What are you interested in?   <!-- predicted: inform_attraction_reqmore_general: I have _number_ _attraction_type_ attractions. _number_ are in the centre, with _number_ in the _area_ and _area_ . Are you interested in information about _number_ of them in a certain area? -->
* How about a _attraction_name_ attraction?
    - slot{"attraction_status": "available"}
    - inform_attraction_select_attraction: There are _number_ in the centre of town. Scudamores Punting Co, and the _hotel_name_ Punter. Would either of those interest you?   <!-- predicted: inform_attraction: The scudamores punting co is at granta place, mill lane phone number is _number_ . The _hotel_name_ punter is at 251a chesterton road phone number _number_ . No entrance fee information listed. -->
* Could you give me the address for the _hotel_name_ Punter, please? I also need a place to stay, preferably somewhere _pricerange_ .
    - slot{"attraction_status": "available"}
    - slot{"hotel_status": "unique"}
    - inform_attraction_inform_booking_hotel_inform_hotel: Sure, the _hotel_name_ punter is lcoated at 251a chesterton road. The _hotel_name_ is in the _pricerange_ price range with _number_ stars. Would you like to book a room?   <!-- predicted: inform_booking_hotel_inform_hotel: Yes, they both do. The _hotel_name_ B&B is our inexpensive _number_ star guesthouse. Would you like me to see if I could book you room? -->
* Does it offer free wifi internet?
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel_inform_hotel: Yes the _hotel_name_ does have free wifi. Would like me to book a room for you?   <!-- predicted: inform_booking_hotel_recommend_hotel_reqmore_general: The _hotel_name_ is a guesthouse that meets your specifications. Would you like any additional information? I could also book a room for you. -->
* Yes please. I will need the _hotel_type_ for _number_ people starting _weekday_ for _number_ nights.
    - slot{"hotel_status": "booked"}
    - I have booked the _hotel_type_ . The reference number is _reference_ . Is there anything else I can help you with?
* No that is all I need today. Thank you for the help.
    - Great, thanks for using our service. Have a great day.
* you too, goodbye!
    - bye_general: Thank you, and goodbye.   <!-- predicted: reqmore_general: Sorry, just to clarify, did you actually not need a taxi after all then? -->


## story_PMUL0578
* Hello, I d like some information on a restaurant today.
    - inform_restaurant_request_restaurant: There are many options in _hotel_name_ , do you have any tastes in particular?   <!-- predicted: request_hotel: Can you please tell me what type of place and if you have any preferences? -->
* I would like some _food_type_ .
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_restaurant: There are _number_ results for _food_type_ restaurants. Is there a certain area or price range you re looking at?   <!-- predicted: inform_restaurant_select_restaurant: We ve got _number_ places serving _food_type_ food in town, _number_ are in the city centre and _number_ in the _area_ . Do you have a preference? -->
* I want something in the _area_ area with a _pricerange_ price.
    - slot{"restaurant_status": "unique"}
    - _restaurant_name_ fits your request perfectly. They are located at _number_ Northampton Street. Would you like to make a booking?
* No thank you, but may I please have the phone number, address, and post code?
    - inform_restaurant_reqmore_general: the phone number is _number_ . the address is _number_ Northampton Street, and the post code is cb30ad. is there anything i can help you with?   <!-- predicted: greet_general_inform_hotel_reqmore_general: Of course! The address of the _hotel_name_ is kingfisher way, hinchinbrook business _attraction_type_ , huntingdon and it s phone number is _number_ , would you like anything else? -->
* I also need a train to _location_ on _weekday_ .
    - slot{"train_status": "available"}
    - request_train: I d be glad to help you with that. From where will you be departing?   <!-- predicted: inform_train: The next train leaving from _hotel_name_ for _location_ departs _weekday_ at _time_ , and will arrive by _time_ . -->
* I m departing from _hotel_name_ and I d like to arrive by _time_ , if possible.
    - slot{"train_status": "available"}
    - request_train: Do you have a departure time you d like?   <!-- predicted: inform_train: I m sorry, that is the closest arrival to _time_ . Would you like me to look at something arriving after that time? -->
* I don t have a departure time but I do need to arrive by _time_ .
    - slot{"train_status": "unique"}
    - inform_train_offerbook_train: there is a train that will arrive at _time_ . Would you like me to book it?   <!-- predicted: inform_train: Great! I have the _reference_ departing at _time_ and arriving by _time_ or if you would like a later time the _reference_ departs at _time_ and arrives by _time_ . -->
* Yes please! I ll also need the train ID, price, and travel time. Thanks!
    - slot{"train_status": "available"}
    - inform_train_request_train: The _reference_ will leave _hotel_name_ at _time_ and arrive in _location_ at _time_ . It will be _number_ pounds and take _number_ minutes. How many tickets do you need?   <!-- predicted: greet_general_inform_train: Certainly. The train s ID is _reference_ , and the price for a ticket is _number_ pounds. -->
* I don t need any tickets at this time. Thank you. That is all.
    - bye_general: Thank you for using this system goodbye   <!-- predicted: welcome_general: you re welcome, thank you for using our system. -->


## story_MUL0197
* I m looking for an _pricerange_ restaurant in the center of town.
    - slot{"restaurant_status": "available"}
    - There are _number_ restaurants that meet your needs. Would you like to narrow your search by type of food?
* I don t care about food. Surprise me.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_recommend_restaurant_reqmore_general: _restaurant_name_ serves _food_type_ , it s located at _number_ Trumpington Street City Centre. Would you like to hear about any others? There are _number_ results if _food_type_ isn t your style.   <!-- predicted: request_train: There area a number of departures on _weekday_ starting at _time_ in the morning. Was there a particular time of day you wanted to depart? -->
* That sounds fine. Can you book it please and get me the reference number?
    - slot{"restaurant_status": "available"}
    - request_booking_restaurant: Sure, what day and time would you like and how many people?   <!-- predicted: nobook_booking_attraction_reqmore_general: I can not. It doesn t give me the option to book tickets. Just general Information. Can I help you with anything else? -->
* I would like a table for _number_ at _time_ on _weekday_ , and I will need the reference number. Thanks.
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_reqmore_general: Okay, the booking was successful. The reference number is _reference_ . Is there anything else I can help you with?   <!-- predicted: book_booking_restaurant: You are booked! Your table will be reserved for fifteen minutes and your reference number is _reference_ . -->
* I m also looking for a place to stay. It needs to include free wifi and parking, be _number_ star, and in the same area as the restaurant.
    - slot{"hotel_status": "available"}
    - recommend_hotel: The _hotel_name_ is a _number_ star _hotel_type_ in the centre area. It is in the _pricerange_ price range, and has free parking and wifi.   <!-- predicted: inform_hotel_select_hotel: I have _number_ options with those specifications. The _hotel_name_ and the _hotel_name_ both with free wifi and parking. Which would you prefer? -->
* Can I get the address of the _hotel_name_ , please?
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel_inform_hotel: Absolutely, the address for the _hotel_name_ is _hotel_name_ Place. Would you like me to book a reservation for you?   <!-- predicted: inform_booking_restaurant_inform_restaurant: Yes, the address is _number_ Hills Road City Centre and postcode is cb21nw. Would you like me to make a reservation? -->
* No, but I will need a taxi between the _hotel_type_ and the booked restaurant.
    - slot{"taxi_status": "booked"}
    - greet_general_inform_taxi: No problem! I have booked you a cab that will take you to the restaurant by _time_ . Look for a _color_ _cartype_ taxi. The cab s contact number is _number_ .   <!-- predicted: inform_taxi: Booking completed! your taxi will be _color_ _cartype_ Contact number is _number_ -->
* Great, thanks for all of your help.
    - reqmore_general_welcome_general: You are welcome. Is there anything else I can do for you today?   <!-- predicted: bye_general_reqmore_general_welcome_general: Okay, great. I m glad I could help. Don t hesitate to contact us again if you need additional assistance. Goodbye. -->
* No. Thank you for your help!
    - You re welcome. Enjoy your day!


## story_MUL2146
* I am looking for a _hotel_type_ , _hotel_name_ .
    - slot{"hotel_status": "unique"}
    - greet_general_inform_booking_hotel_inform_hotel: Sure, I have it right here. Its a _pricerange_ priced guesthouse with a _number_ star rating, free internet and parking. Phone number is _number_ can I book it for you?   <!-- predicted: inform_booking_hotel_inform_hotel: The _hotel_name_ guesthouse _hotel_type_ is located in the _area_ , has a _number_ star rating, and is moderately priced. Would you like me to book it for you? -->
* No, that is all for now.
    - greet_general_reqmore_general: Ok. I can also help with restaurant, train or taxi reservations. Do you need any of these?   <!-- predicted: inform_booking_hotel_inform_hotel: Yes, all of the hotels and guesthouses are able to accommodate _number_ guests per booking. Are you ready to book? If so, I just need a little more info. -->
* I am needing a train to arrive in _hotel_name_ by _time_ .
    - slot{"train_status": "available"}
    - request_train: What day did you need a train for? Also, where will you be departing from?   <!-- predicted: inform_train_request_train: There are very many trains that fit your requirements, where are you leaving from and what day would you like to leave? -->
* I want to travel on _weekday_ . I m coming from Broxbourne to _hotel_name_ .
    - slot{"train_status": "unique"}
    - _reference_ matches your criteria. It leaves at _time_ on _weekday_ . Would you like to book this train?
* As long as it arrives by _time_ , then it s good. Can you book it for _number_ people?
    - slot{"train_status": "booked"}
    - inform_train_reqmore_general: It arrives at _time_ . Your reference number is _reference_ and the total fee for _number_ people is _number_ _reference_ . Is there anything else I can help you with?   <!-- predicted: offerbooked_train_reqmore_general: Sure, the train is actually number _reference_ and your reference number is _reference_ . The price will be _number_ _reference_ payable at the station. Is there anything else today? -->
* No, that s everything. Thank you.
    - welcome_general: You are very welcome!   <!-- predicted: bye_general_welcome_general: Wonderful! You re welcome, have a great day! -->


## story_MUL1695
* Hi there, I m looking for a restaurant that serves _food_type_ food. It can be anywhere, I m willing to pay a _pricerange_ amount of money. Do you have any recommendations?
    - slot{"restaurant_status": "NA"}
    - nooffer_restaurant_select_restaurant: Unfortunately, I wasn t able to find anything that matches your request. Shall we look for a _pricerange_ or _pricerange_ _food_type_ restaurant instead?   <!-- predicted: nooffer_restaurant_request_restaurant: I m sorry, but I could not find any listings for restaurants serving _food_type_ style food. Do you have any other favorite types of cuisines? -->
* Sure, look for a _pricerange_ restaurant. And I prefer the _area_ if possible.
    - slot{"restaurant_status": "NA"}
    - Unfortunately there are none fitting that criteria either, would you like me to search for a different type of restaurant?
* A _food_type_ restaurant, please.
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_inform_restaurant: _restaurant_name_ is a _food_type_ restaurant located in the _area_ at a _pricerange_ price. Would you like to book a table?   <!-- predicted: inform_booking_restaurant_recommend_restaurant: I would recommend _restaurant_name_ . It is an _pricerange_ restaurant in the center. Would you like to book a reservation? -->
* Yes please for _number_ people at _time_ on _weekday_ .
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_reqmore_general: I was ale to succesfully book you, The table will be reserved for _number_ minutes. The Reference number is _reference_ . Can i assist with anything else?   <!-- predicted: book_booking_restaurant: You are booked! Your table will be reserved for fifteen minutes and your reference number is _reference_ . -->
* Yes, I also need a train. I need to get to _hotel_name_ by _time_ .
    - slot{"train_status": "available"}
    - What day and what is the departure location?
* I ll be coming from _location_ , _location_ Street on the same day as my restaurant reservation, please.
    - slot{"train_status": "available"}
    - I have several trains that will get you to Cabridge on time. Is there a particular departure time you would like?
* I would like the latest train leaving that will arrive by _time_ please. Could you give me a departure time and travel time?
    - slot{"train_status": "unique"}
    - The _reference_ will be arriving just before _time_ on _weekday_ . It departs at _time_ and is an _number_ minute ride. Would you like me to book it?
* Can you tell me what time that train leaves?
    - inform_train_reqmore_general: The train departs at _time_ . Can I help you with anything else?   <!-- predicted: inform_train_offerbook_train: The train ID for that is _reference_ and the travel time is _number_ minutes. Would you like me to book you a seat? -->
* No, that s all I need, thank you!
    - bye_general: Thank you for using our system!   <!-- predicted: bye_general_welcome_general: So happy to be of service, and thanks for using _hotel_name_ TownInfo centre today. Have a wonderful day! -->


## story_SNG01924
* I need a taxi, please.
    - I d be happy to assist you today. I ll need a little bit of information from you - let s start with what time you d like to leave arrive?
* I need to get to restaurant _number_ _number_ by _time_
    - slot{"taxi_status": "available"}
    - Ok, I need a little bit more information, where will your taxi be departing from?
* I want to be picked up at _attraction_name_ .
    - slot{"taxi_status": "booked"}
    - Your taxi is booked a _color_ _cartype_ with the contact number of _number_ .
* I look forward to the ride. Thank you.
    - reqmore_general: You re welcome. Is there anything else I can do for you today?   <!-- predicted: reqmore_general_welcome_general: You re very welcome. Is there anything else at all that I could assist you with? -->
* No, that will be all. Thanks very much.
    - You re welcome. Thank you for using the TownInfo centre. Goodbye.


## story_PMUL3044
* i need a place to stay
    - request_hotel: Is there a certain area or price range you had in mind?   <!-- predicted: inform_hotel_request_hotel: Most of the hotels in town offer free parking. Is there a certain area you d like to stay in, or do you have a price range in mind? -->
* I really want to stay with something moderately priced. But, I want it to be _number_ star rated if possible.
    - slot{"hotel_status": "available"}
    - inform_hotel_request_hotel: There are lots of moderately priced _number_ star hotels. Are you interested in a particular part of town?   <!-- predicted: inform_hotel_select_hotel: I have _number_ options with those specifications. The _hotel_name_ and the _hotel_name_ both with free wifi and parking. Which would you prefer? -->
* Maybe a guesthouse with free parking, I have _number_ guests and that will be for _number_ nights this _weekday_
    - slot{"hotel_status": "unique"}
    - We have several such choices in the _area_ , _area_ and _area_ . If you have no preference for location shall I just book _number_ for you?
* That would be great.
    - inform_hotel: _hotel_name_ is a _pricerange_ price, _number_ star guesthouse in the _area_ area with wifi and parking. Will that work?   <!-- predicted: recommend_hotel: If price is not an issue, I recommend the _pricerange_ _hotel_name_ . If you want something cheaper, I recommend _hotel_name_ . -->
* Yeah, that sounds great. Do they have room for all _number_ of us?
    - request_booking_hotel: I can try to see if we do. Can you provide when you want to stay and for how long?   <!-- predicted: inform_booking_restaurant: I can help book a _hotel_type_ if you need it! -->
* book it for _number_ people and _number_ nights starting from _weekday_ .
    - slot{"hotel_status": "booked"}
    - book_booking_hotel_reqmore_general: Done! Your reference number is _reference_ . Can I help you with anything else?   <!-- predicted: book_booking_hotel: Since you mentioned a _hotel_type_ rather than a guesthouse, I ve booked you at the _hotel_name_ , but just let me know if you prefer the other. Your reference is _reference_ . -->
* I am also looking to visit _attraction_name_ , do you know the address and cost to visit?
    - slot{"attraction_status": "available"}
    - inform_attraction: The entrance fee is _number_ pounds and the address is saint john s street.   <!-- predicted: inform_attraction_inform_train_reqmore_general: The _attraction_name_ s address is Market Street, postcode cb23nz. There are many trains arriving in Stansted Airport by _time_ . Would you like to narrow your search further? -->
* Haha, I m not familiar with _hotel_name_ . What part of town is that in?
    - inform_attraction: It is located in the centre.   <!-- predicted: inform_attraction_reqmore_general: They do not charge an entrance fee. Can I help with anything else? -->
* Ok, I think that should be about it for me. Thank you for your help.
    - bye_general_welcome_general: Thanks for letting us assist you today! Have a great trip!   <!-- predicted: greet_general_reqmore_general: Ok. I can also help with restaurant, train or taxi reservations. Do you need any of these? -->


## story_MUL2225
* Hi! I m looking for a place to stay with _number_ stars that includes wifi.
    - slot{"hotel_status": "available"}
    - greet_general_inform_hotel_request_hotel: I can help you with that. I have several options that fit this criteria. Do you prefer a particular area of town?   <!-- predicted: inform_hotel_request_hotel: Most of the hotels in town offer free parking. Is there a certain area you d like to stay in, or do you have a price range in mind? -->
* Just near _hotel_name_ , and should be a guesthouse.
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel_inform_hotel: _hotel_name_ is a guesthouse in the _area_ in the _pricerange_ price range with free wifi and parking. Would you like to reserve a room?   <!-- predicted: recommend_hotel_request_booking_hotel: OK, how about _hotel_name_ ? To book a stay I ll need to know the first day you want to stay, how many days, and how many guests. -->
* Certainly. There will be _number_ of us for _number_ nights starting on _weekday_ .
    - slot{"hotel_status": "booked"}
    - I was able to book for _number_ people for _number_ nights starting on _weekday_ . The reference number is _reference_ . Is there anything else I can help you with?
* Yes, I need a train for the same day. I need to leave after _time_ .
    - slot{"train_status": "available"}
    - request_train: Where are you leaving and arriving from?   <!-- predicted: inform_train: _reference_ leaves for _location_ from _hotel_name_ leaves at _number_ -->
* I m coming to _hotel_name_ from _location_ .
    - slot{"train_status": "unique"}
    - Train _reference_ leaves at _time_ and arrives at _time_ , it is a _number_ minute ride. Do you want me to book you?
* No thanks, I m just looking for information. That s everything I need for now.
    - bye_general: I understand. Have a very nice day.   <!-- predicted: reqmore_general: Will you need a taxi? Or anymore info on your stay? -->


## story_MUL0890
* I m looking for a restaurant that serves _food_type_ food on the _area_ side of town, is there anything like that?
    - slot{"restaurant_status": "NA"}
    - inform_booking_restaurant_inform_restaurant_nooffer_restaurant: There are no _food_type_ restaurants on the _area_ side but there is _number_ on the _area_ side. Would that suffice?   <!-- predicted: nooffer_restaurant_request_restaurant: Unfortunately, there are no _food_type_ restaurants on the _area_ side. Would you like to try a different type of restaurant or area? -->
* What about on the _area_ side? I would like for it to be _pricerange_ .
    - slot{"restaurant_status": "NA"}
    - nooffer_restaurant: I m sorry but there are not any _food_type_ restaurants on the _area_ side of town, either.   <!-- predicted: nooffer_restaurant_request_restaurant: Unfortunately, there are no _food_type_ restaurants on the _area_ side. Would you like to try a different type of restaurant or area? -->
* Bummer, how about _food_type_ food on the _area_ side? I m willing to pay for an _pricerange_ meal, if it s good!
    - slot{"restaurant_status": "available"}
    - inform_restaurant_select_restaurant: There are _number_ _food_type_ restaurant on the _area_ side ranging from moderately priced to _pricerange_ . Do you have a price preference?   <!-- predicted: inform_booking_restaurant_inform_restaurant: I have _attraction_name_ hut cherry hinton located at G4 _hotel_name_ Leisure _attraction_type_ Clifton Way Cherry Hinton. Would you like reservations? -->
* _pricerange_ would be fine. Can I have the address for the most _pricerange_ _food_type_ restaurant out of the _number_ ?
    - inform_restaurant_recommend_restaurant: How about the _restaurant_name_ ? It is in the _pricerange_ price range and serves _food_type_ food. Their address is Newmarket Road Fen Ditton.   <!-- predicted: inform_restaurant: I found _number_ options for you _restaurant_name_ at Regent Street City Centre, _restaurant_name_ at _number_ Mill Road City Centre, and _restaurant_name_ at _number_ _hotel_name_ Road City Centre -->
* I would also like to check on museums on the _area_ side. Can you see what you have in that area?
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: I have found _number_ museums. _number_ of them are free and _number_ costs _number_ pounds. Can I get you more information on any of them?   <!-- predicted: inform_attraction: There are several museums in the _area_ . Some of the more popular ones are the _attraction_name_ of classical archaeology, the lynne strover gallery, and the _attraction_name_ -->
* I need information on all of them please.
    - reqmore_general: What information would you like? The phone number, address, or postcode?   <!-- predicted: inform_booking_restaurant_inform_restaurant: I have _attraction_name_ hut cherry hinton located at G4 _hotel_name_ Leisure _attraction_type_ Clifton Way Cherry Hinton. Would you like reservations? -->
* the address please
    - reqmore_general: I can give you the address for only _number_ , is there _number_ in particular you wish to learn more about?   <!-- predicted: inform_attraction: It s in the centre and the address is saint andrew s street. -->
* Give me information on the _number_ closest to _restaurant_name_ .
    - inform_attraction_recommend_attraction: They are all in the same general area, but _hotel_name_ Artworks is nice. It is located at _number_ Greens Road, cb13ef. You can call them at _number_ .   <!-- predicted: inform_restaurant_reqmore_general: Yes, _restaurant_name_ is a _food_type_ restaurant on the pricey side. Would you like their phone number or address? -->
* Cool! Is that _number_ of the free ones? Gotta save my money for the grub, you know.
    - slot{"attraction_status": "available"}
    - inform_attraction: _hotel_name_ artworks is free.   <!-- predicted: bye_general_welcome_general: Enjoy your time in _hotel_name_ ! I m glad I could help you with your plans today. -->
* Perfect! Thank you so much for your help!
    - reqmore_general: Anything else I can do for you?   <!-- predicted: bye_general: You are welcome and thank you for using _hotel_name_ TownInfo Centre. -->


## story_MUL2365
* Can you find an attraction in the centre?
    - slot{"attraction_status": "available"}
    - There are a lot, ranging from _attraction_name_ to The _hotel_name_ Corn Exchange. Did you have something specific in mind?
* Not really. I just want to see some local tourist attractions in the centre.
    - slot{"attraction_status": "available"}
    - inform_attraction: _attraction_name_ is in the center and it s known for it s _attraction_type_ . The entrance fee is free.   <!-- predicted: recommend_attraction_reqmore_general: If you like parks the Wandlbury Country _attraction_type_ has free admission and is in the cb223ae postcode. Or I can tell you about the other attractions? -->
* I am also looking for a place to dine. The restaurant should serve _food_type_ food and should be in the _pricerange_ price range
    - slot{"restaurant_status": "available"}
    - recommend_restaurant: How about the _restaurant_name_ ? It is located in the city centre.   <!-- predicted: inform_restaurant_request_restaurant: There are _number_ _pricerange_ restaurants in town. Do you have a food preference or an area of town you want to eat in? -->
* Yes, that will work perfect. I will go ahead and contact them myself though. Thanks so much. Take care. Goodbye!
    - slot{"restaurant_status": "available"}
    - bye_general_welcome_general: My pleasure! Have a wonderful day and thanks for contacting the _hotel_name_ TownInfo centre.   <!-- predicted: inform_restaurant_request_booking_restaurant: Their postcode is cb11lh and if you want a reservation just let me know the time, party size, and day and I ll make it for you. -->
* I also need to book the restaurant.
    - request_booking_restaurant: I ll be happy to help with that. Can you tell me the day, time and how many people in your party?   <!-- predicted: request_taxi: What time do you need the taxi? -->
* I would like to dine on _weekday_ and need a table for _number_ people at _time_ .
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_reqmore_general: The booking was successful. The table will be reserved for _number_ minutes. Reference number is _reference_ . what else can I help you with?   <!-- predicted: book_booking_restaurant: You are booked! Your table will be reserved for fifteen minutes and your reference number is _reference_ . -->
* No, as long as the _restaurant_name_ is in the centre area, that is perfect. Thank you.
    - bye_general: Perfect, have a great meal.   <!-- predicted: inform_attraction: There is _attraction_name_ it s in the centre. It is on Saint Andrew s street and it s free. -->


## story_PMUL1801
* I need a train to Peterborough that will be there no later than _time_ .
    - slot{"train_status": "available"}
    - request_train: I have several choices, do you have a time for your departure?   <!-- predicted: inform_train_request_train: What day would you be traveling? There are _number_ trains on that route. There is a train that departs _weekday_ at _time_ and will arrive in Ely at _time_ . -->
* I am looking for a train arriving in Peterborough.
    - request_train: And where will you be leaving from?   <!-- predicted: inform_train_request_train: What day would you be traveling? There are _number_ trains on that route. There is a train that departs _weekday_ at _time_ and will arrive in Ely at _time_ . -->
* I ll be leaving _hotel_name_ on _weekday_ .
    - slot{"train_status": "available"}
    - I have train _reference_ that leaves at _time_ and will have you in Peterborough at _time_ . Would this work for you?
* Yes, that will be fine can you get me a ticket?
    - slot{"train_status": "unique"}
    - offerbook_train_request_train: How many tickets will you need?   <!-- predicted: request_train: Certainly! Can you tell me how many tickets you will be needing? -->
* I need _number_ tickets.
    - slot{"train_status": "booked"}
    - I ve booked you _number_ tickets on the _reference_ . Your reference is _reference_ and the total fee of _number_ _reference_ is payable at the station. Can I help you with anything else?
* I am also looking for a place to stay.
    - request_hotel: sure, in what area of town?   <!-- predicted: inform_hotel_request_hotel: I can we have _number_ places to stay, do you have any pricerange or area you d like to stay? -->
* I d like something moderately-priced, _number_ -stars, and in the _area_ . And I do need wifi.
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel_recommend_hotel_reqmore_general: The _hotel_name_ is a guesthouse that meets your specifications. Would you like any additional information? I could also book a room for you.   <!-- predicted: inform_booking_hotel_inform_hotel: I have several options for you, most are located in the _area_ area of town, is that acceptable? I can book _number_ for you if you would like. -->
* No, but could you book a room on _weekday_ for me please?
    - slot{"hotel_status": "available"}
    - request_booking_hotel: I d be happy to! How many are in your party and how many nights will you be staying?   <!-- predicted: reqmore_general: What part of your trip may I be of assistance with? -->
* _number_ nights starting from _weekday_ , need the reference number too please
    - slot{"hotel_status": "booked"}
    - I have made your reservations and your reference number is _reference_ .
* that is it for today
    - slot{"attraction_status": "available"}
    - bye_general_welcome_general: Gald I could help. Enjoy your stay.   <!-- predicted: bye_general: Thanks for letting us assist you today! Enjoy your stay! -->


## story_MUL1285
* Are there any _food_type_ restaurants in the city centre?
    - slot{"restaurant_status": "available"}
    - inform_restaurant_select_restaurant: There are quite a few _food_type_ restaurants in the centre. Would you like something _pricerange_ , moderately priced, or more _pricerange_ ?   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* I would like something in the _pricerange_ range and i need the address and phone number
    - slot{"restaurant_status": "available"}
    - inform_restaurant_reqmore_general: Sure, how about _attraction_name_ Hut City Centre? It s at Regent Street City Centre cb21ab and can be reached at _number_ . May I help with anything else?   <!-- predicted: inform_restaurant: I found _number_ options for you _restaurant_name_ at Regent Street City Centre, _restaurant_name_ at _number_ Mill Road City Centre, and _restaurant_name_ at _number_ _hotel_name_ Road City Centre -->
* Yes, please. I would like information about the _hotel_name_ .
    - slot{"hotel_status": "unique"}
    - The _hotel_name_ is in the _area_ part of town. It is a moderately priced _number_ star _hotel_type_ with internet service and parking. Would you like to make a reservation?
* Yes, _number_ people, _number_ nights starting from _weekday_ . Reference number please.
    - slot{"hotel_status": "booked"}
    - Booking was successful. Reference number is _reference_ .
* Thanks. I d like to get a taxi as well leaving the restaurant by _time_ . Can I get the contact number and the car type for that please?
    - slot{"taxi_status": "available"}
    - request_taxi: I need a little more information to schedule your taxi. What is your destination?   <!-- predicted: inform_taxi_reqmore_general: A _color_ _cartype_ is picking you up. Here is the contact number _number_ in case you need to call them. Is that everything? -->
* I ll be going from the restaurant we talked about (_attraction_name_ Hut City Centre) to the _hotel_type_ you booked for me (the _restaurant_name_ ).
    - slot{"taxi_status": "booked"}
    - I have booked your taxi. Be looking for a _color_ _cartype_ . If you need to contact them, please call them at _number_ . Anything more I can help with?
* No that is all I needed thank you.
    - bye_general_welcome_general: You re welcome, have a nice day.   <!-- predicted: bye_general: Have a pleasant visit. Thank you for contacting _hotel_name_ TownInfo centre. Good bye. -->


## story_MUL2281
* I need a place to stay in the _area_
    - slot{"hotel_status": "available"}
    - inform_hotel: Ok im seeing alot of choices in hotels is there anything else you need in the _hotel_type_ that would help narrow it down   <!-- predicted: greet_general_inform_hotel_request_hotel: Of course! We have multiple places to choose from. There is _number_ _hotel_type_ and the rest are guest houses. What kind of price range are you looking at? -->
* I d really like to stay in a guesthouse. I heard the ones in _hotel_name_ are very nice.
    - slot{"hotel_status": "available"}
    - inform_hotel: How about the _hotel_name_ Guesthouse? It is rated _number_ stars and is in the _pricerange_ price range.   <!-- predicted: inform_hotel_select_hotel: There is a guesthouse and _hotel_type_ available which do you prefer? -->
* Is it in the _area_ ? And do they have free parking?
    - slot{"hotel_status": "available"}
    - It is indeed in the _area_ and offers both free parking and free wifi.
* Do they have a room available for _number_ people starting _weekday_ ? We will need it for _number_ nights.
    - slot{"hotel_status": "booked"}
    - Alright, I got you booked. Your reference number is _reference_ . Anything else I can do for you?
* Yes. I need to travel from _hotel_name_ to _location_ on _weekday_ . Can you help me find a train?
    - slot{"train_status": "NA"}
    - nooffer_train: There are no trains available on _weekday_ leaving _hotel_name_ and arriving in _location_ . Can you travel on a different day?   <!-- predicted: inform_train_request_train: Perfect. Did you have a departure time in mind? You could leave _location_ as early as _time_ or as late as _time_ and still make it on time. -->
* Not really. Can you check again? I need to get to _location_ by _time_ .
    - slot{"train_status": "NA"}
    - nooffer_train_reqmore_general: I just checked again. Unfortunately there are no trains available. Any other arrangements I can make for you?   <!-- predicted: inform_attraction_request_attraction_select_attraction: There are many museums in _hotel_name_ . Is there a specific area that you would prefer? Also, do you prefer free or a cost for the _attraction_name_ ? -->
* What would be the next available if not on _weekday_ ?
    - inform_train: I did find a train for _weekday_ . _reference_ departs at _time_ and arrives by _time_ . Would that work for you?   <!-- predicted: nooffer_hotel_request_hotel: There are no results. Is there another area we can search or a different price range? -->
* _reference_ departs _hotel_name_ going to _location_ ?
    - slot{"train_status": "unique"}
    - offerbook_train: Yes, it does, would you like me to book you?   <!-- predicted: inform_train_offerbook_train: Ah, it appears that the earliest train, _reference_ , leaves at _time_ , but it does arrive by _time_ . If that is okay, I could book that for you. -->
* Yes, please. I need _number_ tickets.
    - slot{"train_status": "booked"}
    - offerbooked_train: Booking was successful, the total fee is _number_ _reference_ payable at the station .Reference number is _reference_ .   <!-- predicted: offerbooked_train_reqmore_general: Booking was successful for _reference_ , the total fee is _number_ _reference_ payable at the station. Your reference number is _reference_ . Do you need further assistance? -->
* Thank you, goodbye!
    - bye_general: Enjoy your stay, good bye!   <!-- predicted: reqmore_general: Will you need a taxi? Or anymore info on your stay? -->


## story_SNG0008
* Hi, I d like to book a taxi from _hotel_name_ to Saint Catherine s _attraction_name_ .
    - slot{"taxi_status": "available"}
    - In order to book you a taxi I will need to know either when you would like to leave or arrive by?
* I d like to arrive by _time_ , please.
    - slot{"taxi_status": "booked"}
    - inform_taxi_reqmore_general: Alright, I got you booked. the car will be a _color_ _cartype_ and the contact number is _number_ . Anything else I can help you with?   <!-- predicted: inform_taxi: Okay! Your taxi is a _color_ _color_ _cartype_ . Contact number _number_ -->
* That will be all, thanks!
    - bye_general: Have a nice day!   <!-- predicted: bye_general_welcome_general: You re welcome. Enjoy your time in _hotel_name_ and please let us know if you need anything else. Thanks! -->


## story_PMUL0204
* Could you tell me if there are any _food_type_ restaurants in the _area_ side?
    - slot{"restaurant_status": "NA"}
    - nooffer_restaurant: There aren t any _food_type_ restaurants located in the _area_ side.   <!-- predicted: inform_booking_restaurant_inform_restaurant_nooffer_restaurant: There are no _food_type_ restaurants on the _area_ side but there is _number_ on the _area_ side. Would that suffice? -->
* That s fine, how about _food_type_ in the same area?
    - slot{"restaurant_status": "available"}
    - inform_restaurant_select_restaurant: Yes, there are _number_ _food_type_ restaurants in the _area_ . Would you prefer _pricerange_ or _pricerange_ ?   <!-- predicted: inform_booking_restaurant_inform_restaurant: The _restaurant_name_ restaurant is on _area_ Road in City Centre. They are moderately priced and they serve _food_type_ . Would you like to reserve a table there? -->
* I am not bothered about the price. Why don t you select _number_ and provide me with their telephone number and price range?
    - slot{"restaurant_status": "available"}
    - the good luck _food_type_ food takeaway	is _pricerange_ and the postcode is cb17ag
* What is its phone number
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_inform_restaurant: Their phone number is _number_ . Would like to book a table?   <!-- predicted: inform_hotel: Of course. The phone number for _hotel_name_ is _number_ . -->
* Yes can you please?
    - request_booking_restaurant: Yes, I can. How many people will be with you, on what day and at what time would you like your reservation?   <!-- predicted: offerbook_train_request_train: Sure, I can book you on _reference_ arriving by _time_ . Will this be a reservation for _number_ also? -->
* Actually, that is all the information I need. I do need a place to stay in the same area.
    - slot{"hotel_status": "available"}
    - inform_hotel_request_hotel: There are _number_ guesthouses and _number_ _hotel_type_ in the _area_ . Do you have a certain price range you are looking for?   <!-- predicted: inform_booking_hotel_inform_hotel: The _hotel_name_ is in the _pricerange_ price range. I have _hotel_name_ also in the _area_ in the _pricerange_ price range. Would you like to book? -->
* I would like a _number_ star _pricerange_ place please.
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel_inform_hotel: I found _hotel_name_ located at _number_ _hotel_name_ road. Would you like me to book that for you now?   <!-- predicted: inform_booking_hotel_inform_hotel_request_booking_hotel: Sure! We will book you in a _hotel_type_ with _number_ stars. The reservation will be for _number_ people for _number_ nights. How many rooms would you like to reserve? -->
* Is that located in the _area_ ?
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel_inform_hotel: Yes. _hotel_name_ is located in the _area_ part of town. Would you like more information or to book it?   <!-- predicted: inform_booking_restaurant_recommend_restaurant: _restaurant_name_ is a very popular restaurant in the _pricerange_ range. Would you like me to book a reservation for you? -->
* Does it have free parking?
    - slot{"hotel_status": "available"}
    - inform_hotel_reqmore_general: Yes, there is free parking. What else would you like to know?   <!-- predicted: inform_hotel: Yes, they both offer free parking. -->
* find me the phone number
    - inform_hotel_reqmore_general: _hotel_name_ phone number is _number_ . Let me know if there is something else you need.   <!-- predicted: inform_hotel: Of course. The phone number for _hotel_name_ is _number_ . -->
* Great, that s all I need, thanks so much for your help! Have a great day!
    - bye_general_welcome_general: You re welcome! And thanks, you, too!   <!-- predicted: bye_general: i am glad i have been of help to you. great day -->


## story_MUL1935
* Yes, I need information about a train. Do you have information on trains departing from bishops stortford?
    - slot{"train_status": "available"}
    - inform_train_request_train: Sure, there are _number_ trains departing from Bishops Stortford. What is your destination?   <!-- predicted: inform_hotel_request_train: _hotel_name_ number is _number_ . I can absolutely help you with train, can you specify which day you d like to leave? -->
* I ll be heading for _hotel_name_ .
    - slot{"train_status": "available"}
    - What day and time would you like to travel.
* I am leaving on _weekday_ after _time_ .
    - slot{"train_status": "available"}
    - request_train: Is there a time you need to arrive by?   <!-- predicted: request_taxi: What time will you be arriving to your destination please. -->
* When are the arrival times? I m also looking for information on _attraction_name_ . What can you tell be about it?
    - slot{"attraction_status": "available"}
    - inform_train: _reference_ will arrive by _time_ if that works for you?   <!-- predicted: inform_attraction: Sure, I found it! It s located at _number_ Wheeler Street. It s a _attraction_type_ in the city s centre and it has a _number_ pounds entrance fee. -->
* I can make that work.
    - slot{"train_status": "unique"}
    - Okay, before we look for the _attraction_type_ , just to clarify your travel, the _reference_ departs Bishops Stortford _time_ , arrives _hotel_name_ _time_ . Would you like to book a ticket on this train?
* Yes for _weekday_ .I also want to know the nearby attraction called _attraction_name_ , address and area please
    - inform_attraction: Well its _attraction_type_ located in the centre of _hotel_name_ on jesus lane.   <!-- predicted: inform_attraction_reqmore_general: It is located on Trinity Lane and the phone number is _number_ . The exact address isn t listed. Is there anything else I can help with today? -->
* Great, thanks. Oh, and I don t actually need a booking for that train, so I think that s all I needed. Sorry I keep confusing the matter.
    - slot{"attraction_status": "available"}
    - bye_general_welcome_general: Don t worry about it. Thank you for contacting _hotel_name_ TownInfo Centre, and please don t hesitate to reach out again if you need more help!   <!-- predicted: inform_restaurant: There s _food_type_ , _food_type_ , _food_type_ , _food_type_ , and _food_type_ , there s a few others if none of those sound appealing. -->


## story_PMUL3734
* Where is the _hotel_name_ ?
    - slot{"hotel_status": "unique"}
    - It is in the centre of town on regent street. Would you like to book a room?
* Please. I need a room on _weekday_ for _number_ nights, and _number_ people.
    - slot{"hotel_status": "booked"}
    - Okay, your booking was successful! Your reference number is _reference_ .
* Great, thanks. I also want to find out some info on the train schedule from Ely to _hotel_name_ .
    - slot{"train_status": "available"}
    - inform_train_request_train: There are _number_ trains scheduled. Did you have a date or time in mind?   <!-- predicted: greet_general_request_taxi: We can definitely help with that. Do you need the taxi to the _attraction_name_ or to the restaurant, and what time do you need it? -->
* same day as the _hotel_type_ booking
    - slot{"train_status": "available"}
    - inform_train: The first train leaves at _time_ and they leave every _number_ hours after that until _time_ .   <!-- predicted: offerbooked_train: Your reference number is _reference_ and you ll owe _number_ _reference_ when you arrive at the station. I ll search for a _attraction_name_ for you to visit. -->
* okay, I need to arrive by _time_ , so the closest _number_ to that time please.
    - slot{"train_status": "available"}
    - inform_train: There is _reference_ . It leaves at _time_ and arrives at _time_ . Is that good for you?   <!-- predicted: inform_train_offerbook_train: I have _number_ trains that will get you to _hotel_name_ by _time_ . _reference_ will get you there at _time_ . Would that work? -->
* Sounds good. May I have the travel time and ticket price, please?
    - slot{"train_status": "available"}
    - inform_train: Sure, it takes _number_ minutes and costs _number_ pounds.   <!-- predicted: inform_train_reqmore_general: Sure, _reference_ is a _number_ minute trip and each seat costs _number_ pounds. Can I help you with anything else today? -->
* Okay great, could you book me a seat?
    - slot{"train_status": "unique"}
    - offerbook_train: Sure thing. I will work on that for you and be right back with you.   <!-- predicted: nobook_booking_attraction_reqmore_general: I can not. It doesn t give me the option to book tickets. Just general Information. Can I help you with anything else? -->
* What is the departure time for this train? Thank so much!
    - slot{"train_status": "unique"}
    - inform_train_offerbook_train: It departs at _time_ . Can I help you book passage?   <!-- predicted: offerbooked_train_reqmore_general: Great, the train departure time is _time_ , the travel time is _number_ minutes and Train ID is _reference_ . Can I assist with anything else? -->
* No, I don t need to book any tickets at this time.
    - OKay, Do you need any more info then?
* no that is enough thank youu
    - Is there anything else i can do for you today?
* That s it! Bye!
    - If you need anything else, don t hesitate to ask. Have a good day.


## story_SNG02096
* I m looking for a place. I think it s called like Bridge House or Bridge Guesthouse or something.
    - slot{"hotel_status": "available"}
    - slot{"restaurant_status": "available"}
    - inform_hotel: You are looking for the _hotel_name_   <!-- predicted: inform_hotel_reqmore_general: It is a moderately priced guesthouse on the _area_ side of town. It does not offer free parking. Do you want more information? -->
* Could you book it for _number_ people and _number_ nights starting from _weekday_ ?
    - slot{"hotel_status": "NA"}
    - nobook_booking_hotel: Booking was unsuccessful.   <!-- predicted: recommend_hotel_request_booking_hotel: OK, how about _hotel_name_ ? To book a stay I ll need to know the first day you want to stay, how many days, and how many guests. -->
* Okay, book it for _number_ nights starting _weekday_ .
    - slot{"hotel_status": "booked"}
    - book_booking_hotel: Booking was successful.Reference number is _reference_ .   <!-- predicted: book_booking_restaurant_reqmore_general: You re all booked. Reference number is _reference_ . Can I help you with anything else? -->
* Thank you, that s all I need. Good bye.
    - Thank you for using our services.


## story_MUL2427
* I am looking for a _attraction_type_ in _hotel_name_ .
    - slot{"attraction_status": "available"}
    - inform_attraction: We have _number_ cinemas Cineworld in the _area_ , and Vue in the center of town.   <!-- predicted: inform_attraction_reqmore_general: I have _number_ _attraction_type_ attractions. _number_ are in the centre, with _number_ in the _area_ and _area_ . Are you interested in information about _number_ of them in a certain area? -->
* That s great, thank you for your help!
    - select_attraction: Would you prefer something in the center of town, or in the _area_ ?   <!-- predicted: bye_general_welcome_general: You are quite welcome. Thank you for using our services! -->
* Any area is fine. I m also looking for a restaurant in the centre that serves _food_type_ food.
    - slot{"attraction_status": "available"}
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_restaurant: There are _number_ restaurants that fit your criteria. Is there a price range you are looking for?   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* I would like something that is on the cheaper side.
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_inform_restaurant: Sure, _restaurant_name_ is _food_type_ food and is _pricerange_ . Would you like to book a table?   <!-- predicted: inform_booking_restaurant_recommend_restaurant: I would recommend _restaurant_name_ at Thompsons Lane Fen Ditton. Would you like me to book it for you? -->
* Yes, I d like a table for _number_ at _time_ on _weekday_ .
    - slot{"restaurant_status": "booked"}
    - Booking was successful. The table will be reserved for _number_ minutes.Reference number is _reference_ . Can I help you with anything else?
* Yes I need a taxi between _attraction_type_ and restaurant. What do you recommend?
    - request_taxi: I need more information to book that taxi. First, which _attraction_type_ did you decide to visit?   <!-- predicted: nobook_booking_restaurant_request_booking_restaurant: Both restaurants are booked at that time. Will another time work for you? -->
* I suppose the _number_ in the centre makes more sense, since it s close to the restaurant.
    - slot{"attraction_status": "available"}
    - request_taxi: So, you need a taxi between Vue _attraction_type_ , and _restaurant_name_ ?   <!-- predicted: recommend_attraction: _attraction_name_ _attraction_type_ centre	_number_ cb58bs	jesus lane	free_attraction_name_ _attraction_type_ centre	_number_ cb23pq	market square	_number_ pounds_attraction_name_ _attraction_type_ centre	_number_ cb23nz	market street	free_attraction_name_ _attraction_type_ centre	_number_ cb21qy	little saint mary s lane	free_attraction_name_ _attraction_type_ centre	_number_ cb21tt	trinity lane	free -->
* Yes, that would be great. I need to make it to the restaurant by _time_ .
    - slot{"taxi_status": "booked"}
    - OK, a _color_ _cartype_ should be coming to pick you up and the Vue _attraction_type_ , contact number is _number_ . Can I help you with anything else?
* No, thank you, that should be all.
    - bye_general: Thank you! Goodbye.   <!-- predicted: bye_general_welcome_general: You re welcome, farewell! Text back anytime! -->


## story_MUL1620
* Hello! I d like to eat at a _pricerange_ restaurant in the _area_ . Any ideas for me?
    - slot{"restaurant_status": "available"}
    - inform_restaurant: Yes their are _number_ restaurants in the _area_ _number_ serves _food_type_ food the other serves _food_type_ food both meet your price range   <!-- predicted: inform_restaurant_request_restaurant: We have many dining options available in city centre. Do you have a price range or style of food you would prefer? -->
* Can you tell me more about the _food_type_ restaurant please?
    - slot{"restaurant_status": "available"}
    - inform_restaurant_reqmore_general: Yes, it is called _hotel_name_ and is cheaply priced. The phone number is _number_ and the address is Victoria Avenue Chesterton. Is there anything else you d like to know?   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* Can we make a reservation at _hotel_name_ ?
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_request_booking_restaurant: Sure. What day and time would you like to book?   <!-- predicted: offerbook_train_request_train: Sure, I can book you on _reference_ arriving by _time_ . Will this be a reservation for _number_ also? -->
* It will be for _number_ people at _time_ on _weekday_ .
    - slot{"restaurant_status": "NA"}
    - Unfortunately they are booked then, is it alright to choose another day or time?
* Sure. How about _time_ on _weekday_ ?
    - slot{"restaurant_status": "booked"}
    - offerbooked_train: The booking was successful. Your reference number is _reference_ .   <!-- predicted: book_booking_restaurant: Your reservation for _number_ people at the _restaurant_name_ for _weekday_ at _time_ was successful. The table will be reserved for _number_ minutes.Reference number is _reference_ . -->
* Also can you book me a train for _weekday_ ? I want to arrive by _time_ in _hotel_name_ . I m coming from stansted airport.
    - slot{"train_status": "available"}
    - inform_train: I have train _reference_ . It is departing at _time_ and will arrive by _time_ . Would that work for you?   <!-- predicted: inform_train_request_train: There are more than _number_ trains to bishops Stratford, could you tell me what day you would like to leave, where you would like to leave from, and the times. -->
* Yes. What is the reference number for the tickets please?
    - slot{"train_status": "booked"}
    - offerbooked_train: The booking was successful. Your reference number is _reference_ .   <!-- predicted: inform_train_offerbooked_train: Your seats have been reserved. The total fee is _number_ _reference_ payable at the station. Your reference number is _reference_ . Is there anything else I can assist you with? -->
* Thank you so much for your help. That is everything I need.
    - bye_general: You re welcome. Have a nice day.   <!-- predicted: bye_general_welcome_general: You are so welcome. Enjoy your meal. -->


## story_SNG0735
* Hello. I m looking for a _pricerange_ place to eat in the centre. Can you help me?
    - slot{"restaurant_status": "available"}
    - There are _number_ places do you have a food preference?
* Yes, I d love _food_type_ .
    - slot{"restaurant_status": "available"}
    - There are _number_ _food_type_ restaurants meeting your requirements. May I recommend _number_ for you?
* Sure, pick your favorite and let me have the address, postcode, and phone number please?
    - slot{"restaurant_status": "unique"}
    - The _restaurant_name_ is located at _number_ _hotel_name_ Road City Centre, postcode cb21eg, and the phone number is _number_ . Would you like me to make a reservation for you?
* Yes please make me a reservation.
    - slot{"restaurant_status": "available"}
    - Certainly. How many people are dining, and what day and time would you like?
* Actually, I don t need a reservation right now. The restaurant information was all I needed. Thanks for your help.
    - bye_general_welcome_general: You are welcome, enjoy your time in _hotel_name_ .   <!-- predicted: inform_restaurant: There is _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _restaurant_name_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _food_type_ , _area_ _food_type_ , _food_type_ , _food_type_ , and _food_type_ food available in the centre. -->


## story_PMUL1533
* I need a train leaving after _time_ going to _hotel_name_ . Thank you.
    - slot{"train_status": "available"}
    - Where would you like to depart from?
* I want to leave from Peterborough on _weekday_ .
    - slot{"train_status": "unique"}
    - offerbook_train: Train _reference_ would fit the bill, would you like me to book you passage?   <!-- predicted: inform_train_offerbook_train: Ah, it appears that the earliest train, _reference_ , leaves at _time_ , but it does arrive by _time_ . If that is okay, I could book that for you. -->
* Yes, can you book for _number_ people.
    - slot{"train_status": "unique"}
    - offerbook_train: Sure, I will book that for you.   <!-- predicted: offerbook_train_request_train: I will be happy to assist you in booking for this train. How many tickets will you be needing? -->
* I need the reference number.
    - slot{"train_status": "booked"}
    - offerbooked_train_reqmore_general: Okay I booked reservations for _number_ , your reference number is _reference_ . Can I help you with anything further?   <!-- predicted: inform_train_offerbooked_train_reqmore_general: Actually the _weekday_ schedule shows _reference_ with an arrival of _time_ . Your group is booked with the reference number _reference_ . The total fee is _number_ _reference_ . Is there anything else? -->
* Yes, please. I m also looking for a _number_ -star _hotel_type_ with free parking. I d like something moderately-priced, if possible.
    - slot{"hotel_status": "available"}
    - inform_hotel: how about _hotel_name_ ? i hear it s lovely   <!-- predicted: inform_hotel_reqmore_general: There are _number_ moderately priced hotels and guest houses in _hotel_name_ . Do you have any more requirements to help narrow it down? -->
* Sounds great.. Can I have more information
    - slot{"hotel_status": "available"}
    - inform_hotel: Actually, _hotel_name_ doesn t meet your requirements. But I do have other options that are moderately priced, such as _hotel_name_ , Arbury Lodge Guesthouse, and _hotel_name_ .   <!-- predicted: request_taxi: Sure, I can do that. Do you know the name of the restaurant? Also, when would you like to be picked up and arrive by? -->
* Ive heard good things about the _hotel_name_ guesthouse. What is their phone number? And do they have free wifi?
    - slot{"hotel_status": "unique"}
    - Yes, they do have free wifi. Their number is _number_ . Would you like a reservation?
* No that s all right have a great day!
    - bye_general: enjoy your time with us   <!-- predicted: inform_hotel: Actually, _hotel_name_ doesn t meet your requirements. But I do have other options that are moderately priced, such as _hotel_name_ , Arbury Lodge Guesthouse, and _hotel_name_ . -->


## story_PMUL0566
* Hello, I d like some information on a restaurant today.
    - inform_restaurant_request_restaurant: There are _number_ restaurants in _hotel_name_ . To help narrow down results, is there a particular type of food you are looking for?   <!-- predicted: request_hotel: Can you please tell me what type of place and if you have any preferences? -->
* Let s try _food_type_ food.
    - slot{"restaurant_status": "available"}
    - request_restaurant: Sure, do you care if it is _pricerange_ or moderately priced?   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* Moderately priced in centre. I would like to book a table for _number_ at _time_ on _weekday_
    - recommend_restaurant: _restaurant_name_ may have availability.   <!-- predicted: book_booking_restaurant_reqmore_general: All right, I ve made a reservation. Your reference number is _reference_ . What else can I do for you? -->
* Can you book a table for me?
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_reqmore_general: I have booked your table. Your reference number is _reference_ . Is there anything else I can help you with?   <!-- predicted: inform_booking_restaurant_inform_restaurant: _restaurant_name_ is an _food_type_ restaurant on the _area_ side, _number_ Milton Road Chesterton. Phone number is _number_ . Would you like me to book a reservation? -->
* I am also looking for a train that day
    - slot{"train_status": "available"}
    - Where will you go to and from?
* I will leave _location_ and go to _hotel_name_ .
    - slot{"train_status": "available"}
    - request_train: Do you have a time that you need to leave or arrive by?   <!-- predicted: inform_train: The last train with ID _reference_ departing _location_ to _hotel_name_ on _weekday_ will be the best option for you. It will depart by _time_ and arrive by _time_ . -->
* I need to arrive by _time_ . I will also need tickets for _number_ .
    - slot{"train_status": "booked"}
    - I ve got you on the _reference_ , leaving _location_ at _time_ and arriving in _hotel_name_ at _time_ . Reference number is _reference_ and the total fee is _number_ _reference_ payable at the station.
* thank you very much.
    - reqmore_general: Is there anything else I can do for you today?   <!-- predicted: inform_train_reqmore_general: The total travel time will be _number_ minutes. Is there anything else I can help you with today? -->
* That is all I needed thank you for your time.
    - greet_general: You are very welcome. Have a great day.   <!-- predicted: bye_general: My pleasure! Enjoy your trip. -->


## story_MUL2042
* I am looking for a train going to _hotel_name_ and leaving after _time_ .
    - slot{"train_status": "unique"}
    - offerbook_train_request_train: I would be happy to help you find a train. Can you please tell me where you will be departing from?   <!-- predicted: inform_train_offerbook_train: Ah, it appears that the earliest train, _reference_ , leaves at _time_ , but it does arrive by _time_ . If that is okay, I could book that for you. -->
* I ll be departing from _location_ .
    - slot{"train_status": "available"}
    - request_train: What day were you wanting to travel?   <!-- predicted: inform_train_request_train: What day would you be traveling? There are _number_ trains on that route. There is a train that departs _weekday_ at _time_ and will arrive in Ely at _time_ . -->
* _weekday_ departing from _location_ _location_ st. Can you give the arrival time on that train please?
    - slot{"train_status": "unique"}
    - _reference_ leaves at _time_ . It arrives at _time_ . Would you like me to book that for you?
* No thank you. I do need to find a place to stay as well. I need something moderately priced.
    - slot{"hotel_status": "available"}
    - inform_hotel_reqmore_general: There are _number_ moderately priced hotels and guest houses in _hotel_name_ . Do you have any more requirements to help narrow it down?   <!-- predicted: inform_hotel_request_hotel: There are _number_ matching your request. Do you have any preferences such as area, price, parking, or internet? -->
* Yes, I would prefer a _hotel_type_ and a rating of _number_ stars.
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel_recommend_hotel: _hotel_name_ is nice. Free internet too! May I book a room for you today?   <!-- predicted: inform_booking_hotel_inform_hotel: The _hotel_name_ guesthouse _hotel_type_ is located in the _area_ , has a _number_ star rating, and is moderately priced. Would you like me to book it for you? -->
* No thank you, can I please just get their phone number, area, and address? Thanks.
    - slot{"hotel_status": "available"}
    - inform_hotel_reqmore_general: Sure, _hotel_name_ is located in the town centre, at the Sleeperz _hotel_type_ on _location_ . The phone number is _number_ . Can I help you with anything else?   <!-- predicted: inform_attraction_reqmore_general: It is located on Trinity Lane and the phone number is _number_ . The exact address isn t listed. Is there anything else I can help with today? -->
* Can I have the exact address please?
    - inform_hotel: The exact address is Sleeperz _hotel_type_ , _location_ postcode cb12tz.   <!-- predicted: inform_hotel_reqmore_general: Of course! I have Back Lane, Cambourne listed as the address, is there anything else I can help with today? -->
* Great, thank you so much! Goodbye!
    - You re welcome. Goodbye!


## story_MUL1289
* I m trying to plan a trip there but need a _pricerange_ place to stay.
    - slot{"hotel_status": "available"}
    - inform_hotel: _hotel_name_ is located in the centre. They are located at _number_ _location_ road.   <!-- predicted: inform_hotel_request_hotel: Most of the hotels in town offer free parking. Is there a certain area you d like to stay in, or do you have a price range in mind? -->
* Hmm, I m looking for a place in the _area_ . It doesn t need to include internet.
    - slot{"hotel_status": "available"}
    - inform_hotel: _hotel_name_ is _pricerange_ .   <!-- predicted: inform_hotel_select_hotel: There is a guesthouse and _hotel_type_ available which do you prefer? -->
* okay do they have free wifi?
    - slot{"hotel_status": "available"}
    - inform_hotel: Yes, they have free wifi and free parking!   <!-- predicted: greet_general: Great! I can help you with any tourist information you may need. -->
* Okay. Sounds good. Can you tell me the type of _hotel_type_ and provide me with the _hotel_type_ s phone number?
    - inform_hotel_reqmore_general: _location_ is a guesthouse, and their number is _number_ . Can I help with anything else today?   <!-- predicted: inform_hotel: Yes, there is _hotel_name_ . It is located on _number_ _hotel_name_ road. Their phone number is _number_ . -->
* You sure can. I m also quite hungry. Do you have any info on a restaurant called _restaurant_name_ ?
    - slot{"restaurant_status": "available"}
    - inform_restaurant_reqmore_general: Yes, _restaurant_name_ is a _food_type_ restaurant on the pricey side. Would you like their phone number or address?   <!-- predicted: inform_booking_restaurant_inform_restaurant: Absolutely! They are a great _food_type_ restaurant in the centre of town. They are on the _pricerange_ side. Would you like help in reserving a table? -->
* That s fine. I would just like to book a reservation for _number_ at _time_ on _weekday_ . & may I have the reference number?
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant: Yes your reference number is _reference_ .   <!-- predicted: book_booking_restaurant_reqmore_general: I booked that for your for a party of _number_ at _time_ on _weekday_ . The reference number is _reference_ . Is there anything else you need? -->
* I ll need a taxi to get me from the _hotel_type_ to the restaurant.
    - slot{"taxi_status": "available"}
    - request_taxi: I need to know when you would like to be picked up or arrive.   <!-- predicted: select_hotel: Do you want a _pricerange_ _hotel_type_ or a _pricerange_ guesthouse? -->
* I need the tax to get me to the restaurant by _time_ so that I can make our booked time.
    - slot{"taxi_status": "booked"}
    - inform_taxi_reqmore_general: Booking complete. Your taxi will be a _color_ _cartype_ , contact number _number_ . Can I help you with anything else?   <!-- predicted: inform_taxi: Booking completed! your taxi will be _color_ _cartype_ Contact number is _number_ -->
* I think that is all, bye.
    - bye_general_welcome_general: You re welcome, let me know if you need anything else.   <!-- predicted: bye_general_greet_general_welcome_general: Thank you so much for calling! Enjoy your trip! Goodbye! -->


## story_PMUL3940
* I need some information on taking a train from _location_ to _hotel_name_ .
    - slot{"train_status": "available"}
    - Sure, when are you planning to travel?
* _weekday_ , and can you please make sure I get there before _time_ . I don t want to miss Wheel of fortune.
    - slot{"train_status": "available"}
    - inform_train: The last train with ID _reference_ departing _location_ to _hotel_name_ on _weekday_ will be the best option for you. It will depart by _time_ and arrive by _time_ .   <!-- predicted: inform_train_request_train: Perfect. Did you have a departure time in mind? You could leave _location_ as early as _time_ or as late as _time_ and still make it on time. -->
* Thank you. What is the price for that train with ID _reference_ ?
    - inform_train: They are _number_ pounds each   <!-- predicted: inform_train_reqmore_general: Certainly. The travel time is _number_ minutes and the price is _number_ pounds. Is there anything else I can assist with? -->
* Thank you. I am also looking for a _attraction_type_ type attraction in the town centre. Can you tell me what is available?
    - slot{"attraction_status": "NA"}
    - nooffer_attraction: I m sorry I do not have any _attraction_type_ locations in the centre of town.   <!-- predicted: inform_attraction_request_attraction: I m sorry, there are no _attraction_type_ attractions in the centre of the city. Would you like to try a different area of the city? -->
* what about the type of a _attraction_name_ ?
    - slot{"attraction_status": "NA"}
    - nooffer_attraction: I am sorry I do not see any museums in the centre of town.   <!-- predicted: inform_attraction: There is _attraction_name_ it s in the centre. It is on Saint Andrew s street and it s free. -->
* Could you please check again. If you find _number_ could I have the postcode please?
    - inform_attraction: The Broughton House Gallery has the postcode cb11ln.   <!-- predicted: inform_train_offerbook_train: The train ID for that is _reference_ and the travel time is _number_ minutes. Would you like me to book you a seat? -->
* I think that is all I need. Thank you.
    - Thank you for using out service.


## story_SNG1105
* I m looking for an attraction to visit. Is there anything located in the _area_ part of town?
    - slot{"attraction_status": "available"}
    - inform_attraction_request_attraction: There are _number_ attractions in the _area_ part of town. Would you like to visit a _attraction_name_ ?   <!-- predicted: inform_attraction_reqmore_general: I have _number_ _attraction_type_ attractions. _number_ are in the centre, with _number_ in the _area_ and _area_ . Are you interested in information about _number_ of them in a certain area? -->
* No, I was thinking of something fun to do. Do you have any suggestions?
    - inform_attraction_select_attraction: I have several museums to choose from. I also have an _attraction_type_ attraction called _hotel_name_ of a Time. Can I interest you in _number_ of those?   <!-- predicted: inform_attraction_request_attraction: There are _number_ listings for colleges at the city centre, plenty to check out. Do you need info on any particular _attraction_name_ ? Or narrow it down by entrance fee? -->
* _hotel_name_ of a Time sounds like a _hotel_name_ of a time! Yes, can I have their phone number, address, and postcode please?
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: Sure, they re located at unit _number_ , viking way, bar hill, postcode cb238el, and their phone number is _number_ . May I help with anything else?   <!-- predicted: inform_attraction_inform_train_reqmore_general: The _attraction_name_ s address is Market Street, postcode cb23nz. There are many trains arriving in Stansted Airport by _time_ . Would you like to narrow your search further? -->
* No, that s all I need. Thank you!
    - bye_general: Thank you, goodbye.   <!-- predicted: bye_general_welcome_general: You re welcome. Thanks for contacting the _hotel_name_ TownInfo Centre and have a great day! -->


## story_MUL0841
* I am looking for a restaurant in the _area_ part of town.
    - slot{"restaurant_status": "available"}
    - request_restaurant: What type of food are you looking for and what price range?   <!-- predicted: inform_restaurant: The top _number_ places serving _food_type_ cuisine are _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Would you like more options? -->
* I am looking for a restaurant in the _pricerange_ price range and the food type for those restaurants.
    - slot{"restaurant_status": "available"}
    - _food_type_ , _food_type_ , or _food_type_ .
* _food_type_ . And can you find me something to do afterwards in the same area of town?
    - slot{"attraction_status": "available"}
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_inform_restaurant: _restaurant_name_ is a restaurant in the _area_ serving _food_type_ food in the _pricerange_ price range. Do you need more information or want to reserve a table?   <!-- predicted: inform_booking_restaurant_inform_restaurant_reqmore_general: Yes, _restaurant_name_ is a moderately priced _food_type_ restaurant on the _area_ side of town. Would you like a table or more information about them? -->
* I d just like the address for now, thanks. Are there any attractions in the _area_ part of town?
    - inform_restaurant_reqmore_general: The address is _number_ Victoria Road Chesterton. Anything else I can do for you?   <!-- predicted: greet_general_inform_attraction_select_attraction: I am happy to help. There are several types of places to go in the _area_ . Parks, theatre, _attraction_type_ , _attraction_name_ , _attraction_type_ . What sounds good to you? -->
* Could be please call a cab?
    - request_taxi: I d be happy to help you with a taxi, what is your destination departure and what time would you like to arrive leave?   <!-- predicted: request_booking_restaurant: I ll need some more information to make the reservation first. What day and time, and for how many people? -->
* Nevermind, I actually don t need _number_ .
    - inform_attraction_reqmore_general: There are _number_ attractions in the _area_ area of town. Would you like more information?   <!-- predicted: request_taxi: Ok, so you d like a taxi from the restaurant to the _attraction_type_ ? Could you please let me know your desired departure and arrival times? -->
* What is the entrance fee for the attractions?
    - inform_attraction: _attraction_name_ is free in the _area_ part of town.   <!-- predicted: inform_attraction_reqmore_general: Cineworld _attraction_type_ _number_ . I m sorry but the entrance fee is not listed. Is there anything else I can help you with today? -->
* Thanks, that s all I need. Have a nice day.
    - I m happy to help. You have a great day as well.


## story_MUL1607
* I need to find a spot on a train on _weekday_ , can you help me find _number_ ?
    - slot{"train_status": "available"}
    - Yes I can. Where are you going and what time would like to arrive or depart?
* I m leaving from _location_ and going to _hotel_name_ . I d like to leave after _time_ on _weekday_ .
    - slot{"train_status": "available"}
    - inform_train_request_train: I have _number_ options available for _weekday_ . You can leave at _time_ , _time_ . _time_ , _time_ , or _time_ . What time would you like to leave?   <!-- predicted: inform_train: There are _number_ trains within that time frame. The train that will get you to _hotel_name_ closest to _time_ is the _reference_ , which leaves at _time_ and arrives by _time_ . -->
* I ll take the first _number_ at _time_ . When does it arrive?
    - slot{"train_status": "available"}
    - inform_train: It will arrive at _time_   <!-- predicted: inform_train_request_train: There s a train running every day leaving at _time_ and arriving at _time_ . Did you have a particular day in mind? -->
* ok i am also looking for a place to eat in the _pricerange_ price range and should be located in the _area_
    - slot{"restaurant_status": "available"}
    - slot{"train_status": "available"}
    - inform_restaurant_request_restaurant: There are _number_ restaurants available. Is there a specific food type you re looking for?   <!-- predicted: inform_restaurant: The top _number_ places serving _food_type_ cuisine are _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Would you like more options? -->
* No, nothing in particular. Just anything you would recommend.
    - slot{"restaurant_status": "available"}
    - recommend_restaurant: I recommend the _restaurant_name_ located at _hotel_type_ Felix Whitehouse Lane Huntington Road.   <!-- predicted: recommend_restaurant_request_booking_restaurant: I recommend _restaurant_name_ , great word of mouth. What day and time do you want to dine? How many will be going, please? -->
* Can you tell me the food type as well as the phone number and address?
    - slot{"restaurant_status": "available"}
    - inform_restaurant: Yes, it s _food_type_ and the phone number is _number_ , with the address of _hotel_type_ Felix Whitehouse Lane Huntingdon Road.   <!-- predicted: greet_general_inform_hotel_reqmore_general: Of course! The address of the _hotel_name_ is kingfisher way, hinchinbrook business _attraction_type_ , huntingdon and it s phone number is _number_ , would you like anything else? -->
* Thank you very much, that will be all.
    - bye_general: Thank you for using _hotel_name_ TownInfo centre. Please remember us for your future travel needs.   <!-- predicted: welcome_general: you re welcome, thank you for using our system. -->


## story_PMUL4259
* Find me a restaurant in the centre that serves _food_type_ food
    - slot{"restaurant_status": "NA"}
    - nooffer_restaurant_reqmore_general: I m sorry, we don t have anything matching that. Is there something else I can help with?   <!-- predicted: nooffer_restaurant_request_restaurant: I m sorry, but I could not find any listings for restaurants serving _food_type_ style food. Do you have any other favorite types of cuisines? -->
* how about just something that s really overpriced? i don t care if the food is good, just want to impress my boss
    - slot{"restaurant_status": "available"}
    - inform_restaurant_request_restaurant: There are _number_ restaurants fitting your parameters. What kind of cuisine would you like?   <!-- predicted: inform_restaurant: I found _number_ options for you _restaurant_name_ at Regent Street City Centre, _restaurant_name_ at _number_ Mill Road City Centre, and _restaurant_name_ at _number_ _hotel_name_ Road City Centre -->
* What about _food_type_ food?
    - slot{"restaurant_status": "available"}
    - select_restaurant: We have _number_ _restaurant_name_ , and _restaurant_name_ .   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* Let s book it for _restaurant_name_ for _number_ people at _time_ on _weekday_ .
    - slot{"restaurant_status": "booked"}
    - Okay, your booking was successful. Your reference number is _reference_ . Your table will be reserved for _number_ minutes.
* Great. Thank you so much. I also need information on a train to _location_ .
    - slot{"train_status": "available"}
    - request_train: What day and time do you need to travel?   <!-- predicted: inform_train_request_train: There are _number_ trains that travel that route. What day and time would you like to travel? -->
* on _weekday_ and i need to get there by _time_
    - slot{"train_status": "unique"}
    - I have train _reference_ that leaves at _time_ and will get you to _location_ at _time_ . Will that work for you?
* Yes, I actually just needed the train number, so thank you.
    - slot{"train_status": "unique"}
    - offerbook_train_reqmore_general: Can I help you with anything else today or can I book your train ticket for you?   <!-- predicted: inform_train_reqmore_general: travel time is _number_ minutes. Is there anything else I can help with? -->
* No, that will be it. I will book the train later.
    - bye_general: Alright, have a great day!   <!-- predicted: inform_train: The next train leaving from _hotel_name_ for _location_ departs _weekday_ at _time_ , and will arrive by _time_ . -->
* Thanks. You too.
    - bye_general: Thank you very much!   <!-- predicted: bye_general_welcome_general: My pleasure. Please call again if you need more help. I am happy to be of service. -->


## story_PMUL1809
* I m looking for a train that departs from peterborough and arrives by _time_
    - slot{"train_status": "available"}
    - request_taxi: Where would you like to go to?   <!-- predicted: inform_train_request_train: What day would you be traveling? There are _number_ trains on that route. There is a train that departs _weekday_ at _time_ and will arrive in Ely at _time_ . -->
* I am going to _hotel_name_ on _weekday_ .
    - slot{"train_status": "available"}
    - inform_train: There is a train that arrives at _time_ . Would that do?   <!-- predicted: inform_train_select_train: There are _number_ trains available. _number_ leaves at _time_ and the other leaves at _time_ . Which would you prefer? -->
* Sure would. What time does it depart and how much does it cost?
    - slot{"train_status": "booked"}
    - offerbooked_train: leaves at _time_ _number_ _reference_ payable at the station your reference number is _reference_   <!-- predicted: inform_train: Okay the price for a train ticket will be _number_ pounds for _number_ minute ride. -->
* Thanks i appreciate your service. Can you also assist me with finding a place to stay? The _hotel_type_ should be a moderately priced _number_ Star _hotel_type_ .
    - slot{"hotel_status": "available"}
    - request_hotel: What area would you like to stay in?   <!-- predicted: inform_hotel_request_hotel: I show _number_ hotels in the _area_ , _number_ is _pricerange_ and _number_ is _pricerange_ . I also show _number_ _pricerange_ _number_ star _hotel_type_ in the _area_ . Which area do you prefer? -->
* in the _area_ and preferably a _number_ star which is moderately priced
    - slot{"hotel_status": "unique"}
    - inform_booking_hotel_recommend_hotel: _hotel_name_ meets all those requirements, would you like to stay there?   <!-- predicted: inform_booking_hotel_inform_hotel: Yes, they both do. The _hotel_name_ B&B is our inexpensive _number_ star guesthouse. Would you like me to see if I could book you room? -->
* Yes, please. Can you book it for _number_ people and _number_ nights starting from the day we arrive?
    - slot{"hotel_status": "booked"}
    - Booking was successful.Reference number is _reference_
* thanks for the service, that is all I need.
    - enjoy your time with us!


## story_PMUL2433
* Hello, I m looking for an attraction in the type of theatre.
    - slot{"attraction_status": "available"}
    - There is the _reference_ Theatre, _hotel_name_ Arts Theatre, Mumford Theatre, The _hotel_name_ Corn Exchange, and _attraction_name_ . Which would you like to know about?
* Could I get the postcode and entrance fee for the Mumford Theatre please?
    - slot{"attraction_status": "available"}
    - inform_attraction: i don t know the entrance fee but the postcode is cb11pt   <!-- predicted: recommend_attraction_reqmore_general: _attraction_name_ is very famous, free to enter and their postcode is cb23bu. Will there be anything else? -->
* I also need an _pricerange_ restaurant in the _area_ .
    - slot{"restaurant_status": "available"}
    - There are plenty of _pricerange_ restaurants on the _area_ side but if you tell me what kind of cuisine you re interested in, I can narrow it down and recommend _number_ .
* i am not specific on that. recommend _number_ and book for me
    - slot{"restaurant_status": "available"}
    - request_booking_restaurant: I would be more than elated to book it for you, but I need some additional information like when, and how many perhaps?   <!-- predicted: inform_booking_restaurant_inform_restaurant: I have _number_ restaurants that fit those criteria. _restaurant_name_ , _restaurant_name_ , the _attraction_type_ , _restaurant_name_ and restaurant _number_ _number_ . Which would you like a booking for? -->
* I need a table for _number_ people at _time_ on _weekday_ .
    - slot{"restaurant_status": "booked"}
    - Okay, I booked you with _restaurant_name_ . The table will be reserved for _number_ minutes.Reference number is _reference_ .
* Ok, that s all I needed today, Thanks!
    - bye_general_reqmore_general_welcome_general: Okay, great. I m glad I could help. Don t hesitate to contact us again if you need additional assistance. Goodbye.   <!-- predicted: greet_general_inform_attraction: Great! There are thirteen to choose from in that area! -->


## story_MUL2567
* Yeah, I m visiting _hotel_name_ and was wondering if you could tell me about the _attraction_name_ ?
    - slot{"attraction_status": "available"}
    - inform_attraction: Good choice! _attraction_name_ has beautiful _attraction_type_ , located on jesus lane in the town center. Phone number is _number_ .   <!-- predicted: inform_attraction_reqmore_general: I have the _hotel_name_ _attraction_name_ of Technology located in the _area_ side of town. It s at the site of the Old Pumping Station on Cheddar s lane. Would you like more information? -->
* Can you tell me what part of town the _attraction_type_ is located in?
    - inform_attraction_reqmore_general: All Saint s in in the centre of town. Is there anything else you would like to know?   <!-- predicted: greet_general_inform_attraction: That sounds like an exciting trip! _hotel_name_ University Botanic Gardens is located in the centre of town on Bateman Street. Its admission fee is _number_ pounds. -->
* Great, I am also looking to stay at a guesthouse in the _area_
    - slot{"hotel_status": "available"}
    - I found _number_ guesthouses in the _area_ . Did you have a star rating that you wanted?
* No particular star rating but I do want free wifi.
    - slot{"hotel_status": "available"}
    - inform_hotel_request_hotel: Many of the guesthouses in the _area_ offer internet, will you require parking?   <!-- predicted: inform_hotel_select_hotel: I have _number_ options with those specifications. The _hotel_name_ and the _hotel_name_ both with free wifi and parking. Which would you prefer? -->
* Parking is not important. Could you recommend _number_ for me?
    - slot{"hotel_status": "available"}
    - inform_hotel_request_hotel: I am showing _number_ available guesthouses in the _area_ . Could you narrow it down by pricerange or stars?   <!-- predicted: recommend_attraction: I would recommend the _attraction_name_ is located on the _area_ side of _hotel_name_ and the entrance fee is free. -->
* I m looking for a room less then _number_ a night with at least a _number_ star rating.
    - slot{"hotel_status": "unique"}
    - I recommend _hotel_name_ . Although I don t show an exact price it is a moderately priced guesthouse in the _area_ , _number_ stars. Want to book it?
* Yeah, book me a room for _number_ nights, starting _weekday_ .
    - slot{"hotel_status": "available"}
    - How many people is that booking for?
* just _number_ person.
    - slot{"hotel_status": "booked"}
    - book_booking_hotel: Got it! You are successfully booked for _number_ nights starting _weekday_ . Your reference number is _reference_ .   <!-- predicted: book_booking_hotel_reqmore_general: You are booked for the _hotel_name_ . Your reference number is _reference_ . Is there anything else I can assist you with? -->
* Great! I need a taxi to commute between the _hotel_type_ and the _attraction_type_ , too.
    - slot{"taxi_status": "available"}
    - I can get you a taxi from the _hotel_type_ to the _attraction_type_ , I just need to know what time you d like to leave and or arrive by.
* I want to leave the _hotel_type_ by _time_ .
    - slot{"taxi_status": "booked"}
    - I was able to book a _color_ _cartype_ for you, Contact number _number_ .
* Great! That is all I ll need. Thank you and goodbye.
    - Okay, great! have a great trip!


## story_PMUL4842
* I need a restaurant in the centre that serves _food_type_ food.
    - slot{"restaurant_status": "available"}
    - inform_restaurant: sure, i have _number_ options for you   <!-- predicted: inform_restaurant_request_restaurant: There are _number_ _food_type_ restaurants in the area. _number_ are moderately priced and _number_ are _pricerange_ . Can I ask what price range you would like? -->
* I need something in the _pricerange_ price range.
    - slot{"restaurant_status": "available"}
    - recommend_restaurant: Okay, how about _restaurant_name_ ?   <!-- predicted: inform_restaurant: There are _number_ _food_type_ restaurants in the Centre that are in the _pricerange_ price range _restaurant_name_ , _restaurant_name_ , and _restaurant_name_ . Do you have a preference? -->
* Sounds great! Please book a table for _weekday_ at _time_ for _number_ people.
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant: Booking was successful. The table will be reserved for _number_ minutes. Reference number is _reference_ .   <!-- predicted: book_booking_restaurant_reqmore_general: Your table for _number_ is reserved for _weekday_ at _time_ and they ll hold your table for _number_ minutes. Your reference number is _reference_ . Can I help you with anything else today? -->
* Thanks for all your help!
    - reqmore_general: Is there anything else I can help you with?   <!-- predicted: bye_general_welcome_general: You are so welcome. Enjoy your meal. -->
* Yes, actually. I d like to find a guesthouse with free wifi.
    - slot{"hotel_status": "available"}
    - inform_hotel_request_hotel: I have so many. What area would you like to stay in?   <!-- predicted: inform_hotel_select_hotel: I have _number_ different hotels for you, both have free wifi and free parking, would you prefer the Centre area or the _area_ area? -->
* It does not matter but please find a guesthouse in the _pricerange_ range and include free parking.
    - slot{"hotel_status": "NA"}
    - nooffer_hotel: There are no _pricerange_ hotels in the area. Could we look at a moderately priced _number_ ?   <!-- predicted: inform_hotel: Actually, _hotel_name_ doesn t meet your requirements. But I do have other options that are moderately priced, such as _hotel_name_ , Arbury Lodge Guesthouse, and _hotel_name_ . -->
* Actually, how about a _pricerange_ _number_ ?
    - slot{"hotel_status": "available"}
    - request_hotel: What area of town?   <!-- predicted: inform_hotel: _hotel_name_ is a _pricerange_ guesthouse in the centre area. It has a _number_ star rating and includes parking and wifi. It s located at _number_ warkworth street. Phone number _number_ . -->
* In the centre.
    - slot{"hotel_status": "available"}
    - how about _hotel_name_ , it seems lovely.
* Great! What is their postcode?
    - slot{"hotel_status": "available"}
    - inform_hotel_select_hotel: The postal code is CB11eg. May I help you with another aspect of your stay at _hotel_name_ ?   <!-- predicted: greet_general_inform_attraction_reqmore_general: Certainly. The Lynne Strover Gallery s postcode is cb30aq. Can I help you with anything else? -->
* No thank you that will be all
    - reqmore_general: Is there anything else I can help you with today?   <!-- predicted: bye_general_greet_general_welcome_general: Thanks for using our service. Take care. Bye Bye. -->
* That is all I needed.
    - welcome_general: You re welcome, have a great day!   <!-- predicted: bye_general_greet_general_welcome_general: Thank you so much for calling! Enjoy your trip! Goodbye! -->


## story_SNG1075
* I m hoping to find a _attraction_type_ in town.
    - slot{"attraction_status": "available"}
    - inform_attraction_request_attraction: We have _number_ nightclubs. Any preference on entrance fee?   <!-- predicted: inform_restaurant_request_restaurant_select_restaurant: there are _number_ in town. did you have a certain part of town you want to dine in? i have some in the centre and _area_ . -->
* No, can you tell me what the entrance fee is?
    - inform_attraction: The _attraction_name_ costs _number_ pounds. The others are a bit more _pricerange_ .   <!-- predicted: inform_attraction_reqmore_general: Cineworld _attraction_type_ _number_ . I m sorry but the entrance fee is not listed. Is there anything else I can help you with today? -->
* Can you please tell me what the phone number is for _location_ ?
    - inform_attraction: Yes, it is _number_ .   <!-- predicted: inform_attraction_reqmore_general: Certainly, the phone number is _number_ . Is there something else I can assist with? -->
* What is their postcode?
    - _location_ is in postcode cb23qf. Can I help with anything else today?
* No thank you. That is all the information I need.
    - bye_general: Thank you, good bye.   <!-- predicted: bye_general_welcome_general: You are very welcome! Have a great day and I hope you enjoy your visit! Call for help anytime. -->


## story_SNG01332
* I need a taxi to pick me up at _hotel_name_ to leave after _time_ .
    - slot{"taxi_status": "available"}
    - Where would you like to go to?
* I need to get to restaurant _number_ _number_
    - slot{"taxi_status": "booked"}
    - inform_taxi_reqmore_general: Booking completed! Is there anything else I can help you with today?Booked car type _color_ _cartype_ Contact number _number_   <!-- predicted: inform_taxi: Okay! Your taxi is a _color_ _color_ _cartype_ . Contact number _number_ -->
* Thanks! That would be all.
    - reqmore_general: I can also help you with attractions and trains, if you are interested.   <!-- predicted: bye_general: You are welcome. Thank you for contacting _hotel_name_ TownInfo centre. Goodbye. -->
* No, that will be all. Good bye.
    - Thank you for using our services.


## story_SNG0055
* I need a taxi. I am going to _hotel_name_ and I need to leave after _time_
    - slot{"taxi_status": "available"}
    - I will need to know where you need to be picked up?
* I will be at _restaurant_name_ .
    - slot{"taxi_status": "booked"}
    - inform_taxi: Alright I have a _color_ _cartype_ picking you up at _restaurant_name_ at _time_ . The contact number for the taxi is _number_ .   <!-- predicted: inform_taxi_reqmore_general: Alright, I got you booked. the car will be a _color_ _cartype_ and the contact number is _number_ . Anything else I can help you with? -->
* Great that will be everything thanks.
    - bye_general: Have a nice day!   <!-- predicted: welcome_general: You re welcome, glad I could help. -->


## story_MUL2060
* It s _weekday_ and I am bored. Do you have any trains into _hotel_name_ today?
    - slot{"train_status": "available"}
    - request_train: There are many trains, when would you like to depart?   <!-- predicted: inform_train_request_train: There are _number_ trains coming into _hotel_name_ on _weekday_ . Where will you be departing from? -->
* I would like to leave from _location_ after _time_ .
    - slot{"train_status": "unique"}
    - _reference_ leaves at _time_ , would you like me to book that for you?
* Can you give me the price of a ticket?
    - slot{"train_status": "unique"}
    - inform_train_offerbook_train: Tickets are _number_ pounds. Can I book that for you?   <!-- predicted: inform_train_reqmore_general: Sure, _reference_ is a _number_ minute trip and each seat costs _number_ pounds. Can I help you with anything else today? -->
* Great I also need to find a place to stay that doesn t need to have free parking and is in the _pricerange_ price range.
    - slot{"hotel_status": "available"}
    - slot{"train_status": "available"}
    - inform_hotel_reqmore_general_request_hotel: There are _number_ hotels in the _pricerange_ range, any preference on area or anything else?   <!-- predicted: inform_hotel_select_hotel: The _hotel_name_ and the _hotel_name_ are both hotels in the _area_ , _pricerange_ price range with offer free wifi and parking. Which _number_ do you prefer? -->
* _pricerange_ price range in the centre.
    - slot{"hotel_status": "unique"}
    - There are _number_ choices. _hotel_name_ and _hotel_name_ . Do you want to make a reservation at _number_ of these choices?
* I will take _hotel_name_ please.
    - slot{"hotel_status": "unique"}
    - To confirm you want me to book you a room at _hotel_name_ starting on _weekday_ . How many nights will you be staying?
* Yes. Please book it for _number_ people for _number_ nights on _weekday_ .
    - slot{"hotel_status": "NA"}
    - I m sorry, _hotel_name_ is unavailable for those nights. Would you like to try another day or just _number_ night instead?
* Actually, let s back up. I need a place with a star rating of _number_ , in the centre, with free parking. Does the _hotel_name_ have _number_ stars?
    - slot{"hotel_status": "available"}
    - I have the _hotel_name_ that is _pricerange_ and located in the centre. They have a _number_ star rating and offer free parking and free wifi. Would that work for you?
* Yes, that would work for me. Please book it for _number_ people for _number_ nights starting _weekday_ .
    - slot{"hotel_status": "NA"}
    - I m sorry i was unable to book your table for _number_ people for _number_ days on _weekday_ . Would you like another day?
* How about trying just for _number_ night, instead?
    - slot{"hotel_status": "booked"}
    - Booking was successful for _number_ night only. Reference number is _reference_ . Can I be of anything further assistance?
* No, that will be all. Thank you for all of your help!
    - have a nice day, good bye.


## story_PMUL0117
* Hi I am hoping to find a place that is _pricerange_ I can stay at, and also has free wifi.
    - slot{"hotel_status": "available"}
    - inform_hotel: _hotel_name_ near centre is a _number_ star with internet on Regent Street. Phone is _number_ .   <!-- predicted: inform_hotel_request_hotel: Most of the hotels in town offer free parking. Is there a certain area you d like to stay in, or do you have a price range in mind? -->
* Can you find me _number_ with a _number_ star rating?
    - slot{"hotel_status": "available"}
    - inform_hotel: The _hotel_name_ is in the center. The have free internet and parking. their number is _number_ .   <!-- predicted: inform_hotel_recommend_hotel: There are _number_ such guest houses. You might like the _hotel_name_ B and B, which is rated _number_ stars, yet inexpensive, and offers all the luxury the others choices do. -->
* I d like to book this for _number_ people, _number_ nights starting on _weekday_ please.
    - slot{"hotel_status": "booked"}
    - Ok I was able to get this for you. Reference number is _reference_ . Are you looking for places to go as well? I can help with that too.
* Yes can you please assist with _attraction_type_ ?
    - slot{"attraction_status": "available"}
    - request_attraction: What type of attraction?   <!-- predicted: inform_attraction_select_attraction: There are _number_ attractions to choose from in _area_ _hotel_name_ . Would you prefer a _attraction_name_ , a _attraction_name_ , or an _attraction_type_ attraction? -->
* I apologize, I wasn t paying attention to what I wanted. Can you help me find a _food_type_ restaurant in the centre?
    - slot{"restaurant_status": "NA"}
    - Unfortunately, I don t have any _food_type_ restaurants in the city. Is there another type of restaurant I can look for?
* Hmm, is there none at all? Eclectic food?
    - slot{"restaurant_status": "NA"}
    - No, I m sorry. Want to try a different food type?
* _food_type_ , please.
    - slot{"restaurant_status": "available"}
    - inform_restaurant_select_restaurant: There are _number_ places. _number_ are _pricerange_ and _number_ is _pricerange_ . Which do you prefer?   <!-- predicted: inform_restaurant_request_restaurant: I ve got _number_ _food_type_ restaurants in that area, is there a price range you want to narrow it down to? -->
* I need something in the same price range as the _hotel_type_ .
    - slot{"restaurant_status": "available"}
    - inform_restaurant: _restaurant_name_ is in the _pricerange_ price range.   <!-- predicted: inform_attraction: It s located in the _area_ part of town, the phone number there is _number_ , the address is just _attraction_name_ , Milton, the postcode is cb46az. -->
* What is the phone number?
    - slot{"restaurant_status": "available"}
    - inform_restaurant: Their phone number is _number_   <!-- predicted: inform_hotel_reqmore_general: The phone number for the _hotel_name_ is _number_ . Is there anything else I can help with today? -->
* I also need the postcode.
    - inform_restaurant: Sure! Their postcode is _reference_ .   <!-- predicted: inform_restaurant_reqmore_general: The postcode is cb17dy. Is there anything else I can help you with? -->
* Could I book a taxi from the restaurant to the _hotel_type_ please?
    - slot{"taxi_status": "available"}
    - request_taxi: Yes, I can do that. What time would you like to leave?   <!-- predicted: greet_general_request_taxi: We can definitely help with that. Do you need the taxi to the _attraction_name_ or to the restaurant, and what time do you need it? -->
* I would like to leave by _time_ .
    - slot{"taxi_status": "booked"}
    - Booking completed! It will be a _color_ _cartype_ , contact number is _number_
* Great, that s all I needed! Thanks! Bye!
    - bye_general_welcome_general: Yeah, no problem. I am glad I could assist.   <!-- predicted: bye_general: Okay, great! have a great trip! -->


## story_SNG1078
* Do you know where I can find the _attraction_name_ ?
    - slot{"attraction_status": "available"}
    - inform_attraction: Absolutely. _attraction_name_ is on Market Street in the centre of town. Their postcode is cb23nz and is free to enter. Would you need their phone number?   <!-- predicted: inform_attraction_reqmore_general: Certainly! _attraction_name_ is a _attraction_name_ located on the _area_ side of town. Their address is castle street and their phone number is _number_ . Is there anything else? -->
* Great what type of attraction are they?
    - inform_attraction: It is an _attraction_type_ attraction.   <!-- predicted: inform_attraction_reqmore_general: It is a theatre located in the _area_ . Would you like information for it? -->
* That s all the information I need. Thanks for your help!
    - Thank you. Goodbye.


## story_MUL1606
* I am looking for a restaurant named _restaurant_name_ in _hotel_name_ .
    - slot{"restaurant_status": "available"}
    - inform_restaurant: This is a _food_type_ restaurant. It is located at _hotel_name_ Leisure _attraction_type_ Clifton Way Cherry Hinton.   <!-- predicted: inform_restaurant_request_restaurant: There are a total of _number_ _pricerange_ restaurants located in town. Is there a specific area you are going to be in? -->
* Can you book a table for me? Just for _number_ on _weekday_ at _time_ .
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant: I have your table booked. The reference number is _reference_ .   <!-- predicted: book_booking_train_reqmore_general: Your reservation is set. The reference number is _reference_ . Can I help you with anything else? -->
* Great. I ll also need a train to get me there from _location_ King s Cross station.
    - slot{"train_status": "unique"}
    - inform_train_offerbook_train: The _reference_ leaves at _time_ and arrives at _time_ , would that be _number_ you d like to book?   <!-- predicted: inform_train_offerbook_train_reqmore_general: There are departures most days from _hotel_name_ at _time_ . Would you like any more information of train times or help booking a train? -->
* As long it arrives by _time_ going to _hotel_name_ I should be good yes ticket for _number_ please.
    - slot{"train_status": "booked"}
    - inform_train: Reference number is _reference_ . the total fee is _number_ _reference_ payable at the station   <!-- predicted: offerbooked_train_reqmore_general: Sure, the train is actually number _reference_ and your reference number is _reference_ . The price will be _number_ _reference_ payable at the station. Is there anything else today? -->
* That is wonderful. I believe that should be all I need! Thank you.
    - bye_general_welcome_general: You re very welcome, have a wonderful time! Goodbye.   <!-- predicted: bye_general_reqmore_general_welcome_general: Okay, great. I m glad I could help. Don t hesitate to contact us again if you need additional assistance. Goodbye. -->


## story_PMUL3301
* Looking for _hotel_type_ with _number_ star in the center of town.
    - slot{"hotel_status": "available"}
    - inform_hotel_recommend_hotel: The _hotel_name_ is fantastic. It s _pricerange_ , but worth the cost.   <!-- predicted: inform_restaurant_select_restaurant: We have several in the center, and _number_ in the _area_ . They are in assorted price ranges. Do you have any preferences? -->
* Can you book it for me and get a reference number ?
    - slot{"hotel_status": "available"}
    - for how many should i book?
* I actually need to book a specific _hotel_type_ called, the _hotel_name_ .
    - slot{"hotel_status": "available"}
    - inform_hotel: that is a guesthouse located in _area_ and is moderately priced.   <!-- predicted: greet_general_inform_booking_hotel_inform_hotel: Sure, I have it right here. Its a _pricerange_ priced guesthouse with a _number_ star rating, free internet and parking. Phone number is _number_ can I book it for you? -->
* Please book that for _number_ people for _number_ nights starting on _weekday_ .
    - slot{"hotel_status": "booked"}
    - Your booking is confirmed. Your Reference number is _reference_ . Can I assist with anything else?
* Great, I also need to book a train on _weekday_ for _location_ to _hotel_name_ leaving after _time_ .
    - slot{"train_status": "available"}
    - There is a _time_ that would arrive at _time_ . How does that sound?
* Yes what is the price of the ticket and when does the train arrive please?
    - inform_train: it arrives at _number_ and the price is _number_ pounds   <!-- predicted: greet_general_inform_train: Certainly. The train s ID is _reference_ , and the price for a ticket is _number_ pounds. -->
* Great thank you. That will be all for today. Goodbye
    - bye_general: Thank you for using our service!   <!-- predicted: bye_general_welcome_general: You re quite welcome. If you need anything else just message us again. Thanks for contacting the _hotel_name_ TownInfo Centre and have a great day! -->


## story_MUL0682
* I am planning a trip in _hotel_name_ .
    - reqmore_general: What part of your trip may I be of assistance with?   <!-- predicted: greet_general: Great! I can help you with any tourist information you may need. -->
* I am looking for a _hotel_type_ that includes free wifi.
    - slot{"hotel_status": "available"}
    - inform_hotel_select_hotel: I have several options available. Do you prefer a _pricerange_ , _pricerange_ or _pricerange_ price range?   <!-- predicted: inform_hotel_request_hotel: There are _number_ available that match what you re looking for, do you have any preference for what area you want to stay in? -->
* I prefer the _hotel_type_ has at least a _number_ star rating.
    - slot{"hotel_status": "available"}
    - inform_hotel: The _hotel_name_ and the _hotel_name_ in the _area_ are both moderately priced, _number_ star hotels. There is also a more _pricerange_ option in the _area_ . All have internet.   <!-- predicted: recommend_hotel: If price is not an issue, I recommend the _pricerange_ _hotel_name_ . If you want something cheaper, I recommend _hotel_name_ . -->
* Which of those have free parking?
    - Both the _hotel_name_ and the _hotel_name_ have free parking.
* Thank you. I believe I ll try the Lovell. Could you give me their phone number, please?
    - Certainly. That phone number is _number_ .
* Thanks very much. Can you also help me find a train? I d like to travel from _location_ to _hotel_name_ on _weekday_ and I d like to get there by _time_ .
    - slot{"train_status": "available"}
    - inform_train: There are _number_ trains within that time frame. The train that will get you to _hotel_name_ closest to _time_ is the _reference_ , which leaves at _time_ and arrives by _time_ .   <!-- predicted: inform_train_request_train: There are _number_ trains departing from _location_ that will arrive in _hotel_name_ by _time_ . Do you know what day you need to travel on? -->
* Could you book _number_ tickets on that train please? Also, what is the reference number?
    - slot{"train_status": "booked"}
    - offerbooked_train: Alright, you have booked _number_ tickets on _reference_ , leaving at _time_ . Your reference number is _reference_ .   <!-- predicted: inform_train: With pleasure! It will be train number _reference_ . !_number_ pounds per person. -->
* Thank you, that is all I need for now.
    - bye_general: Thank you for contacting _hotel_name_ TownInfo center. Have a great day.   <!-- predicted: bye_general_welcome_general: You re very welcome. Have a great day and text us back anytime! -->


## story_PMUL2146
* I need to find a restaurant in the centre.
    - slot{"restaurant_status": "available"}
    - request_restaurant: Do you prefer a particular type of food or are you looking at a specific price range?   <!-- predicted: inform_restaurant_request_restaurant: There are _number_ restaurants in _hotel_name_ . To help narrow down results, is there a particular type of food you are looking for? -->
* I would like _food_type_ . I have no preference of price range.
    - slot{"restaurant_status": "unique"}
    - inform_booking_restaurant_inform_restaurant: There are _number_ restaurants which meet your needs. _restaurant_name_ is located at _number_ Kings Parade and serves _pricerange_ priced meals. would you like to make reservations?   <!-- predicted: inform_booking_hotel_inform_hotel: We have several such choices in the _area_ , _area_ and _area_ . If you have no preference for location shall I just book _number_ for you? -->
* Yes I need a table for _number_ _weekday_ at _time_ .
    - slot{"restaurant_status": "booked"}
    - Your table for _number_ is reserved for _weekday_ at _time_ and they ll hold your table for _number_ minutes. Your reference number is _reference_ . Can I help you with anything else today?
* I am also looking for an attraction, some type of _attraction_type_ .
    - slot{"attraction_status": "available"}
    - inform_attraction_reqmore_general: I have _number_ listings. _number_ in the _area_ , _area_ or _number_ in the centre. Would you like more information on _number_ of them?   <!-- predicted: inform_attraction_select_attraction: There is the _reference_ Theatre, _hotel_name_ Arts Theatre, Mumford Theatre, The _hotel_name_ Corn Exchange, and _attraction_name_ . Which would you like to know about? -->
* Sure, the _number_ in the _area_ please.
    - slot{"attraction_status": "available"}
    - inform_attraction: I have the _restaurant_name_ located at the plough, green end, fen ditton.   <!-- predicted: inform_booking_hotel_inform_hotel: We have several such choices in the _area_ , _area_ and _area_ . If you have no preference for location shall I just book _number_ for you? -->
* Could you tell me what the postcode is for the _restaurant_name_ ?
    - The postcode is cb58sx. Would you like the phone number?
* no, what the address and area of town, also I will be needing a cab as well.
    - _restaurant_name_ is located at the plough, green end, fen ditton, in the _area_ side of town.
* ok! Thank you! Can you get me a taxi to cambots?
    - slot{"taxi_status": "available"}
    - Absolutely! Just let me know where you d like to depart from, and either what time you want to leave or arrive by.
* I need to be at _restaurant_name_ by _time_
    - slot{"taxi_status": "available"}
    - what will be your depature site?
* Sorry, actually I need to go from _restaurant_name_ to _restaurant_name_ . I want to get there by _time_ .
    - slot{"taxi_status": "booked"}
    - slot{"train_status": "unique"}
    - inform_taxi: Booking completed!Booked car type _color_ _cartype_ Contact number _number_   <!-- predicted: inform_taxi_reqmore_general: No problem; I have booked you a taxi. It is a _color_ _cartype_ , and you may reach them at _number_ . Is there anything else we can help with? -->
* Thank you. What a relief everything is set up now. Again, thanks. Goodbye.
    - reqmore_general: Can I look up anything else before you go?   <!-- predicted: bye_general: Have a good day. Thank you for using _hotel_name_ TownInfo centre. Goodbye. -->


## story_MUL1697
* Hi, are there any trains from _hotel_name_ to _location_ ?
    - slot{"train_status": "available"}
    - I have _number_ results for trains going from _hotel_name_ to _location_ , what day are you looking to travel on and what time would you like to arrive?
* I need to leave on _weekday_ and arrive by _time_
    - slot{"train_status": "available"}
    - inform_train_select_train: I have _number_ that leaves at _time_ and arrives in _location_ at _time_ . Would this be acceptable?   <!-- predicted: inform_train_reqmore_general: I apologize! There are _number_ trains leaving near your requested time. _number_ at _time_ and _number_ at _time_ . Will _number_ of those work? -->
* Yes, I d like _number_ tickets, please.
    - slot{"train_status": "booked"}
    - Great, your _number_ tickets are booked (Ref _reference_ ). Total fee is _number_ ._reference_ , which you ll pay at the station. Can I help with anything else today?
* Yes I need to find a nice _pricerange_ _food_type_ restaurant please.
    - slot{"restaurant_status": "available"}
    - request_restaurant: there are alot of restaurants that fit your needs what area would you like it in   <!-- predicted: inform_restaurant_request_restaurant: There are _number_ _pricerange_ restaurants in town. Do you have a food preference or an area of town you want to eat in? -->
* The area does not matter. They just need to have an available table for _number_ people at _time_ on _weekday_ night.
    - slot{"restaurant_status": "NA"}
    - nobook_booking_restaurant_request_booking_restaurant: I am sorry none of them have booking available for that time,another time maybe?   <!-- predicted: nooffer_restaurant_request_restaurant: Unfortunately, there are no _food_type_ restaurants on the _area_ side. Would you like to try a different type of restaurant or area? -->
* Is _time_ an available time?
    - slot{"restaurant_status": "available"}
    - reqmore_general: I apologize. Can you verify that time for me again please?   <!-- predicted: book_booking_restaurant_reqmore_general: It is booked here is your ref number _reference_ is there anything else you need? -->
* I would like to book a table at _time_ .
    - slot{"restaurant_status": "NA"}
    - nobook_booking_restaurant_request_restaurant: I am not seeing anything available at that time. Maybe we can start from the beginning. You said you are looking for an _pricerange_ _food_type_ restaurant right?   <!-- predicted: nobook_booking_restaurant_request_booking_restaurant: Unfortunately, I could not book the _restaurant_name_ for that day and time. Is there another day or time that would work for you? -->
* Yes. I would like a reservation on _weekday_ at _time_ for _number_ people.
    - slot{"restaurant_status": "NA"}
    - I am unable to get you a reservation at _time_ would you like to pick another time or day?
* how about _time_ on _weekday_ ?
    - slot{"restaurant_status": "NA"}
    - nobook_booking_restaurant_request_booking_restaurant: I m sorry, I have not found a table anywhere for _weekday_ . I have tried _time_ , _time_ and _time_ . Is there any other time you could dine?   <!-- predicted: inform_restaurant_nobook_booking_restaurant_request_booking_restaurant: I m sorry, but I attempted reservations at your specified time at all _number_ restaurants, and none have availability at that time. Would you like to try a different time? -->
* Let is try again, _time_ , _pricerange_ _food_type_ , a group of _number_ on _weekday_ .
    - slot{"restaurant_status": "NA"}
    - nobook_booking_restaurant_request_booking_restaurant: I m sorry, I have not found a table anywhere for _weekday_ at _time_ . Is there any other time you could dine?   <!-- predicted: nooffer_restaurant_request_restaurant: Unfortunately, there are no _food_type_ restaurants on the _area_ side. Would you like to try a different type of restaurant or area? -->
* Is there anything available for _number_ people on _weekday_ at _time_ ?
    - slot{"restaurant_status": "NA"}
    - Unfortunately no. Perhaps you would like to dine at a different time?
* Keep trying. I need the reference number.
    - slot{"restaurant_status": "booked"}
    - book_booking_restaurant_reqmore_general: I was able to book you a table at _restaurant_name_ . Your reference number is _reference_ . Is there anything else I can assist you with?   <!-- predicted: offerbooked_train: I booked your seats for _number_ people on _reference_ departing _hotel_name_ on _weekday_ at _time_ . The total comes to _number_ ._reference_ and your reference number is _reference_ . -->
* No that s it, thank you very much.
    - greet_general: Have a good day and if you need anything else please contact us.   <!-- predicted: bye_general: Have a great trip! Thank you for contacting us for all your booking needs. Enjoy your trip! -->


