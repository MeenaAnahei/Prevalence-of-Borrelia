# Dataset Summary

The *Borrelia burgdorferi* outer surface protein dataset is a molecular
ecology dataset that consists of DNA sequences and other metadata for
four outer surface proteins A,B,C, and p35 (BBA64).This data is derived
from *Ixodes pacificus* ticks and their vertebrate hosts colelcted in
the Bay Area of California.This dataset helps support research on how
the genetic diversity of outer surface proteins correlates with vector
and host diversity which provides insights into the transmission
dynamics of *Borrelia* in the western United States.

# Languages

English

# Data Instances

Each data point represents a tick or host with DNA sequence data for at
least one or two outer surface proteins along with metadata about the
collection and identification.

    # load dataset in and read first rows
    osp <- read.csv("osp_data.csv")
    head(osp)

    ##   Site Collection.Date  Sample.ID Leave.samples.with.AL.initial.for.me.to.run....They.have.very.little.sample.left Year Sample.Type Species       Borrelia
    ## 1 CCSP       4/19/2018 18CCSP.340                                                                               AL 2018        Tick    IPAC B. burgdorferi
    ## 2 CCSP       4/19/2018 18CCSP.342                                                                        Cant find 2018        Tick    IPAC B. burgdorferi
    ## 3 CCSP       4/19/2018 18CCSP.502                                                                               AL 2018        Tick    IPAC B. burgdorferi
    ## 4 CCSP       4/19/2018 18CCSP.605                                                                                  2018        Tick    IPAC B. burgdorferi
    ## 5 CCSP       4/19/2018 18CCSP.613                                                                                  2018        Tick    IPAC B. burgdorferi
    ## 6 CCSP       5/28/2018 18CCSP.723                                                                               AL 2018        Tick    IPAC B. burgdorferi
    ##   Tissue.Extraction.date...day.1. Tissue.Extraction.individual.LAST.name OspA.nPCR.date OspA.nPCR.person OspA.nPCR.result OspA.gel.date OspA.gel.person OspA.Sequence.Date
    ## 1                        10/15/18                                   Eric         2/6/25           Anahei              pos        2/7/25          Anahei                   
    ## 2                        10/15/18                                   Eric            n/a              n/a              n/a           n/a             n/a                n/a
    ## 3                        10/15/18                                 Sukhie         2/6/25           Anahei              pos        2/7/25          Anahei                   
    ## 4                        10/22/18                                   Eric                                                                                                  
    ## 5                        10/22/18                                   Eric                                                                                                  
    ## 6                        10/22/18                                   Eric         2/6/25           Anahei              pos        2/7/25          Anahei                   
    ##   ospA_genotype Genbank.Accession...ospA OspA.Sequence.Result Notes OspB.nPCR.date OspB.nPCR.person OspB.nPCR.result OspB.gel.date OspB.gel.person OspB.Sequence.Date ospB_genotype
    ## 1                                                                                                                                                                                  
    ## 2           n/a                      n/a                  n/a   n/a            n/a              n/a              n/a           n/a             n/a                n/a           n/a
    ## 3                                                                                                                                                                                  
    ## 4                                                                                                                                                                                  
    ## 5                                                                                                                                                                                  
    ## 6                                                                                                                                                                                  
    ##   Genbank.Accession...ospB OspB.Sequence.Result Notes.1 p35.nPCR.date p35.PCR.person p35.nPCR.result p35.gel.date p35.gel.person p35.Sequence.Date p35_genotype
    ## 1                                                                 n/a            n/a             n/a          n/a            n/a               n/a          n/a
    ## 2                      n/a                  n/a     n/a           n/a            n/a             n/a          n/a            n/a               n/a          n/a
    ## 3                                                                 n/a            n/a             n/a          n/a            n/a               n/a          n/a
    ## 4                                                                 n/a            n/a             n/a          n/a            n/a               n/a          n/a
    ## 5                                                                 n/a            n/a             n/a          n/a            n/a               n/a          n/a
    ## 6                                                                 n/a            n/a             n/a          n/a            n/a               n/a          n/a
    ##   Genbank.Accession...p35 p35.Sequence.Result Notes.2 OspC.nPCR.date OspC.nPCR.person OspC.nPCR.result OspC.gel.date OspC.gel.person OspC.Sequence.Date ospC_genotype
    ## 1                     n/a                 n/a     n/a            n/a              n/a              n/a           n/a             n/a                n/a           n/a
    ## 2                     n/a                 n/a     n/a            n/a              n/a              n/a           n/a             n/a                n/a           n/a
    ## 3                     n/a                 n/a     n/a            n/a              n/a              n/a           n/a             n/a                n/a           n/a
    ## 4                     n/a                 n/a     n/a            n/a              n/a              n/a           n/a             n/a                n/a           n/a
    ## 5                     n/a                 n/a     n/a            n/a              n/a              n/a           n/a             n/a                n/a           n/a
    ## 6                     n/a                 n/a     n/a            n/a              n/a              n/a           n/a             n/a                n/a           n/a
    ##   Genbank.Accession...ospC OspC.Sequence.Result Notes.3
    ## 1                      n/a                  n/a     n/a
    ## 2                      n/a                  n/a     n/a
    ## 3                      n/a                  n/a     n/a
    ## 4                      n/a                  n/a     n/a
    ## 5                      n/a                  n/a     n/a
    ## 6                      n/a                  n/a     n/a
