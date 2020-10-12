# IH-community-app
International House (IH) is one of the on-campus student accommodations at UNSW, Sydney. The accummodation has been operating since 1968 established by local various Rotary Clubs with a principle to promote “International Understanding” and provide opportunities for local and overseas students to exchange ideas, share their cultural heritage and expand their knowledge.

This web app is a part of MSA project3 submission. The app is aim to connect every resident including ex-residents from IH UNSW and act as an aggregator platform to access any useful information residents may need during their stay.

# Customer Persona
1. Name: Daniel Wang (23)
2. Occupation: A post-grad international student
3. Hobbies: Play sports, workout, watch movies, go clubbing, eat out.
4. Loves: Talking to people. Exploring new knowledge, innovation, technology, and gadgets.
5. Hates: Reading long text/articles.
6. Typical day: 
    8am - wake up and shower and check the news
    8:30 - have a quick breakfast at IH
    9am - go to class
    12pm -  have lunch at IH
    1pm - have another class
    4pm - flexible slot for rest, social network, groceries shopping, clubs & activities.
    6pm - have dinner at IH and catch up with friends sitting on the same table on the plan for weekends.
    8pm - play pools/table tennis in IH Games room with friends
    9pm - study/do homework
    12am - shower and sleep
7. Hopes and Fears:
    I've just arrived in Australia a week ago. I'm not very familiar with the place and how things work yet. Luckily, I've done some online research about the university, Sydney, and the place to stay prior coming here. Getting an offer to stay at IH UNSW during my study is such a good deal to me as neccessary facilities are all available, every meal is catered and I can meet bunch of students from around the world! This make my life a lot easier. However, all the important information and activities are usually announced on Whatsapp and Facebook group which I usually missed it because there're too many chats going on, so usually I'll rely on friends updated me about the in-house activities when we're having dinner. I hope there's a combined platform or mobile app that I can access and stay updated on the events. Also it would be great if I can cross check other residents' name as well because I'm bad at remembering people's name and it's so awkward when I have to ask them multiple times.
    

# App funtionality
- <b>Home page:</b> Users will be presented with picture gallery featuring past events and what's happening around the college. They can also share their experience by uploading the picture from local file to the gallery (the picture will go into Sharepoint first and pulled by Power Apps to be presented on the gallery). Below the gallery is a short-form text pulled from official Twitter account, but because we don't have official Twitter account, it is now linked to my personal account's API at the moment. Ideally, I want to pull picture form Instagram; however, Facebook & Instagram connectors were just depreciated for Power Apps due to disabling Lagacy API (refer to: https://docs.microsoft.com/en-us/connectors/instagram/).
At the bottom of the page features a link to official social networks where users can stay connected based on their preffered platforms. Official social networks are handled by Marketing Directors elected as part of Residents' society (RESOC). 
With these funtionalities on Home page, users can get a sense of belonging and potentially encourage more residents to stay active and participate on events as the “Collegiate Community” is only worthwhile if you get involved and participate in the activities available.

- <b>Events page:</b> Users can stay updated with what activities have been scheduled on a calendar linked to Outlook account. Users will have to select the 'IH events' from the dropdown selector as I couldn't completely delete or rename my personal 'Calendar' from Outlook. I've added some test events during Sep-Nov 2020.
Currently, we rely on Facebook events page, Whatsapp group chat, and physical posters to announce in-house events. With this functionality, users can check them on-demand on their mobile phone and stay updated if there's any change e.g. postpone, cancel without flooding the Whatsapp group chat causing the message to be lost.

- <b>Residents:</b> Currently, resident names, details, and photos are collected before arrival. It is feasible to pull those details from the university's accommodation office and made available on the app for residents to access.
New residents will benefit tremendously from this feature to recognize and get used to their neighbors and find commonalities such as residents who studies the same major. Ex-residents details can still be retained for networking purposes. Filter is added based on user's interest on status of residents, i.e., current or alumni. Furthermore, Users can search name, field of study, and country of origin through searchbox.

- <b>Bookings:</b> Currently, all the bookings for facilities are done through a free shared timetable website, and people will keep asking in the group chat on what's the url to the booking page. I've integrated buttons which redirect to the url on browser (because an in-app browser isn't supported at the moment).

- <b>About us:</b> This is just a simple information page for residents to learn more about a short history and the goal of building IH as a “Collegiate Community”. Currently, this information is stored in a 30-page long handbook from 2018 and I believe majority of residents don't know about this unless they love reading.

# App extensibility
- Current limitation: Due to Facebook's privacy policy, we're not able to import picture from Instagram through hashtag, so I integrated a direct image uploaded using Microsoft Flow to trigger the automation from Power Apps into Sharepoint when a user upload an image into the app through Home page. However, after multiple attempts from more than 10 different tutorials/methods, I can't make it work at the moment for some reasons, but this is the idea.
- The app can be scaled to cover accommodation office for communication such as parcel received, fire drill schedule, check-in/out, etc. This app can also implement on other student accommodations/communities as well.
- On the gallery on Home page, building a funtion to zoom in when clicking on the photo to enlarge them is quite challenging as I've not seen any tutorial available on this topic yet, but it'll definitely be good for User Experience.

