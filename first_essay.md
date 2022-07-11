<a href="https://juncture-digital.org"><img src="https://juncture-digital.org/images/ve-button.png"></a>

<param ve-config 
       title="Alice's Visual Essay"
       author="Alice McGrath"
       banner="https://ericayhayes.github.io/audubon/img/derivatives/iiif/images/obj2/full/full/0/default.jpg" 
       layout="vertical">

<!-- Entities discussed throughout the essay are typically defined before the essay text and
     are thus available in all text.  Entity identifiers (QIDs) can be found in either
     Wikipedia or Wikidata (https://www.wikidata.org)> -->
<param ve-entity eid="Q185372"> <!-- Girl with a Pearl Earring painting -->
<param ve-entity eid="Q41264"> <!-- Johannes Vermeer -->
<param ve-entity eid="Q221092"> <!-- Mauritshuis -->
<param ve-entity eid="Q1345"> <!-- Philadelphia -->


# Sample visual essay

This is a sample visual essay demonstrating a few key features of a Visual Essay. Additional [Documentation](https://github.com/JSTOR-Labs/juncture/wiki) and [examples](https://jstor-labs.github.io/juncture-examples) are available for reference.
<param ve-image 
       manifest="https://ericayhayes.github.io/audubon/img/derivatives/iiif/obj2/manifest.json">

# Basic usage

## Image

_Girl with a Pearl Earring_ (Dutch: Meisje met de parel) is an oil painting by Dutch Golden Age painter Johannes Vermeer, 
dated c. 1665. Going by various names over the centuries, it became known by its present title towards the end of the 
20th century after the earring worn by the girl portrayed there.[^1]
<param ve-image 
       label="Girl with a Pearl Earring" 
       description="painting by Johannes Vermeer" 
       license="public domain" 
       url="https://upload.wikimedia.org/wikipedia/commons/0/0f/1665_Girl_with_a_Pearl_Earring.jpg">

## Map

Philadelphia is a wonderful place. 1 August.--I came up here an hour ago with Lucy, and we had a most interesting talk with my old friend and the two others who always come and join him. He is evidently the Sir Oracle of them, and I should think must have been in his time a most dictatorial person. He will not admit anything, and downfaces everybody. If he can't out-argue them he bullies them, and then takes their silence for agreement with his views. Lucy was looking sweetly pretty in her white lawn frock; she has got a beautiful colour since she has been here. I noticed that the old men did not lose any time in coming up and sitting near her when we sat down. She is so sweet with old people; I think they all fell in love with her on the spot. Even my old man succumbed and did not contradict her, but gave me double share instead. I got him on the subject of the legends, and he went off at once into a sort of sermon. I must try to remember it and put it down.
<param title="Philadelphia" eid="Q1345" fill="#E692D1">
<param ve-map center="Q1345" zoom="11" prefer-geojson>

## Map with geojson 

Philadelphia is a wonderful place. 1 August.--I came up here an hour ago with Lucy, and we had a most interesting talk with my old friend and the two others who always come and join him. He is evidently the Sir Oracle of them, and I should think must have been in his time a most dictatorial person. He will not admit anything, and downfaces everybody. If he can't out-argue them he bullies them, and then takes their silence for agreement with his views. Lucy was looking sweetly pretty in her white lawn frock; she has got a beautiful colour since she has been here. I noticed that the old men did not lose any time in coming up and sitting near her when we sat down. She is so sweet with old people; I think they all fell in love with her on the spot. Even my old man succumbed and did not contradict her, but gave me double share instead. I got him on the subject of the legends, and he went off at once into a sort of sermon. I must try to remember it and put it down.
<param ve-map title="Philadelphia neighborhoods" 
       center="40.002498,-75.1180283" 
       zoom="11"
       stroke-width="1"
       fill="blue"
       show-labels
       fill-opacity=".5">
<param ve-map-layer geojson active title="Philadelphia neighborhoods" show-labels url="https://raw.githubusercontent.com/blackmad/neighborhoods/master/philadelphia.geojson"
       label="Custom Label">

## Image comparison
He is evidently the Sir Oracle of them, and I should think must have been in his time a most dictatorial person. He will not admit anything, and downfaces everybody. If he can't out-argue them he bullies them, and then takes their silence for agreement with his views. Lucy was looking sweetly pretty in her white lawn frock; she has got a beautiful colour since she has been here. I noticed that the old men did not lose any time in coming up and sitting near her when we sat down. She is so sweet with old people; I think they all fell in love with her on the spot. Even my old man succumbed and did not contradict her, but gave me double share instead. I got him on the subject of the legends, and he went off at once into a sort of sermon. I must try to remember it and put it down. See this [example of image comparison](https://juncture-digital.org/examples/image-compare/)
<param ve-compare curtain
       url="http://digitalscholarship.brynmawr.edu/24-31/files/original/212b7f244b52afe0b808924dfa221780.jpg"
       label="Goodhart Hall, Bryn Mawr College (1936)"
       attribution="BMC Special Collections"
       license="In copyright"
       >
<param ve-compare
       url="http://digitalscholarship.brynmawr.edu/24-31/files/original/0220d31f95d099a775617266cbf480fd.jpg"
       label="Goodhart Hall, Bryn Mawr College (2014)"
       license="Copyright Bryn Mawr College">

## Multiple viewers

Multiple viewers may be defined for a single paragraph of text.  The first viewer defined is displayed as the default viewer.  
Others are selectable using icons displayed in the top right margin of the paragraph.
<param ve-image 
       manifest="https://iiif.juncture-digital.org/manifest/6dd738aed85597cac540ad31dd5818e86ef7f2918c7b43a9eb3123d5538e6e4c">
<param ve-map center="Q1345" zoom="11">

# References

[^1]: [Wikipedia: Girl with a Pearl Earring](https://en.wikipedia.org/wiki/Girl_with_a_Pearl_Earring)
