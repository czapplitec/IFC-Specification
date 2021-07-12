The IfcAlignmentVerticalSegmentTypeEnum indicates the type of a segment of a vertical alignment segment (IfcAlignmentVerticalSegment).


| Vertical curvature | Segmenttype        | Enumeration Values |
|:----|:------------------|:----------|
| No vertical curvature | constant gradient        | CONSTANTGRADIENT |
| Derivative of gradient with respect to horizontal projection of alignment is constant | Vertical curve, parabola  | PARABOLICARC |
| Derivative of vertical angle with respect to 3D arc length along the alignment is constant | Vertical curve, circular | CIRCULARARC  |
| Variation of vertical curvature is constant | Vertical curve, clothoid | CLOTHOID  |


&gt;NOTE A vertical curve in track that starts or ends in canted switches and crossings can be of a higher order polynomial than a parabola.

&gt;NOTE chainage is  longitudinal distance along the horizontal projection of the alignment (e.g. track centre line).


&gt;NOTE Definitions according to EN 13803/2017 (except CLOTHOID)



**Used Symbols and their meaning**


| Symbol&nbsp; | meaning  | Unit, value range |
|:----|:------------------|:----------|
| L | full length of segment        | positive length  L > 0 |
| s | current position on segment        | 0 < s < L |
| &theta; | (Greek "theta") Longitudinal slope angle (incline or decline)   | rad |
| g | gradient (math); g=tan(&theta;) |  |
| x(s) | variable longitudinal coordinate of the projection of the alignment / track centreline into the ground plan.  | length |
| y(s) | variable transverse coordinate of the projection of the alignment / track centreline into the ground plan.  | length |
| z(s) | Variable vertical coordinate of the projection of the track centreline in plan in a Cartesian coordinate system in the vertical direction.  | length |
| z<sub>c</sub>(s) | Ordinate of the vertical circular arc of measured away from the tangent line at position s.  | length |
| L<sub>V</sub> | length of vertical radius radius (inverse curvature)  | length |
| R<sub>V</sub> | radius (inverse curvature) of the track centreline at a point in the elevation diagram (longitudinal section)  | length |
| &kappa;<sub>V</sub> | (Greek "kappa") Vertical curvature   | 1/radius<sub>V</sub> |
| Z<sub>G</sub> | Distance of the tangent intersection from the chord of the vertical circular arc  | length |
| Z<sub>M</sub> |  Distance of the centre of the vertical circular arc to the tangent intersection point (stitch height) | length |
| l<sub>T</sub> | Length of the tangents of the  vertical circular arc | length |

&gt;NOTE Symbols according to EN 13803/2017

&gt;NOTE gradient has a slightly different definition in civil engineering. "Gradient (Civ.Eng.) is the degree of slope, e.g. of a highway or a railway. US grade".

&gt;NOTE most railway track designs use the **small angle assumption**. That means &theta;=tan(&theta;)=gradient.

**References to EN 13803/2017**

EN 13803/2017 covers "Track alignment design parameters". As such it is not fully compatible with definitions for IFC Alignment. Therefore rail specific terms like track have been replaced with more general terms also applicable to road design.

Referenced content of EN 13803/2017 "Table 2 - Elements for vertical alignment" has been modified as follows:

**Vertical curve, parabola:** Derivative of gradient with respect to chainage is constant<br/>
**Generalized:** Derivative of gradient with respect to horizontal projection of alignment is constant

**Vertical curve, circular:** Derivative of vertical angle with respect to sloping length along the track is constant<br/>
**Generalized:** Derivative of vertical angle with respect to 3D arc length along the alignment is constant

EN13803 clause 3.5:
**Chainage**: longitudinal distance along the horizontal projection of the track centre line.
