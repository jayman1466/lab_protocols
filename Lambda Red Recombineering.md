# Lambda Red Recombineering Protocol
This protocol will allow you to use lambda red recombineering to site-specifically integrate or delete fragments in bacterial (usually E. coli) genomes. 

## Strain Requirements
This type of genome engineering requires your strain to have three genes from the Lambda bacteriophage - Beta, Exo, and Gam. The E. coli strains EcNR1 and EcNR2 contain these genes already integrated into the BioAB locus into the genome. If working with other strains, you can use the plasmid **pORTMAGE** (available on Addgene) to introduce these genes into your strain.

## DNA Requirments
As a substrate, Lambda Red uses linear DNA (usually a PCR product) that contains **50bp homology arms** corresponding to the target site in the genome. For more info see [here](https://blog.addgene.org/lambda-red-a-homologous-recombination-based-technique-for-genetic-engineering).

### For knockouts
Knocking out genes with lambda red is not that efficient (usually 1 in 100,000 cells), so you need to select for the knockout using an antibiotic selectable marker. For this you would PCR amplify an antibiotic selectable marker with primers that incorporate 50bp homology arms corresponding to the locus you are knocking out.

### For insertions 
Similar to knockouts, for insertions, you would amplify the cassette-of-interest with primers than incorporate 50bp homology arms corresponding to the integration locus. Your cassette should include some sort of selectable market to select for successful integrations.  

### Note on PCR productes
When PCR amplifying from plasmids, make sure to gel-purify and/or dpn1 digest the product to remove the plasmid template, which will interfere with downstream steps.

## Protocol
1. Grow up your strain (which contains the Lambda Red genes) in 3mL LB at 30-34C until OD 0.4-0.6.
1. Heat shock your culture for 15 minutes at 42C in a skaking water bath. This will induce the lambda red genes.
1. Place the culture on ice. Take 1mL of the culture an move into a 1.5mL eppendorf tube.
1. Spin down (ideally in a cold centrifuge) 10000rpm for 30sec. 
1. Wash pellet with 1mL ice-cold sterile water.
1. Repeat wash an additional time.
1. Do a final spin and resuspend pellet in 50uL sterile cold water.
1. Add 50-100ng PCR product. 
1. Transfer for a cold 1mm electrocuvette.
1. Electroporate (1800V, 200ohm resistance, 25uF capacitance). The time constance should be >4.8ms.
1. Recover in 3mL LB at 30-34C for 2.5-3 hours.
1. Spin down entire culture and spread onto selective solid media. Incubate at 30-34C.
1. In e. coli, colonies should appear within 24-36 hours.

## Curing your strain of pORTMAGE
If you used pORTMAGE as the source of the lambda red genes, it'll be useful to get rid of that plasmid. To do so, culture the strain for 24 hours at 34C (without adding the antibiotic that selects for pORTMAGE). Then culture another 24 hours at 37C (again without the antibiotic that selects for pORTMAGE). Then plate on LB. Check single colonies to see if they lost the plasmid.
