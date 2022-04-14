---
link: https://github.com/upenndigitalscholarship/audubon-birds-of-penn
location: University of Pennsylvania Libraries
layout: work
slug: audubon-in-action 
title: "Audubon in Action: Creative Approaches to Data" 
thumb-img: 
banner-img: audubon-in-action.jpeg
img-source: 
img-source-url: 
status: current
start-year: 2022
end-year: present
context: "Experiment with the latest project, Birds of Philadelphia, which uses high-resolution images of Audubon's plates from The Birds of America alongside crowdsourced observation data to consider the depiction of wildlife data through visual, aural, and interactive components."
role: Project Manager/Developer

---


In this session, come test emerging technologies and digital methods to enhance the impact of the Penn's collections. Experiment with the latest project, Birds of Philadelphia, which uses high-resolution images of Audubon's plates from The Birds of America alongside crowdsourced observation data to consider the depiction of wildlife data through visual, aural, and interactive components. Participants will find creative ways to amplify, build on, and disseminate data from environmental collections and crowdsourced projects. Read more about this project here.

This workshop was hosted as part of Earth Week Data Jam, a week of working and playing with enviornmental data with the Center for Research Data and Digital Scholarship (RDDS) at Penn Libraries.

### Process

Plate images from Audubon's Birds of America were downloaded from Nathan Buchar's GitHub repository, compiled from the Audubon Foundation. Observation data was exported from the Birds of Philadelphia project on iNaturalist, filtered for only those observations posted with a license.

For any observation data with an associated image or sound, these files were exported and saved to a folder named for the corresponding common bird name. Additional sound files were downloaded via the xeno-canto API, querying based on the common bird names. Birds were then matched, by common name, to the corresponding plate images - only those that were matched were included in the project.

Photomosaics were created using a script by Data Dolittle.Display posts were created using Pillow (Python Imaging Library), including the common name, scientific name, and information about the number of observations and last observation recorded on iNaturalist.

The sonification of the observation data was created using Pydub, where 1 second is the equivalent of 1 day of observations. For any day when birds were observed, a random sound file for the corresponding bird was appended to the file. (Datasets for individual bird sounds that were downloaded for this project are labeled with the common name of the bird and available in the sounds folder.) Individual citations for each sound file can be generated from those datasets.) Silence means no birds were observed on that day.

### Resources 


 
