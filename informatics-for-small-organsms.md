# Informatics for 'small' organisms: A green paper.

Michael Ashburner and Susanna Lewis (FlyBase); Lincoln Stein and Paul Sternberg (WormBase).

November 2001, revised April 2002, HTML mark up September 2002

Many 'small' organisms, small not in the physical sense but in the sense that their community of researchers is small, have an urgent need for databases and informatics tools. They look at the 'large' organisms, organisms with a substantial research community, and see that these have well-funded informatics infrastructure supporting the community's research. The obvious question that then arises is: 'how can these guys help us ?' This green paper is a first attempt to address this question.

All organisms, both large and small, have a need of informatics support for two quite different reasons. The first is to serve the research needs of their own communities; the other is to serve the needs of the broader biomedical community who must be able to exploit the great strengths of the comparative approach to biological research.

Both the 'small communities' and their funders are nervous of investing in databases and associated informatic tools. They are nervous for several reasons - their inability to make informed technical decisions; their fear that funding informatics will divert resources from what some still regard as 'real research'; their fear that a commitment to informatics infrastructure will lead them into a never-ending, inescapable development morass. To the funders we can only say that without a suitable informatics infrastructure there is now little point in funding biological research.

This document attempts to establish some criteria that may be used to address the first of these fears, inexperience with informatics.

1. You must, to be successful, have the support of your research community. Get it. This is rule number one.

2. Work towards the greater good, because indulging in power wars leads directly to failure. Once a community does decide to take the leap and concludes that it does require informatics in order to successfully carry out research, then everyone responsible must keep this objective in mind, and not waste energy on ego battles.

3. Talk to those with experience with the 'large' organism databases, e.g., FlyBase, Mouse Genome Database, The Saccharomyces Genome Database, WormBase, The Arabidopsis Information Resource. Talk to those with recent experience in beginning organism databases, e.g., RatBase, DictyBase. Talk not only with their PI's, but also to their curators and computer scientists. Study these databases and learn from them; see what tools they use.

4. Decide, as a matter of practice and principle, to re-use rather than re- invent. Do not be 'original' simply for the point of it; but be inventive when a need cannot be otherwise satisfied. Develop software as 'open source', which is both a specific practice and way of thinking. This means (a) using open source rather than proprietary software and tools and (b) making your own database and any tools associated with it open source. The GMOD site will increasingly have software designed to be used by other model organism databases. If you do need to write your own software for a particular purpose consider contributing to this site.

	[The term Open Source is most usually applied to code, but the philosophy behind the Open Source 'movement' is as equally applicable to data. Read Raymond's 'The Cathedral & The Bazaar' and DiBona et al. (1999) 'Open Sources'. For a definition of Open Source see Appendix B in DiBona et al. 1999.]

5. Spend time understanding abstract representations of the relevant data models describing your domain. Learn how to describe your data at the conceptual level and capturing what is fundamental to its character.

6. Follow the field - subscribe to the email discussion lists from groups such as GMOD and GO. Go to meetings such as ISMB, PAGA, the Gene Ontology Consortium Open meetings, the CSH Sequencing Meeting etc. Work with the other major databases, especially the International Nucleic Acid Sequence Database (GenBank/EMBL-bank, DDBJ), SWISS-PROT, InterPro and the Gene Ontology Consortium. They can help you enormously.

7. Invest in collaborations; meet face-to-face with your collaborators at least three times a year; supplement these with video conferences and conference calls. Invest in quality time with your collaborators.

8. Remember: 'perfection is the enemy of the good'. Do not wait until your data and database and tools are 'perfect' before releasing to the community. They never will be. Get the data out, improve the database and interfaces incrementally. Start with the easy stuff, for example a 'complete' literature reference data set or a community address list.

9. Scope your database - avoid creeping 'featurism'. This is not as easy as it sounds and requires that you really think about what you want to provide to your users and, even more importantly, what they need.

10. Think long-term about the future of your database. Worry, well before the event, how you will ensure that critical work will continue when the founders retire, are fired or get fed up.

## The three levels.

1. Curation - data in.
2. Databasing - data storage and organisation.
3. Access - data out

Details:
1. Curation. This term generally covers four different, but inter- connected, processes:
-- Sequence curation, or rather the curation of sequence annotation: Very often the sequence, and its associated primary annotation, will be coming from an independent sequencing lab. By primary sequence annotation we mean the results of the first high- throughput annotation of the sequence, often dominated by computational data, rather than the product of human curation. Insist that you obtain these data in a standard rich format (e.g. GAME XML, GFF), rather than as GenBank or EMBL-Bank format flat files. For the maintenance of annotation (by computational methods and by curation of the published literature) do not attempt to develop your own tools, but use one that is available from the community and which will interact with your database.
-- Other high-throughput data: ESTs, cDNAs, Increasingly you may need to curate data from high-throughput 'post-genomic' projects, expression arrays, protein-protein interactions etc. This will often require the ability to write one-off scripts to parse data formats.
-- Literature curation: Even if your database only includes annotations on sequence then you will need to curate information from the published scientific literature. This will require tools. Note that, as good as they are neither PUBMED nor MEDLINE cover the entire scientific literature.
-- Curation of personal communications from the community. Much data never gets published in the conventional sense but is immensely useful. Encourage the community to submit it to you. Attempt to archive data from personal web sites maintained by researchers, thus ensuring its persistence beyond the life of one well organized postdoc. Always attribute data to its source, never enter data 'ex cathedra', but attribute it to a particular named 'pope'.

2. Databasing. Do not spend even one minute debating low-level implementation details, for example, Sybase vs. Oracle vs. object orientated database management systems. Rather, accept the fact that particular technological solutions are transitory as that technology improves. Technical differences are negligible relative to differences in skills between individual developers and therefore implementation decisions are best determined by the experience of the personnel that is available. Note that Open Source relational database management systems, such as mySQL and postGRESS, are now reasonably mature.

3. Access. Who is your community ? Let us answer this - it is the community of researchers who work with 'your' organism, it is the greater community of biological and biomedical researchers who, increasingly, need to access data from other species and, it is the community of bioinformaticists who will want to 'mine' your data.

	Ensure that access to your database will not be limited to a WWW- based query tool but will also include access to the entirety of the data in a format that allows computation. Do not kid yourself that a web query interface satisfies the community's needs for access.

## Some references and sources.

### Open Source:

DiBona, C., S. Ockman and M. Stone (editors) (1999). OpenSources. O'Rielly, Sebastopol, CA.
Raymond, E.S (1999). The Cathedral & The Bazaar. O''Rielly, Sebastopol, CA.

### Some model Organism database URLs:

Arabidopsis: http://www.arabidopsis.org/
DictyBase: http://dictybase.org/
FlyBase: http://flybase.bio.indiana.edu/
Mouse Genome Database: http://www.informatics.jax.org/
RatBase: rgd.mcw.edu/
Saccharomyces Genome Database: http://genome-www.stanford.edu/Saccharomyces/
Wormbase: http://www.wormbase.org/

### Other database URLs:

NCBI: http://www.ncbi.nlm.nih.gov/
EBI: http://www.ebi.ac.uk/
DDBJ: http://www.ddbj.nig.ac.jp/
SWISS-PROT: http://www.ebi.ac.uk/swissprot/
InterPro: http://www.ebi.ac.uk/interpro/
Gene Ontology Consortium: http://www.geneontology.org/
GMOD: http://sourceforge.net/projects/gmod

### Data formats:

GAME XML: http://www.bioxml.org/Projects/game/
MAML: http://sourceforge.net/projects/mged/
GFF: http://www.sanger.ac.uk/Software/formats/GFF/index.shtml

### Meetings:

ISMB: http://www.ismb02.org/
GO: http://www.geneontology.org/
Cold Spring Harbor: http://nucleus.cshl.org/meetings/
Open Source RDMS:

mySQL: http://www.mysql.com/
PostGRESS: http://www.postgresql.org/