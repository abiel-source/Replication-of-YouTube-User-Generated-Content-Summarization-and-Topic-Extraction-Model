[Click here to view the Proposal Report (PDF)](Proposal_Report.pdf)

[Click here to view the Milestone Report (PDF)](Milestone_Report.pdf)

[Click here to view the Final Report (PDF)](Final_Report.pdf)

**ABSTRACT**

In 1956, George A. Miller proposed his notion of "The Magical Number" regarding an
exploration of human memory and its limitations. His paper, titled "The Magical Number
Seven, Plus or Minus Two", posits that the human (short term) memory is only able to retain
roughly 5 to 9 "chunks" of information at a
time. Fast forward to the 21st century, large
scale digital platforms offer information at unprecedented volumes, leading to cognitive and
information processing problems such as information overload. Our paper explores the
notion of information overload with respect to
the YouTube platform, and more specifically,
deep learning methods and NLP techniques that
solve information overload with respect to summarizing and compressing general viewership
of a YouTube video comment section. By accessing the comments on any YouTube video,
an AI comment section summary can be used
to determine what users are talking about in a
video. i.e. By taking in large swaths of natural language text, our model attempts to output
abstractive summaries of a number of these topics. The model is intended for use on native
YouTube comments and is built to replicate the
YouTube Topic AI model.

**INTRODUCTION**

As the digital age progresses forwards, the amount
of information that is available to society is increasing exponentially. Due to population growth,
increased ease of access to the internet, and the
continued cultural shift towards electronic commerce and electronic communication, social media
platforms are being brought to the forefront of communication. While some of these communications
are directed towards another, a large amount of
communication is intended for the general populace to peruse. Examples of this include tweets,
Facebook posts and comments on YouTube videos,
as opposed to directly messaging someone.

Due to the incomprehensible amount of content
that is generated on a day-to-day basis, it is impossible for one to watch every video or read through
every post on social media. As evidence, YouTube
alone receives 500+ new hours of video uploads every minute (YouTube Official Blog). Using summarizer models, which take in large swaths of data and
output more easily digestible sentences or phrases,
what was previously thought of as unapproachable
is now significantly easier to comprehend.
Taking inspiration from YouTube’s recent feature currently in beta testing, YouTube Topics, we
have attempted a replication of the comment summarization system currently being worked on. By
taking the contents of the comment section of any
YouTube video and cleansing the data to remove
usernames, the transformer-based model we have
created first performs k-means clustering in order
to determine the number of topics that it should be
summarizing, before summarizing each individual
cluster in an easy-to-understand sentence or two.
In this manner, by taking the closest n comments
of each cluster of YouTube comments and appending them together, our model is intended to summarize the topic behind each of the clusters and output
a one-line summary of the discussion happening.

We tested several methods for both the clustering of k-means and the summarizer model. For
the k-means clustering, we determined the number
of clusters in three ways; the elbow method, the
silhouette method, and by matching to the number
of topics on a YouTube video in question. With
regard to our model, we changed our base model
between Google’s T5 base, Google’s T5 small, and
Facebook’s BART base.

**APPROACH**

The high-level approach and system pipeline remained consistent since the project proposal with
heightened details with respect to low-level implementation decisions. To reiterate, the ultimate
project objective is to engineer an NLP system
that takes in a swath of user-generated comments
and outputs a summary of key overlapping topics
as a means of communicating general viewership
thought or sentiment.

Our proposed system pipeline comprises two
primary systems which abstractly factor the project
directive into two more tractable tasks. Namely,
the identification of key overlapping topics via Kmeans clustering followed by the summarization of
each key topic via a deep-learning NLP model. The
following sections elaborate on the implementationspecific decisions that we made to bring this system
to life.


[Click here to view the Proposal Report (PDF)](Proposal_Report.pdf)

[Click here to view the Milestone Report (PDF)](Milestone_Report.pdf)

[Click here to view the Final Report (PDF)](Final_Report.pdf)
