<!-- pseudocode before the pseudocode:
    - include assumptions?
    - need to start with obtaining the materials aka variables
    - then preparation of casting on the yarn onto a needle
    - setting up how you hold the yarn
    - knit function
    - purl function
    - loop to finish
    - finish off function
    - if else function? - maybe with the count of stitches? or how long you want the swatch??
    - parameters might be the numnber of stitches and color?
-->

# KNITTING A GAUGE SWATCH

## ABOUT:
- What is knitting gauge?
- Knitting gauge corresponds to each individual knitter's tension when knitting. By testing your own knitting gauge you can determine what you need to adjust to acheive the same sized results as a pattern you are following.
- This specific pseudocode will describe creating a stockinette stitch gauge swatch.

## ASSUMPTIONS:
- know how to cast on
- know how to do a knit stitch
- know how to do a purl stitch

## INIT - variables for program
1. yarn
2. knitting needles (2)
3. measuring tape
<!-- maybe add a stitch counter?- that would lead to another function to check stitch count or row count -->

**EXAMPLES**
```
example of a yarn object
    var yarn = {
        brand: 'Bernat',
        type: 'Blanket',
        color: 'almond',
        weight: 6,
        recommendedKnittingNeedleSize: 11,
\\ these are the properties of the yarn variable \\
    }

example of knitting needle
    var knittingNeedleSet {
        brand: 'knitpicks',
        type: 'circular',
        size: 11,
    }
```

## PREPARATION:
```
FUNCTION gatherMaterials:
    * yarn
    * knitting needle matching set (2)
    * measuring tape

FUNCTION checkMaterials:
    a. look at label of yarn and determine yarn weight and corresponding needle size
        *IF yarn label's recommended needle size matches the needle size of the set you have
            THEN
                CONTINUE to KNITTING
            ELSE
                find/buy knitting needles to match the yarn label's recommended needle size

// this would then lead to a loop until continue to KNITTING//
```
<!-- checkMaterials: function() {
        if (yarn.recommendedKnittingNeedleSize == knittingNeedleSet.size) {
            continue to knitting;
        } else if (yarn.recommendedKnittingNeedleSize < knittingNeedleSet.size) {
            REPEAT until....
        } else if (yarn.recommendedKnittingNeedleSize < knittingNeedleSet.size) {
            REPEAT until....
        }
} -->

<!-- matching sizes would return TRUE - if greater than or less than (sizes don't match) would return FALSE -->

## KNITTING THE SWATCH:

```
FUNCTION castOn:
    a. take yarn and cast on stitches UNTIL there are 20 cast on stitches on one needle

FUNCTION holdKnittingNeedles
    a. hold the needle with the casted on stitches in your LEFT hand
    b. hold the needle without stitches in RIGHT hand
    c. place the ball of yarn near you where it won't get tangled by things around it

FUNCTION knit
    a. create a knit stitch using both needles and slip it to the right hand needle
    b. repeat knit stitches until all 20 are on right hand needle

\\ maybe for loop to reach 20 stitches inserted here... \\

FUNCTION turn
    a. turn around (left to right) your work around so now that the needle with the new stitches is now in your LEFT hand and the needle without stitches is in your RIGHT hand

FUNCTION purl
    a. create a purl stitch using both needles and slip it to the right hand needle
    b. repeat purl stitches until all 20 are on right hand needle

FUNCTION finishOFF
    a. check for 20 rows of your stitches so that you have a completed swatch
        * IF 20 rows are counted
            THEN
                FINISH off the final row and continue to next function

FUNCTION takeOffNeedles
    a. slide newly finished swatch off of needle
```
<!--
    - if else to check for 20 stitches each time? or loop until 20 stitches are made
    - could also insert another function to check if you are on the right or wrong side of your knitting to determine whether to knit or purl if you drop/forget your progress
    - so next do a loop to repeat the functions for knitting, turning, and purling functions to create the rows     until the full square swatch is formed
    - should those three actions actually be one full function instead to loop?
    - can insert a final function on how to measure your swatch to test gauge
-->

## START/INIT

```
gatherMaterials
checkMaterials

castOn
holdKnittingNeedles
knit
turn
purl
finishOff
takeOffNeedles

```

## END
