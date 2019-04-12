[![hida](images/hida-128x128.png)](./)

### Content Guidelines
This has all the information that helps author create content in a manner that hida can render effectively.

#### Topic Information
Since a channel is a collection of topics and must be shown to the users (via the list of topics question), it needs to have some standard information. These are (*shown with an example*):

##### Topic Title 
A short title that will appear in lists as well as when starting a topic e.g. **Character Strengths**

##### Topic Desc 
A few words that will appear on the list of topics screens e.g. **It covers information on: what are character strengths; its purpose; the different types; and how to use them. This is based on a workshop conducted by LEADS**.

##### Topic Images
Images are a great way to break the monotony of plain text. This is both while listing in topic list as well as when starting a topic. The platform needs (optionally) two images: small is 48x48 px and a large one of 192x192 px.

##### Topic Actions
This is where the author chooses which of the modes that particular topic should support viz. **E**xplain, **A**sk or **T**est.

---
#### Topic Format
A topic content is a simple text stream. *An example is shown below*:
```
LEAVE TYPES
Leaves can be of the following types:
- Casual Leave (CL) of 8 days per year
- Privilege Leave (PL) of 18 days per year
- Maternity Leave (ML) of 26 weeks
- Paternity Leave (PAL) of 7 days
- Special Leave (SL) of 1 day


CASUAL LEAVE
An employee can avail of 8 days of Casual Leave per year. It can be availed for half a day too. Employees, who are on probation, are credited 4 days of Casual Leave on prorata basis until the employee completes probation.


PRIVILEGE LEAVE
An employee is credited with 18 days of Privilege Leave per year. This is credited after one year of completion. While in probation, 3 PL is credited on probate basis.

This is subject to:
- for leaves exceeding 3 days, the HOD's approval is required 15 days prior to the leave.
- for leaves that exceed 5 days at a stretch, they cannot be availed more than 3 times a year.
- All leave must be availed via the HR system.

```

---
#### Topic Questions
The Author lists all the questions that the topic is scoped to answer. This includes: long answers as well as single or a few word answers. It helps to remember, that the AI system will pick the answer from the text based on what the author has marked. *Examples, of questions from the text may be*:

##### What are the types of leaves
```
Leaves can be of the following types:
- Casual Leave (CL) of 8 days per year
- Privilege Leave (PL) of 18 days per year
- Maternity Leave (ML) of 26 weeks
- Paternity Leave (PAL) of 7 days
- Special Leave (SL) of 1 day
```

##### What is Casual Leave
```
An employee can avail of 8 days of Casual Leave per year. It can be availed for half a day too. Employees, who are on probation, are credited 4 days of Casual Leave on prorata basis until the employee completes probation.
```

##### How much of Casual Leave does a person under probation get
```
Employees, who are on probation, are credited 4 days of Casual Leave on prorata basis until the employee completes probation.
```

---
#### Multiple Paragraph Answers
Simple Answers usually are a single single or at least a single para, where the author just selects the answer from the topic text. However, at times, the answer may span over multiple paragraphs. *Take the example below*.

##### What is Privilege Leave
```
An employee is credited with 18 days of Privilege Leave per year. This is credited after one year of completion. While in probation, 3 PL is credited on probate basis.

This is subject to:
- for leaves exceeding 3 days, the HOD's approval is required 15 days prior to the leave.
- for leaves that exceed 5 days at a stretch, they cannot be availed more than 3 times a year.
- All leave must be availed via the HR system
```
Notice how the answers spans across multiple lines including a blank line after “probate basis”. If you wish that to be the manner in which the content is to be displayed, that blank lines needs to be part of the text.

---
#### One word or a few word answers
At times it is useful to provide answers that are to the point. Just the relevant word or words. This is especially useful when you mark that question as one on which the user may need to be tested. *Examine the following case*:

##### How many days of Privilege Leave is credited each year
```
18
```

---
#### Images in Content
As an author, you may wish to support your voice and text content by an image in an answer. To do so, just insert an img tag as shown below:
```
SHAPE OF CELLS
<img>https://storage.googleapis.com/digital-guru-public/cbse-8-sc-cell/cell_shapes.png</img>Cells are of different shapes. They are usually round, spherical or elongated. Their shape is dependent on their functions. Some are long and pointed at both ends. Some have branches. Some cells like the Amoeba or the White Blood Cells in humans change their shape. The cell membrane and cell wall give shape to a cell.
```
Notice how the image url is placed between two `<img></img>` tags. The URL must be any publicly available address because the Google Assistant retrieves the image from the URL and places it on the screen. It is important to note that if any answer has multiple img tags, only the **first image** within the answer’s range will be considered.

---
#### Video in Content
As an author, you may wish to support your voice and text content by a video in an answer. To do so, just insert an video tag as shown below:
```
WHAT IS CHARACTER STRENGTHS
Character Strengths is our inner strengths that defines our character or personality. It make us, the person we are today. In simple words, as an individual, how we relate to other people and the world around us, is because of our character strengths. This is both, on a personal, and professional level. These are our core strengths with which we are born with, which get enhanced and becomes more  powerful on using them consciously and regularly.

Check out the video on “some common Character strengths. <video>https://www.youtube.com/watch?v=K-3IjNr1gCg></video>
```
Notice how the video url is placed between two <video></video> tags. The URL must be any publicly available address. It is important to note that videos are **not part of the content** that is displayed by Google Assistant. A button is available for the user to tap to call the video which opens on a new screen.

---
#### Text and Speech in Content
By default, the text of an answer is spoken using the set voice of the project. However, at times, one may wish that some of the text need not be spoken. *Take this example*.
```
HOLIDAYS
The following are the holidays for this year:

<silent>
1 Jan (Tue): New Year's Day
14 Jan (Mon): Makkar Sankranti/ Pongal
26 Jan (Sat): Republic Day

4 Mar (Mon): Maha Shivratri
21 Mar (Thu): Holi
. . . 
. . .
</silent>
```
In the above, the Digital Assistant will not read out the holiday dates and names but only the sentence “The following are holidays for the year” because the rest is between the <silent></silent> tags.

---
#### Bold and Italic in Content
At times, you may wish to highlight some part of the text. Google Assistant supports the Markdown or WhatsApp style bold and italics. *Take this example*.
```
CELL DISCOVERY
**Robert Hooke** in **1665** discovered the cell, while observing slices of cork, under a microscope. He noticed compartments like partitioned boxes, which was like a *honey-comb*. He noticed that each box was separated from the other by a wall. He called each box: a **cell**.
```


