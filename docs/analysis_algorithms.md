<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

# Analysis Algorithms

*EPANET uses a variety of algorithms for the hydraulic and water quality analysis. This chapter describes the two different demand models used for hydraulics analysis and the algorithms for the water quality analysis.*


.. _sec-analysis_alg_hyd:

## Hydraulics

  The method used in EPANET to solve the flow continuity and headloss equations
  that characterize the hydraulic state of the pipe network at a given point in
  time can be termed a hybrid node-loop approach. Todini and Pilati (1987) and
  later Salgado et al. (1988) chose to call it the "Gradient Method". Similar
  approaches have been described by Hamam and Brameller (1971) (the "Hybrid
  Method) and by Osiadacz (1987) (the "Newton Loop-Node Method"). The only
  difference between these methods is the way in which link flows are updated
  after a new trial solution for nodal heads has been found. Because Todini's
  approach is simpler, it was chosen for use in EPANET.

  Todini (2003) describes how the Gradient Method can be extended to simulate
  pressure driven demands (PDD). The latest version of EPANET has been
  updated to include these capabilities. A water distribution pipe network
  can now be analyzed two ways, 1) assuming demand, and 2) assuming
  pressure driven demands. The subsections that follow provide a technical
  description for these two demand models.


**Fixed Demand Model**

  Assume we have a pipe network with ${N}$ junction nodes and ${NF}$
  fixed grade nodes (tanks and reservoirs). Let the flow-headloss relation in a
  pipe between nodes $i$ and $j$ be given as:

  .. math::
     :label: eq:pipe_headloss

     $$ H_{i} - H_{j} = h_{ij} = rQ_{ij}^{n} + mQ_{ij}^{2} $$

  where $H$ = nodal head, $h$ = headloss, $r$ = resistance
  coefficient, $Q$ = flow rate, $n$ = flow exponent, and $m$
  = minor loss coefficient. The value of the resistance coefficient will depend
  on which friction headloss formula is being used (see below). For pumps,
  the headloss (negative of the head gain) can be represented by a
  power law of the form

