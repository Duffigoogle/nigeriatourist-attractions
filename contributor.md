# Contributing

There are two ways to contribute to this project:

## Using the form
You can upload details of your tourist attractions directly to the online form here: https://docs.google.com/forms/d/e/1FAIpQLSfdb-9dvaF48k-MqCljlIj7nzAOc5PdQgAd2PaUrM0AVXpgVw/viewform?usp=pp_url. This usually takes about 72 hours to be reviewed and merged.

## Sending in a pull request
Another way to contribute is to directly send in a pull request. Here are some guidelines for this:

1. Ensure that the details of the tourist attraction have been properly verified like:
    Kindly ensure your details are accurate. Also, your PNG file should be clear and not more than 4mb.

2. Add a folder to **tourist_attractions** named after your choiced tourist attraction. In this folder, put the png versions of your tourist attraction. The files should have the same name as the folder and should be lowercase. If your tourist attraction's name has multiple words, kindly separate them with an underscore.

### Folder Structure
```
tourist-attraction_name
| tourist-attraction_name.png
```

3. In **[nigeriatouristattraction.json](https://github.com/duffigoogle/nigeriatourist-attractions/blob/master/logos.json)**, add a `JSON` entry for your tourist attraction.

### JSON Object
```
{
  "title": "Tourist Attraction Name",
  "name": "tourist_attraction_name",
  "url": "https://tourist_attraction_url.com",
  "category": ["Category"]
}
```
**Example**
```
{
  "title": "Ogbunike Caves",
  "filename": "Ogbunike_Caves",
  "url": "https://www.ogbunikecaves.com/",
  "category": ["Outdoor", "Adventure", "Caves", "Exploration"]
}
```

4. If your tourist attraction category is not reflected in categories section *below*, feel free to use a new category.
If you do so, kindly edit this file; adding the newly used category (**[/contributing.md](https://github.com/duffigoogle/nigeriatourist-attractions/blob/master/contributor.md)**) in your PR as well.
**NB:** Your jsonObject category can also be a combined form 2 or more categories in this form:  **e.g.**
```
"category": ["RESORT", "Beach"] or
"category": ["RESORT", "Beach", "Bar"] or
"category": ["RESORT"]
```

5. Make sure your company URL has the `http://` or `https://` prefix or it will be rendered as invalid (this is to prevent some quirks in link redirection).
**NB:** By default, all empty or invalid urls will be linked to google search rather than the official website.
```
"url": "https://thelastgoodman.com" or
"url": "https://www.thelastgoodman.com"
not
"url": "thelastgoodman.com" or
"url": "www.thelastgoodman.com"
```

### Categories
```
* Outdoor
* Hiking
* Adventure
* Waterfall
* Mountain
* Resort
* Farm
* Beach
* Hotel
* Park
* Festival
* Cave
* Exploration
* Boating
* Canoeing
* Games
* Sports
* Museum
* Sculpture
* National Park
* Games Reserve
* Art
* Gallery
* Archery
* Bar
* Club
* Garden
* Arcade
* PaintBall
* Cinema
* Monastry
* Spring
* Confluence
* Bird Watching
* Train Ride
* Polo Club
* Lake
* Palace
* Zoo
* Wine Tasting
* Santuary
* Shrine
* Statue
* Camping
* Picnic
* Canopy Walkway
* Swimming
* Floorboard games
* Tree house 
* Dams
* Monument
* Ranch
* Carnival
* Hill
* River
* Rock
* Art Gallery
* Tomb
* Palace
* Boating & Fishing Lake
* Cottage
* Monoliths
* Port
* Dyeing Pits
* Pottery
* City Walls
* Cenotaph
* Mangroove
* Relics
* Eco-Tourism
* Theatre
* Garden
* Golf Course
* Dam
* Cementery
* Colonial
```

**NOTE**: _Pull requests are usually reviewed within 24 hours. Once your pull request is merged, you should see your tourist attraction on the site a few minutes after._
