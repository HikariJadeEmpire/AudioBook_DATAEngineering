# AudioBook_DATAEngineering
> End-to-end Data Engineering process

#
### Technologies
- Database : ```SQL``` , ```REST API```
- Language : ```Python```

#
### Data Pipeline Architecture

![Personal visualization - Hikari #39;s architecture](https://github.com/HikariJadeEmpire/AudioBook_DATAEngineering/assets/118663358/edd67ad7-a8e3-4b70-b87b-09e09be6ee6b)


# <h3> DATASET </h3>

More info about dataset can be found here:
- **Website :** [Here's one of the sample data.](https://www.audible.com/pd/The-Power-Broker-Audiobook/B0051JH67K?ipRedirectOverride=true&overrideBaseCountry=true&pf_rd_p=2756bc30-e1e4-4174-bb22-bce00b971761&pf_rd_r=MF7KC1JQF3A6GK2ET8XM)
- **Size :** *1.9+ M* rows

<br>

from **mySQL** Database example : <br>
1st table

| Book_ID	| Book Title | Book Subtitle |	Book Author |	Book Narrator |	Audio Runtime |	Audiobook_Type |	Categories |	Rating |	Total No. of Ratings |	Price |
|---------|------------|---------------|--------------|---------------|---------------|----------------|-------------|---------|-----------------------|--------|
| 1 |	Bamboozled by Jesus |	How God Tricked Me into the Life of My Dreams |	Yvonne Orji	| Yvonne Orji |	6 hrs and 31 mins |	Unabridged Audiobook |	Biographies & Memoirs |	5 |	47.0 |	$29.65 |
| 2 |	Sixth Realm Part 1 |	A LitRPG Fantasy Series (The Ten Realms, Book 6) |	Michael Chatfield |	Neil Hellegers |	13 hrs and 33 mins |	Unabridged Audiobook |	Science Fiction & Fantasy |	4.5	| 98.0 |	$24.95 |
| 3 |	Go Tell the Bees That I Am Gone |	Outlander, Book 9	| Diana Gabaldon	| Davina Porter |	27 hrs and 30 mins |	Unabridged Audiobook |	Science Fiction & Fantasy |	None	| NaN	| $41.99 |
| ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |

<br>

2nd table

| timestamp |	user_id	| book_id |	country |
|-----------|---------|---------|---------|
| 2021-05-01 00:00:01 |	ad8eca41 |	1584	| Portugal |
| 2021-05-01 00:00:03	| 561b26c1 | 829	| United States of America |
| 2021-05-01 00:00:04 |	81f149e5 |	1391 |	Japan |
| ... | ... | ... | ... |

<br>

from **REST API** example :

|   | conversion_rate |
|---|-----------------|
| 2021-04-01 |	31.194 |
| 2021-04-02	| 31.290 |
| 2021-04-03	| 31.256 |
| ... | ... |

<br>

# <h3>Description</h3>
To gain a better understanding, you can check out my separate data cleaning process here. <br>

- Getting data from source :

  [![](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1dTeNW17m5obf4TU7nM5JkfoBOAvKdaub)

- Transforming data using ```Spark``` :

  [![](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1M0-kGkxmUccp4w87P5Cqqz6yPH0O1pv5)

# <h3>Pipeline Orchestration</h3>

- **My Capture :**   [cap :camera:](https://github.com/HikariJadeEmpire/AudioBook_DATAEngineering/blob/main/AirflowJob.JPG)
- **My CODE :**   [code :iphone:](https://github.com/HikariJadeEmpire/AudioBook_DATAEngineering/blob/main/ApacheAirflow_manage.py)

![Data_Orchestration](https://github.com/HikariJadeEmpire/AudioBook_DATAEngineering/assets/118663358/fa66e1ab-4414-4f12-8a7d-a8392396d55a)

#
Go to top : [Top :world_map:](https://github.com/HikariJadeEmpire/AudioBook_DATAEngineering#audiobook_dataengineering)
