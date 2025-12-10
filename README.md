

# **Big-Data-Russian-Troll-Tweets**

This project analyzes a large dataset of tweets produced by Russian troll accounts connected to the **Internet Research Agency (IRA)**.
Through data exploration, sentiment analysis, hashtag analysis, and network analysis, we investigate how troll operations influenced political discourse—particularly during the **2016 U.S. Presidential Election**.

The project integrates findings from our own analysis (slides + notebook) and contextual background from public investigations, including NBC News’ open dataset and the Mueller indictment.

---

## **Background: How Russian Trolls Operated**

In 2018, NBC News released a dataset of tweets from **2,752 IRA-controlled accounts** suspended by Twitter. Although Twitter deleted the accounts, journalists reconstructed part of the dataset, enabling graph-based investigation.

Russian troll accounts typically fell into **three categories**:

### **1. “Typical American citizen” personas**

Fake profiles posing as everyday U.S. users, often posting political content, emotional reactions, or photos from real-world events.

### **2. Fake local news outlets**

Accounts like *OnlineCleveland* or *KansasDailyNews* pretended to be local media, sharing exaggerated crime stories to generate fear and polarization.

### **3. Fake political groups**

Accounts such as *TEN_GOP* (explicitly named in the Mueller indictment) mimicked official political organizations to influence partisan communities.

A key insight:
Most troll accounts **barely produced original content** — instead, they heavily **retweeted** a small set of “core” troll accounts to amplify their message.

Graph analysis (PageRank + community detection) reveals **three major communities**, aligned roughly with:

* Right-wing political themes (#MAGA, #TrumpTrain)
* Left-leaning criticism (#ObamasWishlist, #RejectedDebateTopics)
* Black Lives Matter–related topics (#BlackLivesMatter, #BLM, #Racism)

Each community had a handful of **content generators**, while the majority acted as **amplifiers**.

---

## ** Key Findings from Our Analysis**

### **1. Tweet Activity Over Time**

From the slides (page 2), activity was minimal until **2014**, surged sharply in **2015–2016**, and collapsed after **2017**.
This behavior shows **event-driven, coordinated operations**, not organic user activity.

### **2. Top Mentioned Usernames**

Mentions cluster around a small set of high-visibility accounts (slide page 3), forming **target nodes** amplified deliberately.

### **3. Hashtag Polarization**

* **Left-wing trolls** used hashtags like *#BlackLivesMatter*, *#Resist*, *#NotMyPresident* to intensify internal Democratic conflict (slide page 4).
* **Right-wing trolls** pushed *#MAGA*, *#TrumpTrain*, *#DrainTheSwamp* to amplify pro-Trump narratives (slide page 5).

### **4. Sentiment Analysis (2016)**

Both left- and right-wing troll sentiment reacted **instantly** to major events (Podesta leaks, RNC convention, U.S. election).
Left trolls remained **consistently negative**, while right trolls shifted **positive** toward the election period (slide page 6).

### **5. Bernie vs. Hillary Attacks**

Troll activity showed asymmetric targeting (slide page 7):

* Slightly positive toward **Bernie**
* Strongly negative toward **Hillary** (especially from right-wing trolls)

This suggests a strategy to **amplify Democratic division**.

### **6. Network Interpretation**

The mention-based network (slide page 9) shows:

* **Right-troll accounts dominate as hubs**
* Edges only appear when ≥ 3 trolls mention the same user
* Clusters reveal **coordinated groups**, not natural conversation structures

### **7. PageRank Results**

As in the article and our slides (page 10), PageRank helps identify:

* Structurally influential accounts
* Hidden bridges between communities
* Troll clusters acting like **coordinated influence cells**

---

## **Technologies Used**

* **Python**, Jupyter Notebook
* **Pandas**, **NumPy**
* **Matplotlib**, **Plotly**
* **NLTK/TextBlob** for sentiment
* **NetworkX** for graph analysis
* **Neo4j inspiration** for community/PageRank methodology

---


---

## *Authors**

* Fabio Antonicoli
* Tommaso Milanino
* Lorenzo Buellis



