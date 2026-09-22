AK LIVE NEWS Calendar — Updated Android Studio Source

मुख्य सेटिंग:
• Birthday: 14 November
• Reminder: सुबह 9:00 बजे
• App branding: AK LIVE NEWS
• Home screen में profile photo की जगह दी गई है।

अपनी फोटो लगाना:
1. अपनी फोटो को profile.jpg नाम दें।
2. इसे app/src/main/res/drawable-nodpi/ में रखें।
3. activity_main.xml में profile_placeholder की जगह @drawable/profile करें।

महत्वपूर्ण:
इस ZIP में आपकी निजी फोटो की binary file शामिल नहीं की गई है, क्योंकि इस runtime में मूल uploaded photo file उपलब्ध नहीं थी। इसलिए placeholder दिया गया है। आपकी फोटो उपलब्ध होने पर उसे drawable में रखकर सीधे इस्तेमाल किया जा सकता है।

Birthday reminder:
Android AlarmManager स्थानीय फोन पर 14 November को सुबह 9 बजे notification दिखाता है।

सभी users को एक साथ notification:
इसके लिए Firebase Cloud Messaging (FCM) + backend/server की जरूरत होगी। यह local alarm से अलग है। Firebase project की google-services.json और server credentials के बिना production push को पूरी तरह चालू नहीं किया जा सकता।

Android Studio:
• Open करें: AKLiveNewsCalendar
• Gradle sync करें
• Run दबाएँ
