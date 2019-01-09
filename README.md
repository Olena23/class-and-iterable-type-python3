In this project you are asked to create a sequence type that will return a series of (regular convex) Polygon objects.

Each polygon will be uniquely be defined by:
* it is a regular convex polygon:
    * edges (sides) are all of equal length
    * angles between edges are all equal
* the center of the polygon is `(0,0)`
* the number of vertices (minimum `3`)
* the distance from the center to any vertex should be `R` unit (this is sometimes described as the polygon having a *circumradius* of `R`)

The sequence should be finite - so creating an instance of this sequence will require the passing in the number of polygons in the sequence to the initializer.

The Polygon objects should be immutable, as should the sequence itself.

In addition, each Polygon should have the following properties:
* number of vertices
* number of edges (sides)
* the edge length
* the apothem (distance from center to mid-point of any edge)
* surface area
* perimeter
* interior angle (angle between each edge) - in degrees
* supports equality based on # edges and circumradius
* supports ordering based on number of edges only

The sequence object should also have the following properties:

* should support fully-featured slicing and indexing (positive indices, negative indices, slicing, and extended slicing)
* should support the `length()` function
* should provide the polygon with the highest `area:perimeter` ratio