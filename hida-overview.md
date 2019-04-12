[![hida](images/hida-128x128.png)](./)

### Terminology
#### **Channel**
This holds all the organisations content that is available to a user by using an **invocation** in Google Assistant. For example, in the demo, **Talk to Digital Trainer** was the invocation that directed all requests from the user to the *Digital Trainer* content. For purposes of convenience, we call this customised content and its working as a **Channel**.

#### **Topics** 
For purposes of ease, the hida platform groups content into **Topics**. Topics help a user identify the content they are interested in. Examples of a topic can be: *HR Policy*, or even just *Leave Policy*, or *Product Details of ...* and so on. We recommend that a topic should not be very large for better performance. A topic scope, where all the contents of a topic can get answered in about **50 questions**, would be a suitable size.

#### Content
Think of a **topic content** as a plain text file which holds all the answers to the questions related to that topic. Of course, the content creator (author) may wish to add images, or provide a link to a video, or apply some highlighting to some part of the text to make it more interesting. Check the ![content guidelines](images/content-guidelines.html) to know more about it.

#### Question & Answer
Authors are expected to list all possible **unique questions** (to the extent possible) that can be answered from within the content. For every question, they need to pick that part of the content where the **answer** lies. The question provided by the author is indicative one, while the actual user may ask it in a different manner. It is the job of **hida** to decipher that.

#### Topic Functionality
Using the question-answer based content of each topic, the author can choose to provide one or more of three functionalities to the user. They are (explained below): **Ask**, **Explain** or **Test**.


