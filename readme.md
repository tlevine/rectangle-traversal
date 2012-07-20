Direction of traversal of rectangles by people as a function of sight lines
=======

## Introduction

For a while, I've been thinking that a shorter person is more likely to start
with the short leg when traversing a rectangle. After a further ponder, I
think relates to whether they can see their final location; somatic education
methods like Alexander Technique claim that vision is important in guiding
movement. This leads me to a slightly different hypothesis:

> Given two paths of equal distance to a goal, a person is more likely to
> choose the path where the goal is visible sooner.

In the case of the rectangle, this would mean that people would start
with the short leg if they can't see the target, as getting to the long
leg would help them see the target. It might also mean that they would
start with the long leg if they can see the target because starting with
the short leg would make them turn further away from the target at first,
making it harder to see.

Depending on how rectangular paths are designed, this potential relationship
could be confounded with effects of handedness; theories like right-hand
preference suggest that, other things being equal, people might be more likely
to start with the right side (more specifically, the side of their handedness).

## Methods

Participants were made to chose how to traverse a rectangular table in order
to retrieve beers from the opposite corner. The table arrangement and beer
location were varied, and route of travel was recorded.

### Room setup

A long table was placed in the middle of the room. Two beers were placed at one
corner, and an "X" was drawn on the floor at the opposite corner.

### Participants

Participants were recruited at a [frat party, picnic, &c.] in [place]; they were
offered a beer in return for participation in a one-minute experiment.
[Demographics based on study setting--general age, location, &c.].

### Procedure

Participants were asked to stand at the X and were given the following directions.

1. Do not start walking until I say "start".
2. There are two beers at the opposite corner of the table.
3. When I tell you, walk to the opposite corner of the table, and pick up the beers.
4. After you pick them up, bring them back here, and put either one on this "X".
5. You may keep the other beer.

After giving these directions, the experimentor asked "Do these directions make
sense?" and clarified any resulting misunderstandings. Once the directions were
clear, the experimentor told the participants, "Please start."

As the participant traversed the table, the experimentor drew two arrows on a
form (figure [form]) to indicate whether the participant turned left or right
at the start of each of the two legs of the trip (from the "X" to the beers
and from the beers to the "X").

[]
Figure [form]

After the participant returned the beer, the experimentor asked for the
participants handedness and then debriefed the participant.

### Variables

Before the participant entered the experiment room, it was configured into
one of four ways based on two two-level factors:

1. target location and
2. short leg.

At the end of the experiment, handedness was collected.

#### Target location
Target location was one of "floor" or "table". Beers were placed on the floor
in the floor condition and on the table in the table condition
(figure [target_locations]).

[]
Figure [target-locations]

They also had a specific placement in the horizontal axes. In both conditions,
the beers were placed within [four inches] of the corner point. In the table
condition, the beers were placed approximately along the diagonal of the
rectangular table that included the corner point. In the floor condition, the
beers were placed [four inches] from the corner in the opposite direction,
so they were not underneath the table.

Given the table dimensions and the beer placement, participants should have
been able to see the beers in the floor condition when they were at either
of the adjacent corners but not when they were at the opposite corner. In the
table condition, participants should have been able to see the beers from any
corner.

#### Short leg

A rectangle has four different vectors that connect opposite corners (figure
[vectors]). These vectors correspond to the routes that we could have asked
participants to traverse.

Participants were expected to walk around the table rather than over or under
the table. (We ignored any participants who walked through the table.)
In these expected paths, a participant would first turn one direction (left
or right), then traverse a leg of the table, then turn the other direction
and traverse the remaining leg. In order to control for affects of handedness,
we classified these four routes into two route types.

1. Short leg left, long leg right: If the participant turns left first,
    he traverses the short leg first.
2. Short leg right, long leg left: If the participant turns left first,
    he traverses the long leg first.

These are also diagramed in figure [path types].

[]
Figure [path types]

I randomly chose one leg from each of these two route types to use for the entire
study. Only one of these route types was used for each particular participant,
and the route type was randomly chosen for each trial. The beer and "X" were
placed according to this route type definition.

#### Handedness
Participants were asked for their handedness, which was recorded as "left",
"right" or "other". Data from participants with "other" handedness were
ignored.

### Route choice

Direction of each leg of travel was recorded on a form (section [whatever]) and
then translated into a "left", "right" or "other". If participants took routes
that did not fit neatly into "left" or "right", such as jumping over the table
or back-tracking, the direction was marked as "other", and the trial was ignored.

### Model

Data were transformed into four binomial variables:

1. Target location (floor or table)
2. First side of first leg of travel (left, right other)
3. First side of second leg of travel (short, long or other)
4. Short leg matches handedness (yes, no or other)

The first of these variables should be straightforward given the earlier
definition. The second variable corresponds to the route taken to retrieve
the beer. The third variable corresponds to the route taken to return the beer
to the "X".

The fourth variable relates two variables that were collected. One of these
variables is handedness. The other is the "short leg" variable discussed earlier.
That is, it's whether the table was arranged with the short leg to the left or
the right of the "X" from the point of view of the participant. When handedness
was "other", this variable was also "other".

If any of the variables was "other", the trial was ignored.

These four variables were modeled with bivariate analysis of variance with two
main effects and their interaction. Since all values of "other" were ignored,
all of the variables had exactly two levels.

## Results

[Some number of] people participated in the study. Here are some summary
statistics.

Regarding our interventions,

* [] trials had the short leg left and the target location floor
* [] trials had the short leg left and the target location table
* [] trials had the short leg right and the target location floor
* [] trials had the short leg right and the target location table

```
    Short leg   Target location | Number of trials
    ---------   --------------- | ----------------
    Left        Table           | 
    Left        Floor           | 
    Right       Table           | 
    Right       Floor           | 
```

Regarding handedness, [] people were left-handed, [] were right-handed and
[] were "other".

[]% of legs involved left turns first, and []% involved right turns first.
[]% of legs involved short sides first, and []% involved long sides first.

[]% of legs were something else, including [potential hilarity].

The aforementioned model had [reasonable fit statistics] and yielded [these
coefficients] (table [foo] and figure [bar]).

[Table with coefficients]

[Plot with observations and fitted values from the model]

When the target was on the table and the short leg did not match handedness,
people were [more likely to take the long leg?].
When the target was on the table and the short leg did match handedness,
people were [more likely to take the short leg?].
When the target was on the floor, [people were more likely to take the short
leg regardless of whether it matched handedness].

### Discussion

[It appears that both handedness and position of beer affect the choice of
route around the rectangular table, with the latter having a stronger effect.]

This relates to the relevance of vision in human movement.

More immediately, the study results can be used in the design of paths.
If people prefer to see the endpoint of their travel, landmarks can be
positioned or obscured in order to direct traffic to whichever path the
designer intends.

## Conclusion

[These results support the hypothesis?]

## Future research

* Alexander Technique
* Applications in parks, streets, &c.
