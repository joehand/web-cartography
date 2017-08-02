## Web Cartography Final Project

Goal: tell a story you a personally engaged with via an interactive map.

Steps:

1. Proposal - Create a brief proposal on the problem, story, and data needs for your project (< 350 words)
2. Beta Map - Put your data on a map!
2a. Beta data pipeline (if applicable) - create a full pipeline for your data.
3. Final Map Experience - present map to class on **August 30th**!

#### Timeline

* August 7th - Proposal
* August 14th - Data pipeline proposal (if applicable)
* August 16th - Beta Map
* August 21st - Data pipeline implementation
* August 30th - Final map

We will have class time weekly to work on projects and address any questions or roadblocks. If you want to bounce ideas off me before drafting a full proposal or starting any part, please do!

### 1. Proposal

**Draft Due Monday August 7th**

* Problem Statement - What is the problem you are attempting to address with your map?
* What story to tell - What story will you tell with your map and data to highlight unique angle of your problem?
* Data needs - What data will you use? how will you access the data? does it need to be cleaned/processed before putting on a map?

I'll give feedback on the draft and we can iterate based on the draft. Please have it in on Monday to give us enough time!

#### Example Proposal

As Portland continues to grow, many people continue to get around in single occupancy vehicles. Increasing traffic and commute times proportionally burdens public transit vehicles more than private vehicles. Additionally, it makes transit harder to depend on, reduces service convenience, and makes users more likely to use a car for the next trip (if you're sitting in traffic anyways, may as well be in more comfort). Recently, groups such as the [Portland Bus Lane Project](https://portlandb.us/) have started to advocate for transit only lanes. However, the scope of the problem is difficult to convey.

We've all seen maps of Portland covered in red showing the traffic. Often we just think of cars and traffic, but buses also get stuck in them! My map will focus on the total delay throughout the Trimet system, and how many full or nearly full buses are delayed. By highlighting buses stuck in traffic, how full they are, and total ridership delays, we can show the urgency of the situation. If time permits, I can also start to identify particular routes that are more impacted.

Trimet provides an API of lie vehicle locations with some metadata. The API is a bit inconsistent and doesn't provide GeoJSON directly. To improve user experience, I will create a module to fetch data from the API, process, and cache it on a server. To improve the live updates, I will look at tools for streaming the data to the client.

### 2. Beta Map

**Due August 16th**

Put your data on a map! This should be a mvp type map. The goal is to show me (and yourself) that the data can be put on a map and give us the opportunity to start seeing what stories we can tell with the data.

#### Example

Joe's live trimet map (link todo)

#### 2a. Data Pipeline

**Proposal Due August 14th**

**Code Due August 21st**

The data pipeline will get your data from your source to your map. For some, this may be a geojson ajax call, like we were doing in the early leaflet maps. And for others, this map be a more involved pipeline involving data processing or making the data available as tiles or through other formats.

##### Proposal

The proposal is a short description, building on your project proposal, of what tools you'll make use of to get your data from source => map. It should be similar but more specifically identify the tools needed.

Example:

> On a server, I will fetch data from the trimet API, select the properties I need, turn it into GeoJSON, and make it available over Dat and via websockets. I will only store the raw data as geojson on the server. My client side map will use the data via websockets to live update vehicle locations and calculate relevant stats on demand.

##### Implementation

Build your data pipeline in code form. If possible, this should be done as standalone modules.

Example:

* [Server side](https://github.com/joehand/trimet-live-archive)
* TODO: [Client side]()

### 3. Final Map Experience

Build your final map and be prepared to present it to class on August 30th. 
