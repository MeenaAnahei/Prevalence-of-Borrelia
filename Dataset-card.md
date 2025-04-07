# Dataset Summary

The *Borrelia burgdorferi* outer surface protein dataset is a molecular
ecology dataset that consists of DNA sequences and other metadata for
four outer surface proteins A,B,C, and p35 (BBA64).This data is derived
from *Ixodes pacificus* ticks and their vertebrate hosts collected in
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

# Rationale

This data set was curated to explore the genetic variation of outer
surface proteins that are crucial for the survival and transmission of
*Borrelia.* OspA and B are expressed in the tick mid gut while C and p35
are expressed in the hosts. Understanding the variation across tick and
hosts species provides insights into the ecology of Lyme Disease.

# Initial Data Collection and Normalization

Samples were collected during tick season of April-May 2018-2024 in the
Bay Area of California.Ticks were collected from vegetation and ear
punches were taken from hosts then stored in ethanol. DNA was then
extracted and gene specific PCR was performed to confirm the presence of
outer surface proteins.

# Annotation Process

PCR results were interpreted from gel electrophoresis banding patterns.
Positive bands were recorded verifying the tick and host IDs.

# WHo are the Annotators

Original collectors, identifiers, and DNA extractors were undergraduate
and graduate researchers from San Francisco State University. For PCR
and electrophoresis, graduate researchers.

# Personal and Sensitive Information

This dataset contains the names of the collectors, identifiers, and
those who conducted every wet lab experiment.

# Social Impact of Dataset

This enhances the understanding of *Borrelia burgdorferi* distribution
and outer surface protein expression in the western US. This region of
the US has been less understood in terms of Lyme disease ecology. With
this dataset, it can further inform public health efforts in vector
surveillance and control.

# Discussion of Biases

Sampling was limited to ticks collected at specific sites in the Bay
Area of California. Some sites had more collections than others due to
abundance and weather at the time of tick and mammal collection. Host
diversity may be biased by the trapping success.PCR detection may depend
on DNA quality and primer performance.

# Other Known Limitations

Mixed infections can possibly be under detected due to the PCR protocol
being used that takes into account one species of *Borrelia*. There is
temporal variation not taken into account from the samples collected
across all 7 years. There is a possibility of cross contamination and
the risk of false positives as PCRs are sensitive especially if they’re
not controlled.

# Dataset Curators

This dataset was created by Swei Lab at San Francisco State University.
