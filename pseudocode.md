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
    - yarn
    - knitting needles (2)
    - measuring tape
<!-- stitch counter? -->

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
// this would then lead to a loop //
```
