<!-- Skillmap template -->
<!-- Each skillmap consists of map properties, paths, and a series of nodes(tutorials/activies) for each path -->

<!-- A skillmap will follow this general format -->
# ID

* skillmapProperty1: Map1
* skillmapProperty2: This is the skillmap.

## Path-1

* pathProperty1: First topic.
* pathProperty2: This is the first topic. 

### Path-1-Activity1

* path1Activity1Property: First activity
* path1Activity1Property2: tutorial
* next: link to the next activity ID

* Path1Activity1TutorialLink: Link
* imageUrl: Link to image 


<!-- Example of a skillmap with functional properties, paths, and nodes/activities -->

<!-- Use a single # heading to define the skillmap ID -->
# skillmap-ID/belt-level

<!-- Set the following properties for the skillmap -->
* name: Skillmap Name
* description: Description of the Skillmap
<!-- Provide a direct link to the background image, use a raw link if direct path doesn't work -->
* backgroundurl: https://github.com/<username>/<repo>/<directPath>
* bannerurl: https://github.com/<username>/<repo>/<directPath>
<!-- Provide a hex value for the following properties -->
* primarycolor: rgb(94, 187, 211) <!-- This provides the color for the path and locked nodes -->
* secondarycolor:rgb(94, 187, 211) <!-- This provides the color for unlocked nodes -->
* tertiarycolor:rgb(94, 187, 211)  <!-- This provides the color for the background -->
* highlightcolor: rgb(94, 187, 211) <!-- This provides the color for the current node border and reward nodes -->

<!-- Use two ## to define a path on the skillmap -->
## path/belt-degree

<!-- Set the following properties for the path -->
* name: Path name  <!-- Ex. First Degree White Belt -->
* description: Description of the Path.

<!-- Now you may define nodes within the current path as tutorials or certificates -->

<!-- Use three ### to define a node for the path -->
### node/activity/current_level

<!-- Set the following properties for each node -->
* name: Level name
* type: tutorial <!-- Set type to tutorial for the node to be an activity -->
* description: Description of the activity. 
* tags: easy, beginner, subject <!-- Separate tags by commas -->
* next: level-2 <!-- This links the current node to the following node -->
* allowedcarrover: <!-- set to true by default to carry over code, may set to false -->

* url: https://github.com/<username>/<repo>/<directPath> <!-- Link to the activity itself -->
* imageUrl: https://github.com/<username>/<repo>/<directPath> <!-- Panel displays image when node is selected -->

### level-2 <!-- Following node linked from previous node -->


<!-- At the end of a path, you may add a node to serve as a certificate of completion! -->
### path_finished

* name: Name of completion node
* type: certificate <!-- Set type to certificate -->
* kind: completion <!-- completion -->
* url: <!-- Link to certificate -->