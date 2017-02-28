
# Esox masquinongy
## common name: Muskielunge


```
import urllib.request
import json

muskie_url = "https://fishbase.ropensci.org/species/?genus=Esox&species=masquinongy"

raw_json = urllib.request.urlopen(muskie_url)
decoded_json = raw_json.read().decode('utf-8')
parsed_json= json.loads(decoded_json)
raw_json.close()

```

```
print("Threat to humans: " + parsed_json["data"][0]["Dangerous"])
```


```python
print("Comments: " + parsed_json["data"][0]["Comments"])

```

    Comments: Lives in clear vegetated lakes, quiet pools and backwaters of creeks and small to large rivers (Ref. 205, 10294).  Solitary, lurking hunter on other fishes as well as on ducklings, muskrats, and snakes. Oviparous, spawn in spring as the ice melts (Ref. 205).



```python
print("Used for Aquaculture: " +parsed_json["data"][0]["UsedforAquaculture"])
```

    Used for Aquaculture: commercial


# Oncorhynchus mykiss
## Common name: rainbow trout


```python
import urllib.request
import json

steelhead_url = "https://fishbase.ropensci.org/species/?genus=Oncorhynchus&species=mykiss"

raw_json2 = urllib.request.urlopen(steelhead_url)
decoded_json2 = raw_json2.read().decode('utf-8')
parsed_json2= json.loads(decoded_json2)
raw_json.close()
```


```python
print("Threat to humans: " + parsed_json2["data"][0]["Dangerous"])
```

    Threat to humans: potential pest



```python
print("Comments: " + parsed_json2["data"][0]["Comments"])

```

    Comments: Adults inhabit cold headwaters, creeks, small to large rivers, and lakes.  Anadromous in coastal streams (Ref. 5723).  Stocked in almost all water bodies as lakes, rivers and streams, usually not stocked in water reaching summer temperatures above 25°C or ponds with very low oxygen concentrations.  Feed on a variety of aquatic and terrestrial invertebrates and small fishes. At the sea, they prey on fish and cephalopods.  Mature individuals undertake short spawning migrations.  Anadromous and lake forms may migrate long distances to spawning streams (Ref. 59043). Utilized fresh, smoked, canned, and frozen; eaten steamed, fried, broiled, boiled, microwaved and baked (Ref. 9988).  Cultured in many countries and is often hatched and stocked into rivers and lakes especially to attract recreational fishers (Ref. 9988).



```python
print("Used for Aquaculture: " +parsed_json2["data"][0]["UsedforAquaculture"])
```

    Used for Aquaculture: commercial



```python

```


```python

```
